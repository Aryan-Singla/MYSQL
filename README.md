ALL These Commands run in the cmd

cd path - will enter in the mysql folder

mysql -u root -p  - will start the mysql

show databases; - will show the databases

create database aryandb; - will create the databases

use aryandb - will change the database to the aryandb2

To create the table employee with the following coloumns ->

CREATE TABLE EMPLOYEE(
EMPID int,
FirstName varchar(255),
LastName varchar(255),
EMPAGE int,
EMPZONE varchar(255)
);

DESC EMPLOYEE -> will show the formed table

TO ENTER THE VALUES IN THE EMPLOYEE TABLE ->

INSERT INTO EMPLOYEE(EMPID, FirstName, LastName, EMPAGE, EMPZONE) VALUES(1, 'TOM', 'STEPHEN', 50, 'WEST'); -> we enter the any umber of the rows by just changing the values

SELECT * FROM EMPOLOYEE; -> WILL SHOW THE EMPLOYEE TABLE
  
SELECT EMPID FROM EMPLOYEE -> THIS WILL SELECT THE EMPID COLOUMN


CONSTRAINTS -> Here is age constraint so it will no enter the age if less than the 20

CREATE TABLE EMPLOYE(
EMPID int,
FIRSTNAME varchar(255),
LASTNAME varchar(255),
EMPAGE int,
CHECK (EMPAGE>20)
);


DEFAULT CONSTRAINTS ->

CREATE TABLE NEW(
    -> EMPID int NOT NULL,
    -> FIRSTNAME varchar(255),
    -> LASTNAME varchar(255),
    -> EMPDEPT varchar(255) DEFAULT 'Operations'
    -> );

INSERT INTO NEW(EMPID, FIRSTNAME, LASTNAME)
    -> VALUES(1, 'EMMA', 'WATSON');
SELECT * FROM NEW

After that we can check the table by SELECT * FROM NEW and it shows the EMPDEPT with DEFAULT Operations


INDEX CONSTRAINTS -> ENTRY IS TABLE HERE.


INDEX 1 -> DEMOINDEX CREATED ON THE EMPID  
 CREATE INDEX DEMOINDEX
 -> ON ENTRY(EMPID);


INDEX2 -> DEMOINDEX2 CREATED ON THE FIRSTNAME
CREATE INDEX DEMOINDEX2
-> ON ENTRY(FIRSTNAME)


TO GET INDEXES -> SHOW INDEXES FROM ENTRY


TO DELETE THE INDEXES -> DROP INDEX DEMOINDEX1 ON ENTRY


ALTER THE TABLE ->

ADD THE COLOUM IN THE ENTRY TABLE ->

ALTER TABLE ENTRY
-> ADD EMPLOC varchar(255);


DELETE THE COLOUM IN THE ENTRY TABLE ->

ALTER TABLE ENTRY
-> DROP COLUMN EMPLOC; 



