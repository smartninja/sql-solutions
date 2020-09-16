### Exercise 1.1: Chinook database

- Download this database: [Chinook.sqlite](https://storage.googleapis.com/smartninja-org-assets/curriculums/sql/Chinook_Sqlite.sqlite)
- Open it with SQLite Browser

#### Exercise solutions

1) This database has many tables. Write an SQL command that will print **Name** from the table **Artist** (for all the database entries).

```sql
SELECT Artist.Name
FROM Artist;
```

2) Print all data from the table **Invoice** where `BillingCountry` is **Germany**.

```sql
SELECT *
FROM Invoice
WHERE  Invoice.BillingCountry = 'Germany';
```

3) Count how many **albums** are in the database. Look into the SQL documentation for help: [http://www.w3schools.com/sql/sql_functions.asp](http://www.w3schools.com/sql/sql_functions.asp)).

```sql
SELECT COUNT(*)
FROM Album;
```

4) How many customers are from France?

```sql
SELECT COUNT(*)
FROM Customer
WHERE Customer.Country = 'France';
```

5) What is the **sum** of all invoices (their totals) in the database?

```sql
SELECT SUM(Invoice.Total)
FROM Invoice;
```

6) How much is the **average** of all the invoice totals?

```sql
SELECT AVG(Invoice.Total)
FROM Invoice;
```
