# Scenario 07 — HTML Forms

## Project
University Student Registration & Admission Form

## Topics
form, label, input, text, email, password, number, date, tel, url,
radio, checkbox, select, option, textarea, button, fieldset, legend,
required, minlength, maxlength, min, max, autocomplete

## Real World Features
- Personal information
- Gender selection
- Department selection
- Semester selection
- Technical skills
- Address
- Terms agreement
- Form validation



1. HTML Form kya hota hai?
Form ka purpose user se information collect karna hota hai.

2. <label> aur id/for Relationship 3
Jab user label par click karega, browser related input ko focus kar sakta hai — accessibility ke liye important.

3.  <input>, type, placeholder, name, value, required, min, max, minlenght, maxlenght

4. action — Data kis URL/server endpoint par jayega.
method — Data kis HTTP method se submit hoga.

5. GET
Data URL/query parameters mein visible ho sakta hai: /search?query=html — search forms mein common.

6. POST
Data request body mein send hota hai — login/signup/create records ke liye common.
⚠️ POST akela sensitive data ko secure nahi banata — HTTPS aur server-side security bhi zaroori hai.

7. Form Accessibility 🔥
Rule 1: Har input ka label Rule 
2: label for = input id Rule 
3: placeholder ≠ label Rule 
4: required fields indicate karo Rule 
5: fieldset se group karo

8.  disabled vs readonly
1) Disabled
<input type="text" value="Pakistan" disabled>
User interact nahi kar sakta aur disabled control form submission mein include nahi hota.

2) Readonly
<input type="text" value="Pakistan" readonly>
User change nahi kar sakta, lekin value form submission ka part ho sakti hai.

9. autocomplete
<input type="email" name="email" autocomplete="email">
Name → autocomplete="name" Phone → autocomplete="tel" Address → autocomplete="street-address"

10. Form Test & Validation Concept
Test 1: Empty submit → required validation 
Test 2: "hello" as email → email validation fails 
Test 3: Age "10" → min="16" fails
Client-side validation useful hai, lekin security ke liye server-side validation bhi mandatory hoti hai.


























