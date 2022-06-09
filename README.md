The dict.py is an interactive dictionary integrated with psql
Before running the programm, we need to create a data base first.

Follow these steps with the commands bellow:

1. open psql and type your password:
psql postgres postgres

2. create the database dict:
postgres=# create database dict;

3. Create user and password:
NOTE : the same user and password will be inserted into dict.py
postgres=# create user dict with password 'abc123';
postgres=# grant all privileges on database dict to dict;
postgres=# \q

4. Go to the dict database:
psql dict dict

5. Run the program dict.sql:
\i dict.sql

All set!