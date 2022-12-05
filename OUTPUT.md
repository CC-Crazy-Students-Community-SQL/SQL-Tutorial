# SQL Output
* &emsp;Diese Befehle gehen in der CLI, also starten wir diese mit `` mysql-ctl cli; ``<br />
* &emsp;In diesem Tutorial wird "name" als Platzhalter für den Name einer Datenban, Tabelle, Feld ... verwendet.<br />
* &emsp;Dieser muss natürlich dann umbenannt werden.<br />
* &emsp;Hier seht Ihr den Output, der durch das CLI angezeigt wird, sofern der Befehlt keinen Fehler ausgibt.<br />

## SQL - Inhaltsverzeichnis
* <a href="#l1">Datenbank anlegen</a>
* <a href="#l2">Datenbanken anzeigen</a>
* <a href="#l3">Datenbank auswählen</a><br />
* <a href="#l4">Tabelle anlegen</a>
* <a href="#l5">Tabelle befüllen</a>
* <a href="#l6">Tabelle anzeigen</a>

## SQL - Standart Ausgabe
  * <a name="l1">Datenbanken erstellen</a><br />
```yaml
OUTPUT:
mysql> CREATE DATABASE test;
Query OK, 1 row affected (0.00 sec)

mysql>
```
  * <a name="l2">Datenbanken anzeigen</a><br />
```yaml
OUTPUT:
mysql> SHOW DATABASES;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mysql              |
| performance_schema |
| sys                |
| test               |    -- neu angelegte Datenbank
+--------------------+
4 rows in set (0.01 sec)

mysql>
```
  * <a name="l3">Datenbank auswählen</a><br />
```yaml
OUTPUT:
mysql> USE test;    -- neu angelegte Datenbank benutzen

Database changed
```
  * <a name="l4">Tabelle anlegen</a><br />
```yaml
OUTPUT:
mysql> CREATE TABLE Persons (PersonID INT NOT NULL PRIMARY KEY, LastName VARCHAR(255), FirstName VARCHAR(255));
Query OK, 0 rows affected (0.16 sec)

mysql>
```
  * <a name="l5">Tabelle befüllen</a><br />
```yaml
OUTPUT:
mysql> INSERT INTO Persons (PersonID, LastName, FirstName) VALUES (1, 'Mustermann', 'Max');
Query OK, 1 row affected (0.01 sec)
mysql> INSERT INTO Persons (PersonID, LastName, FirstName) VALUES (2, 'Musterfrau', 'Maxime');
Query OK, 1 row affected (0.01 sec)

mysql>
```
  * <a name="l6">Tabellen anzeigen</a><br />
```yaml
OUTPUT:
mysql> SELECT * FROM Persons;
+----------+------------+-----------+
| PersonID | LastName   | FirstName |
+----------+------------+-----------+
|        1 | Mustermann | Max       |
|        2 | Musterfrau | Maxime    |
+----------+------------+-----------+
2 rows in set (0.00 sec)

mysql>
```



###### sandrosimperl.cc@gmail.com
