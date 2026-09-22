Q1: Table hoti kya hai?
Table ka use structured / tabular data show karne ke liye hota hai. Example --> Student Result
1. Real-world examples
University Results, Course Schedules, Invoices, Order Details, Employee Records, Product Comparison, Admin Dashboards, Reports, Financial Data

⚠ Important: Table ko website ka overall layout banane ke liye use nahi karna chahiye. Tables sirf data ke liye hain. Layout ke liye baad mein CSS Flexbox /
Grid use karenge.


Q2:  Basic <table>
Sabse basic table:
<table>
<tr>
<td>Wasif</td>
<td>Software Engineering</td>
</tr>
<tr>
<td>Ali</td>
<td>Computer Science</td>
</tr>
</table>
<table> — poori table. <tr> — Table Row. <td> — Table Data.

1. <tr> — Table Row  // Jitni row chahhyeh utny tr hongy aik table m.
2. <td> — Table Data  // td ka matlab Table Data — table ka normal cell.
3. <th> — Table Header  // Headings (Student | Marks | Grade) ke liye <th> use hota hai:
4. <caption>  // Table ka title dene ke liye <caption> use hota hai — accessibility aur samajhne dono ke liye useful.
5. What is thead, tbody, tfoot 

Q3: colspan
colspan ka matlab: ek cell multiple columns occupy kare.

Q4: rowspan
rowspan ka matlab: ek cell multiple rows occupy kare.

Q5: scope — Accessibility
Column header: <th scope="col">Name</th> | Row header: <th scope="row">Wasif</th>
Ye screen readers ke liye table relationships ko clearer banata hai.



Q2. What is <tr>?
Table Row.
Q3. What is <td>?
Table Data cell.
Q4. What is <th>?
Table Header cell.
Q5. Difference between <thead> and <tbody>?
thead header information rakhta hai, tbody main table data rakhta hai.
Q6. What is colspan?
Ek cell ko multiple columns span karne deta hai.
Q7. What is rowspan?
Ek cell ko multiple rows span karne deta hai.
Q8. Why is <caption> used?
Table ka title / description provide karne ke liye.
Q9. Why is scope useful?
Headers aur related data cells ka relationship clear karta hai — accessibility ke liye.


 Quick MCQs
1. HTML table row ke liye kya use hota hai?
A) <row>
B) <tr> ✅
C) <td>
D) <table-row>
2. Table header ke liye?
A) <head>
B) <header>
C) <th> ✅
D) <thead>
3. Multiple columns merge karne ke liye?
A) rowspan
B) merge
C) colspan ✅
D) columnspan
4. Multiple rows merge karne ke liye?
A) rowspan ✅
B) colspan
C) rows
D) merge-row
5. Main table data usually kis element mein hota hai?
A) <main>
B) <tbody> ✅
C) <data>
D) <content>



















