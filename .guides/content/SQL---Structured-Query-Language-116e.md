Structured query language (SQL) is a language for creating, accessing and manipulating databases. It allows users to search for records which contain a particular item or items of data.

Example commands include:
```sql
SELECT 
FROM
WHERE 
LIKE
AND 
OR
```
And symbols such as

- ```*```
and

- ```%```

Using the tblCars table the following command can be used to display records:
```sql
SELECT * FROM tblCars;
```
This will display all of the records in the table and show all of their fields. The * symbol is used for ‘display all records’.

Notice that a semi-colon is used the finish the statement and the command words are in upper case. But that is not essential as lower case work just as well.
```sql
SELECT Make, Model FROM tblCars;
```
This will display all of the records but only the two fields indicated.
```sql
SELECT Make, Model FROM tblCars
WHERE Make LIKE “Audi”;
```
This will display only one record where the make is ‘Audi’ and show the two fields.
```sql
SELECT Make, Year FROM tblCars
WHERE Make LIKE “Audi” OR Make LIKE “Hyundai”;
```
This will display two records with the two fields indicated.
```sql
SELECT Make, Model, Power FROM tblCars
WHERE Year < 2016 AND Power > 1.4;
```
This would display records of cars made before 2016 with an engine size greater than 1.4.

The % symbol is used the replace one or more characters.

If you had a table of students and you wanted all of the ones with a surname starting with ‘W’ you would write:
```sql
WHERE Surname LIKE “W%”
```