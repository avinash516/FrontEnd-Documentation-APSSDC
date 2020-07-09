## Part - I

![](RackMultipart20200628-4-mprj2k_html_237499165a11f2b9.gif)

### FMS vs DBMS vs noSql

The **key difference** between DBMS and File Management System is that **a DBMS stores data to the hard disk according to a structure while a file management system stores data to the hard disk without using a structure.**

**Advantages of DBMS:**

- High Security
- User Friendly nature
- Having a structure

**Disadvantages of DBMS:**

- Low performance

**Advantages of FMS**

- High Performance
- User friendly nature

**Disadvantages of FMS**

- Low security (Everyone can access it without any kind of authentication)

- **NoSql**

**NoSQL** databases (aka &quot;not only SQL&quot;) are non tabular, and store data differently than relational tables. NoSQL databases come in a variety of types based on their data model. The main types are document, **key-value** , **wide-column** , and **graph**. They provide flexible schemas and scale easily with large amounts of data and high user loads.

It covers the disadvantages of both DBMS and FMS

NoSql =\&gt; FMS + DBMS

**Advantages of NoSql**

- High performance
- High Security

- Installation procedure of XAMPP | Oracle

**Install XAMPP ( Linux )**

- For linux operating system, We&#39;ve to download the software from official website ([https://www.apachefriends.org/download.html](https://www.apachefriends.org/download.html))

Open Terminal and enter:

sudo tar xvfz xampp-linux-1.7.7.tar.gz -C /opt

(replace _xampp-linux-1.7.7.tar.gz_ with the version of xammp you downloaded). It has been reported that the MYSQL database of xampp 1.7.4 does not work with Joomla 1.5.22

This installs ... Apache2, mysql and php5 as well as an ftp server.

_sudo /opt/lampp/lampp start_

And

_sudo /opt/lampp/lampp stop_

**Install XAMPP in WINDOWS**

- For Windows operating system, We&#39;ve to download the software from official website ([https://www.apachefriends.org/download.html](https://www.apachefriends.org/download.html))
- We can install the software by double clicking on the downloaded software. And we have to follow a few steps according to steps.

**Starting with the SQL environment**

