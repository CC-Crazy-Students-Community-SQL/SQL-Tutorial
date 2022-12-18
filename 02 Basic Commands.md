# SQL
* &emsp;Diese Befehle gehen in der CLI, also starten wir diese mit `` mysql-ctl cli; ``<br />
* &emsp;In diesem Tutorial wird "name" als Platzhalter für den Name einer Datenban, Tabelle, Feld ... verwendet.<br />
* &emsp;Dieser muss natürlich dann umbenannt werden<br />

## SQL - Inhaltsverzeichnis
* <a href="#l1">MySQL Datenbanken anzeigen lassen</a><br />
* <a href="#l2">Tabellen anzeigen lassen</a></a></a><br />
* <a href="#l3">Datenbank anlegen</a></a><br />
* <a href="#l7">Datenbank löschen</a></a><br />
* <a href="#l4">Tabellen anlegen</a><br />
* <a href="#l8">Tabellen löschen</a><br />
* <a href="#l5">Datenbank / Tabelle auswählen</a><br />
* <a href="#l6">.sql Dateien aufrufen im CLI</a><br />
* <a href="#l9">Objekte nach Existez abfragen</a><br />

## SQL - Standart Befehle
* <a name="l1">Datenbanken anzeigen lassen</a><br />
```yaml
SHOW DATABASES;
```
* <a name="l2">Tabellen anzeigen lassen</a>
  * Dieser Befehl geht nur mit einer ausgewählten Datenbank<br />
```yaml
SHOW TABLES;
```
* <a name="l3">Datenbank anlegen</a><br />
```yaml
CREATE DATABASE name;
```
* <a name="l7">Datenbank löschen</a><br />
```yaml
DROP DATABASE name;
```
* <a name="l4">Table anlegen</a>
  * Dieser Befehl geht nur mit einer ausgewählten Datenbank<br />
  * Dieser Befehl geht nicht ohne Felder, kommt aber noch später<br />
```yaml
CREATE TABLE name;
```
* <a name="l8">Table löschen</a>
  * Dieser Befehl geht nur mit einer ausgewählten Datenbank<br />
```yaml
DROP TABLE name;
```
* <a name="l5">Datenbank oder Tabelle zur Verwendung auswählen</a><br />
```yaml
USE name;
```
* <a name="l5">.sql Dateien aufrufen im CLI</a><br />
```yaml
SOURCE path/file.sql;
```
* <a name="l9">Objekte nach Existez abfragen</a><br />
```yaml
DROP TABLE IF EXISTS name;
```
```yaml
CREATE DATABASE IF NOT EXISTS name;
```

###### sandrosimperl.cc@gmail.com
