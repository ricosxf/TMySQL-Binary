TMySQL-Binary
=============

Binary of TMySQL


TMySQL is based on MySQL 5.5.24, developed by Tencent's DBA team.



TMySQL 1.0 (2012-09-25)

1. Add new InnoDB row_format GCS, which is default in TMySQL.
2. Based on GCS row format, table in InnoDB support online adding columns, which only need to modify meta data.

Bug fixed:

1. log-warnings does not work in session level
http://bugs.mysql.com/bug.php?id=66953
2. Insertion of an out-of-range value into a partitioned table was not handled correctly in all cases. This is a regression that first appeared in MySQL 5.5.23. (Bug #14005441, Bug #65587) 
http://bugs.mysql.com/bug.php?id=65587





TMySQL 1.1 (2012-12-07)

1. InnoDB partitioned table support online adding columns.
2. Optimize the memory usage of innnodb's dictionary.

Bug fixed:

1. GBK charset is not Fully supported in mysql
http://bugs.mysql.com/bug.php?id=67739
2. overflow caused replication sql thread failed to execute events
https://bugs.launchpad.net/percona-server/+bug/1070255
