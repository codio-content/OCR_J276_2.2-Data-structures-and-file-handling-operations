Large volumes of data are usually stored in databases created using a database management system (DBMS) such as Access or mySQL. The data is stored in **tables** such as the one below.

![](.guides/img/dbtable.png)

Each column is a **field** – an item of data that is to be stored.
Each row is a **record** – a collection of fields for each instance or example of a ‘car’.

### Key fields
Each record must have a piece of data that is unique to just that record and this is stored in the key field.
But in the table above there is no key field – there could be lots of different Audi cars and different manufacturers could use the same model name. And there are obviously many cars with the same colour and more than one built each year!

A way round this problem is to create another field. In the example above we could insert a field named ‘Number’ and give each car a unique number. 

In school management systems every student is given a unique 10 digit ULN (Unique Learner Number). No other student can have the same one and it can be used for key fields as students may have the same names, post codes etc.