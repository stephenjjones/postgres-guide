Commands
========

connect to postgres

  .. code-block:: console

      $ psql

Commands::

    =# \list   show databases

    =# \dt     list tables in current database

    -- make sure connection is termintated first
    =# drop database dbname;   drop database

    =# \c dbname     switch db connection

    -- terminate db connection
    =# select pg_terminate_backend(pid) from pg_stat_activity_where datname='YourDatabase';
    
    -- create database
    =# CREATE DATABASE your_db OWNER yourdbuser ENCODING 'UTF8';

    =# \q      quit database
    
    =# ALTER TABLE table_name RENAME COLUMN column_name TO new_column_name;

    =# ALTER TABLE assets ALTER COLUMN name TYPE VARCHAR;
    
    =# ALTER TABLE table_name ALTER COLUMN column_name SET DEFAULT NULL;
    
    =# ALTER TABLE customers ADD COLUMN contact_name VARCHAR NOT NULL;

    =# ALTER TABLE mytable ALTER COLUMN mycolumn DROP NOT NULL;
