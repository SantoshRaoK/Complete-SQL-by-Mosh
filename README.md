<h2>Complete-SQL-by-Mosh</h2>
<ul>
<li>
    <a href="#date-from-a-single-table">Retrieving Data From a Single Table</a>
    <ol>
        <li>
            <a href="#data-in-customer-table">Data in <b>customer</b> table</a>
        </li>
        <li>
            <a href="#the-slect-statement">The Select Statement</a>
        </li>
        <li>
            <a href="#select-cluse-details">The Select Clause</a>
        </li>
        <li>
            <a href="#">The Where Clause</a>
        </li>              
        <li>
            <a href="#">The AND OR and NOT Operators</a>
        </li>
    </ol>
</li>
<li>
    <a href="#date-from-a-multiple-table">Retrieving Data From Multiple Tables</a>
</li>
<li>
    <a href="#insert-update-delet-date">Inserting, Updating, and Deleting Data</a>
</li>
<li>
    <a href="#summarizing-data">Summarizing Data</a>
</li>
<li>
    <a href="#write-complex-query">Writing Complex Query</a>
</li>
<li>
    <a href="#essential-mysql-function">Essential MySQL Functions</a>
</li>
<li>
    <a href="#mysql-views">Views</a>
</li>
<li>
    <a href="#stored-procedures">Stored Procedures</a> 
</li>
<li>
    <a href="#trigger-and-events">Triggers and Events</a>
</li>
<li>
    <a href="#transactions-and-concurrency">Transactions and Concurrency</a>
</li>
<li>
    <a href="#mysql-data-type">Data Type</a>
</li>
<li>
    <a href="#mysql-designing-database">Designing Databases</a>
</li>
<li>
    <a href="#indexing-for-high-performance">Indexing for High Performance</a>
</li>
<li>
    <a href="#mysql-securing-databases">Securing Databases</a>
</li>
</ul>
<!--Details about "Data From a Single Start" -->
    <h2 id="date-from-a-single-table">Retrieving Data From a Single Table</h2>
    <!--Data in customer table-->
    <h3 id="data-in-customer-table">1) Data in customer table</h3>
    <img src="git-html/images/customer_table.png" title="All data in customer table"> 
    <h3>SQL script</h3>
    <!--##########################################################################################-->
    <!--Select all data from customers table-->
    <h3 id="the-slect-statement">2) Select all data from customers table</h3>
    <pre>
        <code>
            SELECT * FROM customers;
        </code>
    </pre>     
    <hr />    
    <h3>Select a specefic element</h3>
    <pre>
        <code>
            SELECT * FROM customers WHERE last_name = 'MacCaffrey';
        </code>
    </pre>
    <!--##########################################################################################-->
    <hr /> 
    <!--The SELECT cluse in Details-->
    <h3 id="select-cluse-details">3) The SELECT cluse in Details</h3>
    <p>
        The "SELECT *" returns all the columns present in a table. If our table contains a large number of records it may 
        create a  negative impact in the database server and the network also. We can also select a specefic number of column 
        based on our requirement. 
    <p/>
    <h3>Select specfic column<h3/>
    <pre>
        <code>
            SELECT first_name, last_name, points FROM customers;
        </code>
    </pre>
    <hr />
    <!--Select all data from customers table-->
    <h3>SELECT a column and apply matmatical calculation on it</h3>
    <pre>
        <code>
            SELECT 
                first_name, 
                last_name, 
                points, 
                points + 100 AS 'points with discount' 
            FROM customers;
        </code>
    </pre>     
    <hr />    
    <h3>Select a specefic element</h3>
    <pre>
        <code>
            SELECT * FROM customers WHERE last_name = 'MacCaffrey';
        </code>
    </pre>
    <hr />    
    <h3>Short table data</h3>
    <pre>
        <code>
            SELECT * FROM customers WHERE birth_date < '1990-01-01' ORDER BY city;
        </code>
    </pre>     
    <hr />
    <!--Details about "Data From a Single END" -->
    <hr />
    
<h2 id="date-from-a-multiple-table">Retrieving Data From Multiple Tables</h2>
<h2 id="insert-update-delet-date">Inserting, Updating, and Deleting Data</h2>
<h2 id="summarizing-data">Summarizing Data</h2>
<h2 id="write-complex-query">Writing Complex Query</h2>
<h2 id="essential-mysql-function">Essential MySQL Functions</h2>
<h2 id="mysql-views">Views</h2>
<h2 id="stored-procedures">Stored Procedures</h2>
<h2 id="trigger-and-events">Triggers and Events</h2>
<h2 id="transactions-and-concurrency">Transactions and Concurrency</h2>
<h2 id="mysql-data-type">Data Type</h2>
<h2 id="mysql-designing-database">Designing Databases</h2>
<h2 id="indexing-for-high-performance">Indexing for High Performance</h2>
<h2 id="mysql-securing-databases">Securing Databases</h2>
