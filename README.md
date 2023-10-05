# Ex. No: 4 Creating Procedures using PL/SQL

### AIM: To create a procedure using PL/SQL.

### Steps:
1. Create employee table with following attributes (empid NUMBER, empname VARCHAR(10), dept VARCHAR(10),salary NUMBER);
2. Create a procedure named as insert_employee data.
3. Inside the procdure block, write the query for inserting the values into the employee table.
4. End the procedure.
5. Call the insert_employee data procedure to insert the values into the employee table.
6. Display the employee table

### Program:
```
Developed by:Kavinesh M
Register no:212222230064
```
```sql
SQL> create table employeee(empid number,empname varchar (20), dept varchar (10) ,salary number);

Table created.

SQL> create or replace procedure insert_employeee_data AS
  2      begin
  3      insert into employeee (empid,empname,dept,salary)
  4      values (1,'Kavinesh','MD',1000000);
  5      insert into employeee (empid,empname,dept,salary)
  6      values (2,'Guru','HR',500000);
  7      insert into employeee (empid,empname,dept,salary)
  8      values (3,'Dhinesh','IT',200000);
  9     commit;
 10    end;
 11     /

Procedure created.

SQL> begin
  2      insert_employeee_data;
  3      end;
  4      /

PL/SQL procedure successfully completed.

SQL> select * from employeee;
```
### Output:
![image](https://github.com/kavinesh8476/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/118466561/108dff39-d9e5-4440-81bb-bfa64aecb871)

### Result:
Hence the procedure using pl/sql is created successfully.
