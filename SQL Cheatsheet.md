<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>SQL Cheatsheet</title>
  <link rel="stylesheet" href="https://stackedit.io/style.css" />
</head>

<body class="stackedit">
  <div class="stackedit__left">
    <div class="stackedit__toc">
      
<ul>
<li><a href="#sql-cheatsheet">SQL Cheatsheet</a>
<ul>
<li><a href="#sql-keywords">SQL Keywords</a></li>
<li><a href="#databases-notes">Databases Notes</a></li>
</ul>
</li>
</ul>

    </div>
  </div>
  <div class="stackedit__right">
    <div class="stackedit__html">
      <h1 id="sql-cheatsheet">SQL Cheatsheet</h1>
<p>Gosh is Markdown so much better; I might start doing all my notes this way.<br>
Written with <a href="https://stackedit.io/">StackEdit</a>.</p>
<h2 id="sql-keywords">SQL Keywords</h2>
<h3 id="select">Select</h3>
<p><code>SELECT column1, column2… FROM table1</code><br>
<code>SELECT * FROM table1</code></p>
<h3 id="select-distinct">Select Distinct</h3>
<p>Only shows unique values</p>
<p><code>SELECT DISTINCT column1, column2… FROM table1</code></p>
<p><code>SELECT COUNT(DISTINCT column1) FROM table1</code></p>
<h3 id="where">Where</h3>
<p><code>SELECT column1 FROM table1 WHERE conditional1</code></p>
<p>Ex:<br>
<code>SELECT * FROM table1 WHERE column1='something'</code><br>
<code>SELECT * FROM table1 WHERE column1 BETWEEN 0 AND 60</code><br>
<code>SELECT * FROM table1 WHERE column1 IN ('One Value', 'Another Value')</code><br>
<code>SELECT * FROM table1 WHERE column1 LIKE '%s'</code> (patterns)</p>
<p>You can use <code>=</code>, <code>&lt;</code>, <code>&gt;</code>, <code>&gt;=</code>, <code>&lt;=</code>, <code>!=</code> too.</p>
<h3 id="and-or-and-not">And, Or and Not</h3>
<p><code>SELECT * FROM table1 WHERE conditional1 AND conditional2 AND ...</code><br>
<code>SELECT * FROM table1 WHERE conditional1 OR conditional2 OR...</code><br>
<code>SELECT * FROM table1 WHERE NOT conditional1</code></p>
<h3 id="order-by">Order By</h3>
<p><code>SELECT column1, column2 ... FROM table1 ORDER BY column1, column2 ... ASC|DESC</code></p>
<h3 id="insert-into">Insert Into</h3>
<p><code>INSERT INTO table1 (column1, column2, ...) VALUES (value1, value2, ...)</code></p>
<h3 id="is-null-and-is-not-null">Is Null and Is Not Null</h3>
<p><code>SELECT column1, column2... FROM table1 WHERE column1 IS NULL</code><br>
<code>SELECT column1, column2... FROM table1 WHERE column1 IS NOT NULL</code></p>
<h3 id="update">Update</h3>
<p><code>UPDATE table1 SET column1 = value1, column2 = value2, ... WHERE conditional1</code></p>
<h3 id="delete">Delete</h3>
<p><code>DELETE FROM table1 WHERE conditional1</code></p>
<h3 id="top-and-limit">Top and Limit</h3>
<p>SQL Server / MS Access Syntax:<br>
`SELECT TOP</p>
<h2 id="databases-notes">Databases Notes</h2>
<h3 id="relational-database-management-system-rdbms">Relational Database Management System (RDBMS)</h3>
<p><strong>Record</strong> = <strong>Entry</strong> = <strong>Row</strong><br>
<strong>Unique Key</strong>: Each value must be unique<br>
<strong>Primary Key</strong>: Key that doesn’t have null values<br>
<strong>Foreign Key</strong>: Entry in one table that serves as a primary key in another</p>
<h3 id="normalizing-data">Normalizing Data</h3>
<p><strong>First Normal Form</strong>: Each entry should only have one piece of data in it<br>
<strong>Second Normal Form</strong>: Each field in a row should be fully dependent on a single key<br>
<strong>Third Normal Form</strong>: all data in non-key columns should be independent of each other</p>

    </div>
  </div>
</body>

</html>
