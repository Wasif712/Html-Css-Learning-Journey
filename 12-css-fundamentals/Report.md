# What is CSS?
CSS (Cascading Style Sheets) is a stylesheet language used to describe the presentation and visual appearance of HTML
documents.

HTML website ka structure banata hai.
CSS website ki: colors, spacing, size, typography, layout, positioning, responsiveness, animation, waghera control karti hai.

# Simple:
## HTML = Structure
## CSS = Presentation
## JavaScript = Behavior

# Three Ways to Add CSS

## Inline CSS
<h1 style="color: blue;"> DevFlow </h1>
Problem: Large project mein maintain karna difficult.

# Internal CSS
<style>
h1 { color: blue; }
</style>
Ye same HTML document ke <head> mein hota hai. Small experiments ke liye useful.

## External CSS ⭐
Professional websites mein commonly external stylesheet use hoti hai.
<link rel="stylesheet" href="styles.css">

## modern CSS architecture mein styling ke liye classes generally preferred hoti hain.
IDs useful hain:
unique anchors
JavaScript targeting
accessibility relationships
specific document references

# CSS Cascade | Important 
The CSS cascade is the process by which the browser determines which styles are applied when multiple CSS rules target the same element.
p {
color: red;
}
p {
color: blue;
}
Same specificity.
Later rule wins:
blue

# Specificity | Important
CSS specificity is the mechanism used by browsers to determine which selector has greater priority when multiple selectors match the same element.
Basic priority understanding:
Inline styles
↓
ID
↓
Class / attribute / pseudo-class
↓
Element / pseudo-element

Because ID selector has higher specificity than class and element selectors. so green wins.

# Specificity Calculation
Common conceptual notation: (a, b, c, d)
## Where:
a = inline styles
b = IDs
c = classes, attributes, pseudo-classes
d = elements and pseudo-elements

# Inheritance
Inheritance is the CSS mechanism through which certain property values are passed from a parent element to its descendants.
Example:
body {
color: #222;
}

# CSS Variables — Introduction
Modern CSS mein custom properties bohat important hain.
:root {
--primary-color: #2563eb;
--text-color: #111827;
--surface-color: #ffffff;
}
Then:
body {
color: var(--text-color);
}
