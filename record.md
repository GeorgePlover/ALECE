- You need to specify the directory '$PG_DATADIR$' to put the database data and create a database whose name is the same with your account name of the Linux system. Suppose your account name is 'nsh' and your postgresql data directory is '/home/nsh/pg_data', run the following scripts.
```bash
- initdb -D /home/nsh/pg_data
- set port = 5433 in /home/nsh/pg_data/postgresql.conf
- pg_ctl -D /home/nsh/pg_data start
- psql -p 5433 dbname=postgres
- create database nsh;
```