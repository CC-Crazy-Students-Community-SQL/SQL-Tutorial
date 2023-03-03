# SQL

## SQL Server- Standart Befehle

* MySQL DB-Start
  * Startet den SQL Server

```yaml
mysql-ctl start;
```
  * Startet den SQL Server

```yaml
sudo service mysql start;
```
* MySQL DB-Stop
    * Stopt den SQL Server

```yaml
mysql-ctl stop;
```
* MySQL DB-CLI start
    * Startet das Command Line Interface auf dem SQL Server

```yaml
mysql-ctl cli;
```
* MySQL DB-CLI exit
    * Beendet das Command Line Interface auf dem SQL Server

```yaml
CREATE USER 'user'@'host' IDENTIFIED BY 'password';
```
* CREATE USER 'user'@'host' IDENTIFIED BY 'password';
    * Erstellt den User mit dem Passwort, um nicht den root nutzen zu müssen

```yaml
GRANT ALL PRIVILEGES ON *.* TO 'user'@'host' WITH GRANT OPTION;
```
* GRANT ALL PRIVILEGES ON *.* TO 'user'@'host' WITH GRANT OPTION;
    * Gibt dem User zu allen Datenbanken Berechtigung
    * WITH GRANT OPTION nur wenn der User auch GRANT Berechtigungen haben soll

```yaml
FLUSH PRIVILEGES;
```
* FLUSH PRIVILEGES;
    * Reloaded die Berechtigungen, damit die Berechtigunen greifen, ansonten müsste man den Server restarten.

```yaml
exit;
```

###### sandrosimperl.cc@gmail.com
