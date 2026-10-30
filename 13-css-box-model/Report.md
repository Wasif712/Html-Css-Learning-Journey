# CSS Box Model
The CSS Box Model describes how every HTML element is represented as a rectangular box consisting of content, padding, border, and margin.
Roman Urdu mein: Har HTML element browser ke nazdeek ek box hota hai.

         MARGIN
┌─────────────────────┐
│        BORDER       │
│  ┌───────────────┐  │
│  │    PADDING    │  │
│  │ ┌───────────┐ │  │
│  │ │  CONTENT  │ │  │
│  │ └───────────┘ │  │
│  └───────────────┘  │
└─────────────────────┘


# Content
Content actual information hoti hai.
Example: <h1>Build Better Software</h1>
Build Better Software content hai.
CSS:
h1 {
width: 500px;
height: 100px;
}
Yahan width/height normally content area ko affect karti hai depending on box-sizing .

# Padding
Definition: Padding is the space between an element's content and its border.
Padding element ke andar space create karti hai
Example:
.card {
padding: 30px;
}
Visual:
┌─────────────────┐
│                 │
│     padding     │
│ ┌─────────────┐ │
│ │   CONTENT   │ │
│ └─────────────┘ │
│                 │
└─────────────────┘

# Margin
Definition: Margin is the space outside an element's border that separates it from surrounding elements.
.card {
margin: 30px;
}

## Difference:
padding = inside
margin = outside

# Border
Three parts: border-width, border-style, border-color
Example:
.card {
border-width: 2px;
border-style: solid;
border-color: black;
}
Shortcut:
.card {
border: 2px solid black;
}

# Four-Side Syntax
Padding:
.card {
padding: 10px 20px 30px 40px;
}
Order: Top, Right, Bottom, Left
Clockwise:
       TOP
        ↑
LEFT ← box → RIGHT
        ↓
     BOTTOM

# One Value
.card {
margin: 20px;
}
All sides:
Top = 20px
Right = 20px
Bottom = 20px
Left = 20px


# Two Values
.card {
padding: 20px 40px;
}
Means:
Top = 20px
Bottom = 20px
Left = 40px
Right = 40px

# Three Values
.card {
margin: 10px 20px 30px;
}
Means:
Top = 10px
Left = 20px
Right = 20px
Bottom = 30px

# Box Sizing
Deff: The box-sizing property defines how the total width and height of an element are calculated.Two major values: content-box, border-box
This is one of the most important CSS concepts.
Default: box-sizing: content-box;
Suppose:
.card {
width: 300px;
padding: 20px;
border: 5px solid black;
}

With content-box :
Content = 300px
Padding = 40px
Border = 10px
Total = 350px

Formula:
Total Width
=
Content
+
Left Padding
+
Right Padding
+
Left Border
+
Right Border

# border-box
Modern CSS projects commonly use:
* {
box-sizing: border-box;
}
Now:
.card {
width: 300px;
padding: 20px;
border: 5px solid black;
}
Total outer width:
300px
Padding and border width ke andar calculate hote hain

# max-width
Professional websites mein extremely useful:
.container {
width: 100%;
max-width: 1200px;
}
Meaning:
Element 1200px se zyada wide nahi hoga.

# Centered Container
.container {
width: 100%;
max-width: 1200px;
margin: 0 auto;
}
margin: 0 auto horizontal centering ke liye common technique hai.
┌─────────────────────────────────────┐
│                                     │
│      ┌─────────────────────┐        │
│      │                     │        │
│      │   1200px container  │        │
│      │                     │        │
│      └─────────────────────┘        │
│                                     │
└─────────────────────────────────────┘

# min-width
.card {
min-width: 250px;
}
Element ideally 250px se chhota nahi hoga.

# Height
.hero {
height: 500px;
}
Lekin fixed heights carefully use karo.
Agar content zyada ho gaya:
fixed height
↓
content overflow
Isliye real-world websites mein min-height aksar better option ho sakta hai.

# min-height
.hero {
min-height: 500px;
}
Meaning: Hero at least 500px high hoga, lekin content ki requirement ho to aur bara ho sakta hai.

# Overflow
Suppose:
.card {
width: 300px;
height: 100px;
}
Aur content bohat zyada hai. Content box se bahar nikal sakta hai Control:
.card {
overflow: hidden;
}
Common values: visible, hidden, scroll, auto

# overflow: auto
.card {
overflow: auto;
}
Agar content ko scrolling ki zaroorat ho to browser appropriate scrolling provide kar sakta hai.
Real-world use: code blocks, chat windows, tables, dashboards, logs

# overflow-x and overflow-y
Vertical overflow: Responsive tables mein ye bohat useful hoga.
Vertical overflow.
.container {
overflow-x: auto;
}
Horizontal overflow.
.container {
overflow-y: auto;
}

# Border Radius
.card {
border-radius: 12px;
}
Corners rounded.
Circle:
.avatar {
border-radius: 50%;
}

## Individual Corners
.card {
border-top-left-radius: 20px;
border-top-right-radius: 20px;
border-bottom-right-radius: 10px;
border-bottom-left-radius: 10px;
}

# Box Shadow
Definition: The box-shadow property adds shadow effects around an element's box. Example:
.card {
box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
}

Concept:
horizontal offset
↓
vertical offset
↓
blur
↓
spread
↓
color

# Outline
outline border jaisa lag sakta hai, lekin technically different hai.
button:focus {
outline: 3px solid blue;
}

Accessibility ke liye focus indicator important hai.
⚠ Isliye blindly mat lagana.:
*:focus {
outline: none;
}
Keyboard users ke liye focus indication important hai.

# Margin Collapse
CSS ka slightly advanced concept.
Example:
h2 {
margin-bottom: 30px;
}
p {
margin-top: 20px;
}
Vertical margins kuch block formatting contexts mein collapse kar sakti hain. Ye beginner ko confusing lagta hai.
Important idea: 30px + 20px
har case mein automatically: 50px nahi hota.
Browser margin collapsing rules apply karta hai. Aage layouts mein Flexbox/Grid use karne se spacing behavior aur predictable ho jayega.

