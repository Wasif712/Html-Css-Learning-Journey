# Accessibility kya hai?
Web accessibility is the practice of designing and developing websites so that people with different abilities can access,
understand, navigate, and interact with web content.

Accessibility ka matlab hai website ko aise banana ke different abilities wale users bhi website ko properly use kar saken.
For example:
keyboard user
screen-reader user
visually impaired user
user with motor difficulties
mobile user

## Simple rule:
Navigation = <a>
Action = <button>

### Empty alt screen reader ko indicate karta hai ke image meaningful content nahi provide karti.

## Important concepts
caption → table ka purpose.
th → heading.
scope="col" → column heading.
scope="row" → row heading.

# Keyboard Navigation
Accessibility ka ek major concept:
User website ko mouse ke baghair operate kar sake.
Common keyboard keys:
TAB → next interactive element
SHIFT+TAB → previous
ENTER → activate link/button
SPACE → activate buttons / controls
ESC → close applicable UI
Abhi CSS/JS nahi aaye, lekin HTML structure keyboard accessibility ka foundation create karta hai.

# Definition <dl>
The <dl> element represents a description list containing terms and their associated descriptions.
Structure:
<dl>
<dt>Term</dt>
<dd>Description</dd>
</dl>
Useful for:
profile information
specifications
metadata
glossary
key/value information

# Definition
<caption> — Exam Point
The <caption> element provides a title or description for an HTML table.
Example:
<table>
<caption>Student Attendance</caption>
...
</table>
Accessibility aur table understanding dono mein useful.

# Question Answers
- What is Web Accessibility?
Web accessibility is the practice of making websites usable by people with different abilities and disabilities.
- What is ARIA?
ARIA (Accessible Rich Internet Applications) provides attributes that can improve the accessibility semantics of dynamic web content and user
interface components.
- What is an accessible form?
An accessible form provides clear labels, logical grouping, keyboard accessibility, meaningful controls, and appropriate feedback to users.
- Why is semantic HTML important for accessibility?
Semantic HTML provides meaningful structure that helps browsers, assistive technologies, developers, and users understand the purpose and
relationships of content.
- What is the difference between a link and a button?
A link is primarily used for navigation to another resource or location, while a button is primarily used to perform an action.
- What is the purpose of alt ?
The alt attribute provides alternative text for an image when the image cannot be perceived or displayed.

