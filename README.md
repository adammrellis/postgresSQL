# SQL Refference Sheet

## How to create a database

    -Make sure you have both HomeBrew and PostGreSQL

    -Install Postico

    -Open Postico and within postgres pull up SQL Query

    -Type CREATE DATABASE (whatever you want to name the database here)

    -Click Execute Statement and go back to localhost where the databases display

    -Refresh the page

    -Look into the documentation here if there are any questions

        https://www.codementor.io/engineerapart/getting-started-with-postgresql-on-mac-osx-are8jcopb

## How to create a table
    
    -Use the CREATE TABLE key words to create a table within the specific database
    -Example:
        ````            CREATE TABLE COMPANY(
                ID INT PRIMARY KEY     NOT NULL,
                NAME           TEXT    NOT NULL,
                AGE            INT     NOT NULL,
                ADDRESS        CHAR(50),
                SALARY         REAL
                ); ````
    -This would create a table called COMPANY
    -Look into this Documentation if you have any questions

        https://www.tutorialspoint.com/postgresql/index.htm


## How to get everything from a single table
    -Using the SELECT query followed by a * FROM (table name) would get all of hte information from said table
    -Example:
        ````            SELECT * FROM table_name; ````

## How to get one thing from a table using a "WHERE" clause
    -Using the WHERE clause helps state the condition you are updating/deleting/adding to/or getting exlusively
    -This example uses the SELECT and the WHERE clauses to get a specific thing within a table:
        ````            SELECT column1, column2, columnN
                    FROM table_name
                    WHERE [search_condition]; ````

## How to add something to a table 
    -You can use the INSERT INTO (what table you are inserting into) to add somthing into your table
    -Example:
            ````        INSERT INTO COMPANY (ID,NAME,AGE,ADDRESS,SALARY,JOIN_DATE)              VALUES (1, 'Paul', 32, 'California', 20000.00,'2001-07-13');````

## How to edit something inside of a table
    -Use the UPDATE query and the WHERE clause states the condition that you are updating.
    -Example:
        ````            UPDATE table_name
                SET column1 = value1, column2 = value2...., columnN = valueN
                WHERE [condition]; ````

## How to remove something from a table
    -Use the DELETE query, if you want to be specific on what you are deleting, use the WHERE clause again to specifically state what you are deleting. 