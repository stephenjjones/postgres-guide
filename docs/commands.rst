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
