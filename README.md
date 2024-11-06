Enter password: ******
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 38
Server version: 8.0.35 MySQL Community Server - GPL

Copyright (c) 2000, 2023, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql> show databases;
+------------------------------+
| Database                     |
+------------------------------+
| azcare                       |
| bookstore                    |
| classicmodels                |
| crimeanalysisdb              |
| crimeanalysisreportingsystem |
| e_com                        |
| fhms                         |
| fsd_oct_sample_db            |
| fsd_oct_sms_db               |
| hex_fsd_nov_24_insurance_db  |
| hexaware                     |
| hmsazcare                    |
| hospitalmanagementsystem     |
| information_schema           |
| lab_op                       |
| mydatabase                   |
| myecomapp                    |
| mysql                        |
| new_db                       |
| order_management_db          |
| ordermanagementsystem        |
| org                          |
| performance_schema           |
| sidb                         |
| sys                          |
| temp                         |
+------------------------------+
26 rows in set (0.02 sec)

mysql> use hex_fsd_nov_24_insurance_db;
Database changed
mysql> show tables;
+---------------------------------------+
| Tables_in_hex_fsd_nov_24_insurance_db |
+---------------------------------------+
| policy                                |
| policy_seq                            |
+---------------------------------------+
2 rows in set (0.01 sec)

mysql> select * from policy;
Empty set (0.03 sec)

mysql> select * from policy;
+----+-----------------------------------------------------------------------+-----------------+---------------+--------------------------------+
| id | description                                                           | policy_category | policy_type   | title                          |
+----+-----------------------------------------------------------------------+-----------------+---------------+--------------------------------+
|  1 | Covers third party expenses from repairing to new spare parts         | CAR             | THIRD_PARTY   | Partial Coverage Policy        |
|  2 | Covers repairing cost comprehensively                                 | CAR             | COMPREHENSIVE | Partial Repair Coverage Policy |
|  3 | Covers all expenses comprehensively from repairing to new spare parts | BIKE            | COMPREHENSIVE | Full Alpha Coverage Policy     |
+----+-----------------------------------------------------------------------+-----------------+---------------+--------------------------------+
3 rows in set (0.01 sec)

mysql> select * from policy;
+----+-----------------------------------------------------------------------+-----------------+---------------+--------------------------------+
| id | description                                                           | policy_category | policy_type   | title                          |
+----+-----------------------------------------------------------------------+-----------------+---------------+--------------------------------+
|  1 | Covers third party expenses from repairing to new spare parts         | CAR             | THIRD_PARTY   | Partial Coverage Policy        |
|  2 | Covers repairing cost comprehensively                                 | CAR             | COMPREHENSIVE | Partial Repair Coverage Policy |
|  3 | Covers all expenses comprehensively from repairing to new spare parts | BIKE            | COMPREHENSIVE | Full Alpha Coverage Policy     |
+----+-----------------------------------------------------------------------+-----------------+---------------+--------------------------------+
3 rows in set (0.00 sec)

mysql> select * from policy;
+----+-----------------------------------------------------------------------+-----------------+---------------+-----------------------------+
| id | description                                                           | policy_category | policy_type   | title                       |
+----+-----------------------------------------------------------------------+-----------------+---------------+-----------------------------+
|  1 | Covers third party expenses from repairing to new spare parts         | CAR             | THIRD_PARTY   | Partial Coverage Policy     |
|  2 | Covers repairing cost comprehensively                                 | CAR             | COMPREHENSIVE | Third Party Coverage Policy |
|  3 | Covers all expenses comprehensively from repairing to new spare parts | BIKE            | COMPREHENSIVE | Full Alpha Coverage Policy  |
+----+-----------------------------------------------------------------------+-----------------+---------------+-----------------------------+
3 rows in set (0.00 sec)

