Installation
============

Mac (OS X)
----------

Install and connect to postgres::

    $ brew update
    $ brew install postgresql
    $ which psql # confirm proper installation at /usr/local/bin/psql
    $ postgres -D /usr/local/var/postgres # start postgres server
    $ createdb 'whoami' # create a default db based on your username
    $ psql

Create a database::

    =# CREATE DATABASE yourdbname OWNER yourdbuser ENCODING 'UTF8'
    OR
    =# CREATE DATABASE yourdbname
    =# CREATE USER myprojectuser WITH PASSWORD 'password';
    =# ALTER ROLE myprojectuser SET client_encoding TO 'utf8';
    =# ALTER ROLE myprojectuser SET default_transaction_isolation TO 'read committed';
    =# ALTER ROLE myprojectuser SET timezone TO 'UTC';
    =# GRANT ALL PRIVILEGES ON DATABASE myproject TO myprojectuser;
    =# \q

Ubuntu
------
Install client::

    $ sudo apt-get install postgresql-client
