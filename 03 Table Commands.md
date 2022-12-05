# SQL - Tabellen Befehle
* &emsp;Diese Befehle gehen in der CLI, also starten wir diese mit `` mysql-ctl cli; ``<br />
* &emsp;In diesem Tutorial wird "name" als Platzhalter für den Name einer Datenban, Tabelle, Feld ... verwendet.<br />
* &emsp;Dieser muss natürlich dann umbenannt werden<br />

## SQL - Inhaltsverzeichnis
* <a href="#l1">Tabelle erstellen</a><br />
* <a href="#l2">Tabelle befüllen</a><br />


## <a name="l1">SQL - CREATE - Tabelle erstellen</a>
* Definition<br />
```yaml
CREATE TABLE name (Attributdefinition [PRIMARY KEY]) [, FOREIGN KEY (Attributliste) REFERENCES Tabellenname (Attributliste)]);
```
* Erklärung<br />
```yaml
CREATE TABLE table_name (feld_name feld_datentyp(eventuelle_menge) feld_attribute feld_standart_wert);
```
* Beispiel<br />
```yaml
CREATE TABLE Persons (PersonID INT NOT NULL PRIMARY KEY, lastname VARCHAR, firstname VARCHAR);
```
<br />

## <a name="l2">SQL - INSERT - Tabelle befüllen</a>
* Definition<br />
```yaml
INSERT INTO Quelle [(Auswahlliste)] VALUES (Werteliste) | SELECT <Auswahlkriterien>;
```
* Erklärung<br />
```yaml
INSERT INTO table_name (feld_name_1, feld_name_2) VALUES ('feld_inhalt_1', 'feld_inhalt_2') | SELECT <aus_select_daten_bekommen>;
```
* Beispiel<br />
```yaml
INSERT INTO Persons (PersonID, LastName, FirstName) VALUES (1, 'Mustermann', 'Max');
```


###### sandrosimperl.cc@gmail.com
