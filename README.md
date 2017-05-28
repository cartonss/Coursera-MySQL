# Coursera-MySQL
hi

%load_ext sql

Now that the SQL library is loaded, we need to connect to a database. The following command will log you into the MySQL server at mysqlserver as the user 'studentuser' and will select the database named 'dognitiondb' :
%sql mysql://studentuser:studentpw@mysqlserver/dognitiondb

Once you are connected, the output cell (which reads "Out" followed by brackets) will read: "Connected:studentuser@dognitiondb". To make this the default database for our queries, run this "USE" command:
%sql USE dognitiondb

SELECT breed
FROM dogs LIMIT 10 OFFSET 5;
10 rows of data will be returned, starting at Row 6.
An alternative way to write the OFFSET clause in the query is:
SELECT breed
FROM dogs LIMIT 5, 10;