- PHPMyAdmin includes sql environment. It provides us to run sql queries
- By using URL ([http://localhost/phpmyadmin](http://localhost/phpmyadmin) ) from your favorite browser to visit the sql environment.

- Database ( Collection of tables )
  - CREATE DATABASE \&lt;database name\&gt;

Creating a database does not select it for use; you must do that explicitly. To make menagerie the current database, use this statement:

mysql\&gt;USE \&lt;database name\&gt;

- Tables

Creating the database is the easy part, but at this point it is empty, as [**SHOW TABLES**](https://dev.mysql.com/doc/refman/8.0/en/show-tables.html) tells you:

mysql\&gt;SHOWTABLES;

Empty set (0.00 sec)

**Syntax for creating table**

mysql\&gt;CREATETABLE \&lt;table\_name\&gt; (nameVARCHAR(20),emailVARCHAR(60),species VARCHAR(20), gender CHAR(1), birth DATE);

Getting list of Tables

mysql\&gt;SHOWTABLES;

+---------------------+

| Tables in menagerie |

+---------------------+

| \&lt;table\_name\&gt; |

+---------------------+

- Varchar vs varchar2
  - Varchar takes empty values too.
  - Varchar2 doesn&#39;t allow empty values or null values.

- Data Types

<img src="https://raw.githubusercontent.com/avinash516/FrontEnd-Documentation-APSSDC/master/images/image3.png" />

The following table shows the string data types in MySQL:

| **String Types** | **Description** |
| --- | --- |
| [CHAR](https://www.mysqltutorial.org/mysql-char-data-type/) | A fixed-length nonbinary (character) string |
| [VARCHAR](https://www.mysqltutorial.org/mysql-varchar/) | A variable-length non-binary string |
| BINARY | A fixed-length binary string |
| VARBINARY | A variable-length binary string |
| TINYBLOB | A very small BLOB (binary large object) |
| BLOB | A small BLOB |
| MEDIUMBLOB | A medium-sized BLOB |
| LONGBLOB | A large BLOB |
| [TINYTEXT](https://www.mysqltutorial.org/mysql-text/) | A very small non-binary string |
| [TEXT](https://www.mysqltutorial.org/mysql-text/) | A small non-binary string |
| [MEDIUMTEXT](https://www.mysqltutorial.org/mysql-text/) | A medium-sized non-binary string |
| [LONGTEXT](https://www.mysqltutorial.org/mysql-text/) | A large non-binary string |
| [ENUM](https://www.mysqltutorial.org/mysql-enum/) | An enumeration; each column value may be assigned one enumeration member |
| SET | A set; each column value may be assigned zero or more SET members |

The following table illustrates the MySQL date and time data types:

| **Date and Time Types** | **Description** |
| --- | --- |
| [DATE](https://www.mysqltutorial.org/mysql-date/) | A date value in CCYY-MM-DD format |
| [TIME](https://www.mysqltutorial.org/mysql-time/) | A time value in hh:mm:ss format |
| [DATETIME](https://www.mysqltutorial.org/mysql-datetime/) | A date and time value inCCYY-MM-DD hh:mm:ss format |
| [TIMESTAMP](https://www.mysqltutorial.org/mysql-timestamp.aspx) | A timestamp value in CCYY-MM-DD hh:mm:ss format |
| YEAR | A year value in CCYY or YY format |

## Part - II

![](RackMultipart20200628-4-mprj2k_html_237499165a11f2b9.gif)

Dropping

DROP DATABASE \&lt;database name\&gt; (Dropping a DataBase)

DROP TABLE \&lt;table name\&gt; (Dropping a Table)

**Inserting Data into Table**

mysql\&gt;INSERTINTO \&lt;table\_name\&gt;

VALUES(&#39;Hanuman Kumar&#39;,&#39;hanumankumar@gmail.com&#39;,&#39;hamster&#39;,&#39;m&#39;,&#39;1994-09-02&#39;);

- Operators :
  - Mathematical or Arithmetic
    - +, -, \*, /, %
  - Logical
    - AND
    - OR
    - NOT
  - Comparison Operators and
    - =, !=,\&lt;\&gt;,\&lt;,\&gt;,\&lt;=,\&gt;=, IN, NOT IN, BETWEEN, NOT BETWEEN, EXISTS, NOT EXITS, LIKE, NOT LIKE
  - Set Operators
    - UNION, UNION ALL, MINUS, INTERSECT

- Numerical Functions :
  - ABS(-1) = 1
  - CEIL
    - 123.456 =\&gt; 124
  - FLOOR
    - 123.456 =\&gt; 123

- LN
- MOD (10,3) =\&gt;1
- POWER(2,3) =\&gt; 8
- ROUND(1.2345)=\&gt;1
- SQRT(25) =\&gt; 5

**Aggregation :**

An aggregate function performs a calculation on multiple values and returns a single value.

For example, you can use the AVG() aggregate function that takes multiple numbers and returns the average value of the numbers.

- MAX()

The MySQL MAX() function returns the maximum value in a set of values. The MAX() function comes in handy in many cases such as finding the greatest number, the most expensive product, and the largest payment from customers.

SELECT MAX(\&lt;column name\&gt;) FROM \&lt;table name\&gt;

- MIN()

The MIN() function returns the minimum value in a set of values. The MIN() function is very useful in some scenarios such as finding the smallest number, selecting the least expensive product, or getting the lowest credit limit.

SELECT MIN(\&lt;column name\&gt;) FROM \&lt;table name\&gt;

- SUM()

The SUM() function is an [aggregate function](https://www.mysqltutorial.org/mysql-aggregate-functions.aspx) that allows you to calculate the sum of values in a set.

SELECT SUM(\&lt;column name\&gt;) FROM \&lt;table name\&gt;

- COUNT

The COUNT() function is an [aggregate function](https://www.mysqltutorial.org/mysql-aggregate-functions.aspx) that returns the number of rows in a table. The COUNT() function allows you to count all rows or only rows that match a specified condition.

The COUNT() function has three forms: COUNT(\*), COUNT(expression) and COUNT(DISTINCT expression).

### **COUNT(\*) function**

The COUNT(\*) function returns the number of rows in a result set returned by a [SELECT](https://www.mysqltutorial.org/mysql-select-statement-query-data.aspx) statement. The COUNT(\*) returns the number of rows including duplicate, non-NULL and NULL rows.

### **COUNT(expression)**

The COUNT(expression) returns the number of rows that do not contain NULL values as the result of the expression.

### **COUNT(DISTINCT expression)**

The COUNT(DISTINCT expression) returns the number of distinct rows that do not contain NULL values as the result of the expression.

The return type of the COUNT() function is [BIGINT](https://www.mysqltutorial.org/mysql-int/). The COUNT() function returns 0 if there is no matching row found.

SELECT COUNT(\*) FROM \&lt;table name\&gt;

SELECT COUNT(\&lt;column name\&gt;) FROM \&lt;table name\&gt;

MySQL supports the following aggregate functions:

| **Aggregate function** | **Description** |
| --- | --- |
| [AVG()](https://www.mysqltutorial.org/mysql-avg/) | Return the average of non-NULL values. |
| BIT\_AND() | Return bitwise AND. |
| BIT\_OR() | Return bitwise OR. |
| BIT\_XOR() | Return bitwise XOR. |
| [COUNT()](https://www.mysqltutorial.org/mysql-count/) | Return the number of rows in a group, including rows with NULL values. |
| [GROUP\_CONCAT()](https://www.mysqltutorial.org/mysql-group_concat/) | Return a concatenated string. |
| JSON\_ARRAYAGG() | Return result set as a single JSON array. |
| JSON\_OBJECTAGG() | Return result set as a single JSON object. |
| [MAX()](https://www.mysqltutorial.org/mysql-max-function/) | Return the highest value (maximum) in a set of non-NULL values. |
| [MIN()](https://www.mysqltutorial.org/mysql-min/) | Return the lowest value (minimum) in a set of non-NULL values. |
| [STDEV()](https://www.mysqltutorial.org/mysql-standard-deviation/) | Return the population standard deviation. |
| STDDEV\_POP() | Return the population standard deviation. |
| STDDEV\_SAMP() | Return the sample standard deviation. |
| [SUM()](https://www.mysqltutorial.org/mysql-sum/) | Return the summation of all non-NULL values a set. |
| VAR\_POP() | Return the population standard variance. |
| VARP\_SAM() | Return the sample variance. |
| VARIANCE() | Return the population standard variance. |

## Part - III

![](RackMultipart20200628-4-mprj2k_html_237499165a11f2b9.gif)

Sql Commands

- Data Definition Language
- The commands are reflects the structure of the table
  - CREATE
  - DROP
  - ALTER
    - Syntax : ALTER TABLE employee RENAME COLUMN name TO names (Oracle)
    - Syntax : ALTER TABLE employee CHANGE \&lt;old column name\&gt; \&lt;new column name along with datatype \&gt; (mySql)
    - Deleting the column : ALTER TABLE \&lt;table name\&gt; DROP COLUMN \&lt;column-name\&gt;
    - ALTER TABLE \&lt;table\_name\&gt; ADD \&lt;column-name\&gt; \&lt;data\_type with size\&gt;

## Part - IV

![](RackMultipart20200628-4-mprj2k_html_237499165a11f2b9.gif)

  - RENAME : RENAME TABLE \&lt;old table name\&gt; TO \&lt;new table name\&gt;
  - TRUNCATE
    - Syntax: TRUNCATE TABLE employees
- Data Manipulation Language (DML):
  - INSERT
  - DELETE
    - Syntax : DELETE FROM \&lt;table\_name\&gt; WHERE (clause) \&lt;condition\&gt;
    - Example:
      - [DELETE](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/delete.html)FROM employees WHERE id=1
  - UPDATE
    - Syntax : UPDATE employees SET \&lt;column\_name\&gt;=\&lt;value\&gt; WHERE \&lt;column\_name\&gt;=\&lt;value\&gt;
    - Example:
      - [UPDATE](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/update.html) employees [SET](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/set.html) name=&#39;Ranga&#39;WHERE id=1
      - [UPDATE](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/update.html) employees [SET](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/set.html) name=&quot;Poojitha&quot;WHERE id=1[AND](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/logical-operators.html#operator_and) name=&quot;Ranga&quot;

Auto Increment:

1 .The column must be initialized with any kind of key constraints

SYntax: ALTER TABLE \&lt;table\_name\&gt; ADD PRIMARY KEY (\&lt;column\_name\&gt;)

2. The column value should not be empty

Syntax :

ALTER TABLE \&lt;table\_name\&gt; MODIFY \&lt;column\_name\&gt; \&lt;datatype with length\&gt; NOT NULL AUTO\_INCEREMT

Example:

[ALTER](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/alter-table.html)[TABLE](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/alter-table.html) employees MODIFY id integer(20) [NOT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/logical-operators.html#operator_not)NULLAUTO\_INCREMENT

\*\* Constraints:

These are the rules for enforcing on specific field ( columns )

- NOT NULL
- DEFAULT
- PRIMARY KEY
  - 1. 1 table can have only one primary key
  - 2. The value should not be empty
  - 3. Won&#39;t allow duplicate values
- UNIQUE KEY
- FORIEGN KEY

## Part - V

![](RackMultipart20200628-4-mprj2k_html_237499165a11f2b9.gif)

- DCL (Data Control Language)
  - GRANT
    - Granting Permissions to specific user.
  - REVOKE
    - Withdrawing the permissions which were given using GRANT command.
- TCL (Transaction Control Language)
  - COMMIT
  - ROLLBACK
  - SAVEPOINT

LIKE clause:

The LIKE operator is a logical operator that tests whether a string contains a specified pattern or not.

The LIKE operator is used in the [WHERE](https://www.mysqltutorial.org/mysql-where/) clause of the [SELECT](https://www.mysqltutorial.org/mysql-select-statement-query-data.aspx) , [DELETE](https://www.mysqltutorial.org/mysql-delete-statement.aspx), and [UPDATE](https://www.mysqltutorial.org/mysql-update-data.aspx) statements to filter data based on patterns.

MySQL provides two wildcard characters for constructing patterns: percentage % and underscore \_ .

- The percentage ( % ) wildcard matches any string of zero or more characters.
- The underscore ( \_ ) wildcard matches any single character.

For example, s% matches any string starts with the character s such as sun and six. The se\_ matches any string starts with se and is followed by any character such as see and sea

Example :

[SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html) \* FROM employees WHERE name [LIKE](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/string-comparison-functions.html#operator_like)&#39;K%&#39; ( Retrieving data where name starts with character &#39; **K**&#39; )

SELECT \* FROM employees WHERE name [LIKE](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/string-comparison-functions.html#operator_like)&#39;%a%&#39; ( Retrieving data where name contains character &#39; **a**&#39; )

## Part - VI

![](RackMultipart20200628-4-mprj2k_html_237499165a11f2b9.gif)

Relationships

### One-to-one

One-to-one relationships occur when there is exactly one record in the first table that corresponds to exactly one record in the related table.

MySQL does not contains any &quot;ready&quot; options to define the one-to-one relationship, but, if you want to enforce it, you can add a foreign key from one primary key to the other primary key, by doing this, both tables will have the one-to-one relationship automatically.

Here&#39;s an example to define a one-to-one relationship in MySQL.

![](RackMultipart20200628-4-mprj2k_html_4bb9c908ec000532.jpg)

### One-to-many

`CREATE VIEW viewAreas AS  SELECT * FROM Areas, Maps WHERE  Areas.ID = Maps.AreaID;`

### Many-to-many

A _many-to-many relationship_ occurs when multiple [records](https://fmhelp.filemaker.com/help/18/fmp/en/FMP_Help/glossary.html#ww1028030) in a [table](https://fmhelp.filemaker.com/help/18/fmp/en/FMP_Help/glossary.html#ww1045562) are associated with multiple records in another table. For example, a many-to-many relationship exists between customers and products: customers can purchase various products, and products can be purchased by many customers.

The following example includes a Students table, which contains a record for each student, and a Classes table, which contains a record for each class. A join table, Enrollments, creates two one-to-many relationships—one between each of the two tables.

<img src="https://raw.githubusercontent.com/avinash516/FrontEnd-Documentation-APSSDC/master/images/image6.png" />

The primary key Student ID uniquely identifies each student in the Students table. The primary key Class ID uniquely identifies each class in the Classes table. The Enrollments table contains the foreign keys Student ID and Class ID.

Example

Table 1: (Primary Key)

- The values should be unique
- One table can have only one primary key
- Primary key doesn&#39;t allow any NULL values.

USE apssdc;

CREATE TABLE employees (

id int(20) AUTO\_INCREMENT,

name varchar(30),

email varchar(70),

PRIMARY KEY(id))

Table2 : (Foriegn Key)

[CREATE](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/create-table.html)[TABLE](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/create-table.html) salaries(

id [int](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/numeric-types.html)(20) [NOT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/logical-operators.html#operator_not)NULL,

salary [int](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/numeric-types.html)(20),

FOREIGNKEY(id) REFERENCES employees(id)

)

Example :

Students

Roll name email

2 ccc ccc@gmail.com

Marks

Roll marks

2 40

#### ON DELETE cascade: (REFERENTIAL INTEGRITY)

[CREATE](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/create-table.html)[TABLE](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/create-table.html) salaries(

id [int](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/numeric-types.html)(20), salary [int](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/numeric-types.html)(30),

FOREIGNKEY(id) REFERENCES employees(id) ON[DELETE](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/delete.html)CASCADE )

UNIQUE KEY

- Same as primary key (Doesn&#39;t allow duplicate values)
- We can specify multiple unique attributes for a single table.

## Part - VII

![](RackMultipart20200628-4-mprj2k_html_237499165a11f2b9.gif)

Joins in SQL

A relational database consists of multiple related tables linking together using common columns which are known as [foreign key](http://www.mysqltutorial.org/mysql-foreign-key/) columns. Because of this, data in each table is incomplete from the business perspective.

For example, in the [sample database](http://www.mysqltutorial.org/mysql-sample-database.aspx), we have the orders and orderdetails tables that are linked using the orderNumber column:

<img src="https://raw.githubusercontent.com/avinash516/FrontEnd-Documentation-APSSDC/master/images/image5.png" />

To get complete orders&#39; information, you need to query data from both orders and orderdetails tables.

Thats why joins come into the play.

A join is a method of linking data between one ([self-join](http://www.mysqltutorial.org/mysql-self-join/)) or more tables based on values of the common column between the tables.

MySQL supports the following types of joins:

1. [Inner join](https://www.mysqltutorial.org/mysql-inner-join.aspx)
2. [Left join](https://www.mysqltutorial.org/mysql-left-join.aspx)
3. [Right join](https://www.mysqltutorial.org/mysql-right-join/)
4. Full[join](https://www.mysqltutorial.org/mysql-cross-join/)

To join tables, you use the cross join, inner join, left join, or right join clause for the corresponding type of join. The join clause is used in the [SELECT](http://www.mysqltutorial.org/mysql-select-statement-query-data.aspx) statement appeared after the FROM clause.

### Inner Join

The [inner join](https://www.mysqltutorial.org/mysql-inner-join.aspx) clause joins two tables based on a condition which is known as a join predicate.

The inner join clause compares each row from the first table with every row from the second table. If values in both rows cause the join condition evaluates to true, the inner join clause creates a new row whose column contains all columns of the two rows from both tables and include this new row in the final result set. In other words, the inner join clause includes only rows whose values match.

  - For getting common values between two tables
  - Example:

[SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html)

employee.id,

employee.name,

salaries.salary,

employee.addressFROM employee

INNERJOIN salaries ON employee.id=salaries.id

The following Venn diagram illustrates the inner join:

<img src="https://raw.githubusercontent.com/avinash516/FrontEnd-Documentation-APSSDC/master/images/image1.png" />

### Left Join

Similar to an inner join, a [left join](https://www.mysqltutorial.org/mysql-left-join.aspx) also requires a join-predicate. When two tables using a left join, the concepts of left and right tables are introduced.

The left join selects data starting from the left table. For each row in the left table, the left join compares with every row in the right table. If the values in the two rows cause the join condition evaluates to true, the left join creates a new row whose columns contain all columns of the rows in both tables and includes this row in the result set.

If the values in the two rows are not matched, the left join clause still creates a new row whose columns contain columns of the row in the left table and NULL for columns of the row in the right table.

In other words, the left join selects all data from the left table whether there are matching rows exist in the right table or not. In case there is no matching rows from the right table found, NULLs are used for columns of the row from the right table in the final result set.

  - It returns data from left table even the data is not available in right table
  - Example :

[SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html)

employee.name,

Salaries.salary,

employee.addressFROM employee

[LEFT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/string-functions.html#function_left)JOIN salaries ON employee.id=salaries.id

This Venn diagram illustrates how to use the left join to select rows that only exist in the left table:

<img src="https://raw.githubusercontent.com/avinash516/FrontEnd-Documentation-APSSDC/master/images/image4.png" />

### Right Join

The [right join](https://www.mysqltutorial.org/mysql-right-join/) clause is similar to the left join clause except that the treatment of tables is reversed. The right join starts selecting data from the right table instead of the left table.

The right join clause selects all rows from the right table and matches rows in the left table. If a row from the right table does not have matching rows from the left table, the column of the left table will have NULL in the final result set.

  - It returns data from right table even the data is not available in left table
  - Example :

[SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html) employee.name,

Salaries.salary,

employee.addressFROM employee

[RIGHT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/string-functions.html#function_right)JOIN salaries ON employee.id=salaries.id

This Venn diagram illustrates how to use the right join to select data that exists only in the right table:

<img src="https://raw.githubusercontent.com/avinash516/FrontEnd-Documentation-APSSDC/master/images/image2.png" />

### Full join

Unlike the inner join, left join, and right join, the [cross join](https://www.mysqltutorial.org/mysql-cross-join/) clause does not have a join condition. The right join makes a Cartesian product of rows from the joined tables. The cross join combines each row from the first table with every row from the right table to make the result set.

Suppose the first table has n rows and the second table has m rows. The cross join that joins the first with the second table will return nxm rows.

  - Left Join + Right Join
  - The result will contain all records from both tables, and fill in Null for missing matches.
  - Example :

[SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html) employee.name,

salaries.salary,

employee.addressFROM employee

[RIGHT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/string-functions.html#function_right)JOIN salaries ON employee.id=salaries.id

UNION

[SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html) employee.name,

salaries.salary, employee.addressFROM employee

[LEFT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/string-functions.html#function_left)JOIN salaries ON employee.id=salaries.id

- Storing Resulting data after applying different kinds of Joins
  - Example:

[CREATE](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/create-table.html)[TABLE](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/create-table.html) result AS

[SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html) employee.name,

salaries.salary,

employee.addressFROM employee

[LEFT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/string-functions.html#function_left)JOIN salaries ON employee.id=salaries.id

Importance of HAVING clause

- Selecting data from a table by filtering based on condition

## Part - VIII

![](RackMultipart20200628-4-mprj2k_html_237499165a11f2b9.gif)

Clauses in SQL :

- HAVING

The HAVING clause is used in the [SELECT](https://www.mysqltutorial.org/mysql-select-statement-query-data.aspx) statement to specify filter conditions for a group of rows or aggregates.

The HAVING clause is often used with the [GROUP BY](https://www.mysqltutorial.org/mysql-group-by.aspx) clause to filter groups based on a specified condition. If the GROUP BY clause is omitted, the HAVING clause behaves like the [WHERE](https://www.mysqltutorial.org/mysql-where/) clause.

SELECT product, SUM(quantity) AS &quot;Total quantity&quot; FROM order\_details GROUP BY product HAVING SUM(quantity) \&gt; 10;

- GROUP BY
  - We can get data from multiple records and make them into one column.
  - Example :

1.[SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html) name,[COUNT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/group-by-functions.html#function_count)(address) FROM employee GROUPBY address

2.[SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html) name,[SUM](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/group-by-functions.html#function_sum)(marks) AS Total\_marks FROM marks GROUPBY name

3.[SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html) name,[MAX](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/group-by-functions.html#function_max)(marks) AS Total\_marks FROM marks GROUPBY name

- ORDER BY
  - To sort the data (ascending order, descending order)
  - ASC - Ascending Order
  - DESC - Descending Order

Example :

1. [SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html) name,address FROM employee ORDERBY name ASC
2. [SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html) name,address FROM employee ORDERBY name DESC

Note : By Default we retrieve information in ascending order by using ORDER BY.

- WHERE
- SELECT
- FROM
- DISTINCT
  - For getting unique values from the table
  - Example :

[SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html)DISTINCT(id),salary FROM salaries

Relationships:

- One - one
- One - Many
  - Relationship between one field in one table and many fields in another table
  - Example :

[SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html) E.name,M.subject,M.marksFROM employee E [RIGHT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/string-functions.html#function_right)JOIN marks M ON E.name=M.name

- Many - One
  - Example :

[SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html) E.name,E.address,[SUM](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/group-by-functions.html#function_sum)(M.marks) AS Total\_marks FROM employee E INNERJOIN marks M ON E.name=M.nameGROUPBY E.name

2.[SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html) E.name, M.subject,M.marks,S.salaryFROM employee E, marks M,salaries S WHERE E.id=M.id[and](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/logical-operators.html#operator_and) E.id=S.id

## Part - IX

![](RackMultipart20200628-4-mprj2k_html_237499165a11f2b9.gif)

LIMIT :

[SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html) \* FROM employee LIMIT3

Example 2:

[SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html) \* FROM employee ORDERBY id DESCLIMIT3

Example 3:

[SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html) \* FROM([SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html) \* FROM employee ORDERBY id DESCLIMIT3) employee ORDERBY id ASC

**Wildcards :**

**%**

R **% =\&gt;** The value must be starts with &#39;R&#39;

%R =\&gt; The value must be ends with &#39;R&#39;

%R% =\&gt; The value needs to have the character of &#39;R&#39;.

**\_**

Matching the positional values.

Example :

[SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html) \* FROM`employee`WHERE name [LIKE](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/string-comparison-functions.html#operator_like)&#39;\_a%&#39;

[SELECT](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/select.html) \* FROM`employee`WHERE name [LIKE](http://localhost/phpmyadmin/url.php?url=https://dev.mysql.com/doc/refman/5.5/en/string-comparison-functions.html#operator_like)&#39;\_%a&#39; (Matching at last character)

[]

This is used for matching any character in the given structure

&#39;[abc]%&#39; =\&gt; The value must be starts with &#39;a&#39; or &#39;b&#39; or &#39;c&#39;

&#39;[!abc]%&#39; =\&gt; The string should not start with &#39;a&#39; or &#39;b&#39; or &#39;c&#39;.

&#39;[a-z]%&#39; =\&gt; The string should start with any kind of alphabet.

**VIEWS :**

This is a virtual table we can store the value by getting those from an expression

Example :

CREATEVIEW data ASSELECT name FROM employee;

The manipulating commands are similar to the commands in table.

Normalization :

We can break the complex table into pieces (Normalization)

1. Reducing redundancy of Data
2. Data integrity (Primary Key, Forien Key)
  1. Problems without normalization
    1. Insertion anomaly
    2. Update anomaly
    3. Deletion anomaly

Kinds of Normal forms:

- 1NF =\&gt;Need to avoid multiple values in a cell. A Single cell can&#39;t hold multiple values.
- 2NF =\&gt;
  - Must be satisfied 1st Normal form
  - Have to create multiple tables for assigning primary keys efficiently

- 3NF =\&gt;
  - Must be satisfied with the 2nd NF.
  - Non - primary key value should not be depend upon a non-primary key value

- BCNF =\&gt; ([Boyce–Codd normal form](https://en.wikipedia.org/wiki/Boyce%E2%80%93Codd_normal_form))
  - Must be satisfied with 3NF
    - Student name and subject
    - Teacher and subject
  -

      - Student and Professor in one table
      - Subjects in another table

**Transaction management** :

**A** tomicity

**C** onsistency

**I** solation

**D** urability

A transaction is a very small unit of a program and it may contain several lowlevel tasks. A transaction in a database system must maintain Atomicity, Consistency, Isolation, and Durability − commonly known as ACID properties − in order to ensure accuracy, completeness, and data integrity.

- **Atomicity** − This property states that a transaction must be treated as an atomic unit, that is, either all of its operations are executed or none. There must be no state in a database where a transaction is left partially completed. States should be defined either before the execution of the transaction or after the execution/abortion/failure of the transaction.

- **Consistency** − The database must remain in a consistent state after any transaction. No transaction should have any adverse effect on the data residing in the database. If the database was in a consistent state before the execution of a transaction, it must remain consistent after the execution of the transaction as well.

- **Durability** − The database should be durable enough to hold all its latest updates even if the system fails or restarts. If a transaction updates a chunk of data in a database and commits, then the database will hold the modified data. If a transaction commits but the system fails before the data could be written on to the disk, then that data will be updated once the system springs back into action.

- **Isolation** − In a database system where more than one transaction are being executed simultaneously and in parallel, the property of isolation states that all the transactions will be carried out and executed as if it is the only transaction in the system. No transaction will affect the existence of any other transaction.
