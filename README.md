# sql-tutorial
https://www.youtube.com/watch?v=xaWlS9HtWYw&amp;list=PL-osiE80TeTsKOdPrKeSOp4rN3mza8VHN

## Installation

1. Install Postgres and a simple UI 

    ```bash
    brew install postgresql
    # https://youtu.be/xaWlS9HtWYw?list=PL-osiE80TeTsKOdPrKeSOp4rN3mza8VHN&t=192
    brew cask install psequel 
    ```

2. Start Postgres
    ```bash
    brew services start postgresql
    ```

3. Initialize the database
    ```bash
    createdb sample_db
    psql sample_db 
    ```

## Creating the first table
https://youtu.be/w4HEVY_GjqY?list=PL-osiE80TeTsKOdPrKeSOp4rN3mza8VHN&t=317

[Postgres Dataype Table](https://www.postgresql.org/docs/9.5/static/datatype.html#DATATYPE-TABLE)

```sql
VARCHAR(N) /*Where n is maximum amount of characters that will be stored in the field*/
```

## Delete a table
```sql
DROP TABLE people
```

## Populate data
https://youtu.be/fA0jpjwi4J8?list=PL-osiE80TeTsKOdPrKeSOp4rN3mza8VHN

It is possible to insert data with or without fieldnames.

```sql
INSERT INTO people VALUES (3, 'Dave')
INSERT INTO people (id, name) VALUES (3, 'Dave')
```
