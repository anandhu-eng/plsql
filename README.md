## Pl\SQL

## How to  execute from plsql file
    @{path}{filename.sql}

## Parts of Pl\SQL
- Declerative part (**DECLARE**)
- Executable part (**BEGIN**)
- Exception handling part (**EXCEPTION**)

After the three parts, the code ends with **END**.

## Declaring variables
    var1 NUMBER(2);
    var2 BOOLEAN;
    var3 VARCHAR(100);
If we want to declare variable to hold **m** digits to the left of the decimal point and **n** digits to the right of the decimal point. We declare like this:

    var4 NUMBER(m+n,n);

Declaring constant variables:

    var5 CONSTANT NUMBER := 100;

## Assigning values to variables
-Normal assignment

    tax := price * tax_rate;
    valid_id := FALSE;
    bonus := current_salary * 0.10;
    wages := gross_pay(emp_id, st_hrs, ot_hrs) - deductions;

-Assigning from Database

    Select sal*10 INTO bonus FROM emp WHERE empno=1;
    
Here, we inserted salary with a hike of 10% into variable **bonus**.

## Printing to the console

    dbms_output.put_line('string' | <variable>);

## Inserting values into the database
    insert into summary(total,tot_loads,start_time) values(tot_records,records_loaded,process_start_time);


## If condition 
    IF CONDITION THEN
        STATEMENTS
    END IF;

## For loop
    FOR <variable> IN <initial value> .. <final value> LOOP
        STATEMENTS
    END LOOP;

