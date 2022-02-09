# Solution Design

## 1. Standards und Technologien
### 1.1 Rücksprache mit Auftraggeber
Der Auftraggeber stellte die Anforderung, dass das Backend in ASP.NET und das Frontend in VUE.JS entwickelt werden muss.  
Nach Rücksprache mit dem Auftraggeber dürfen wir nun selbst entscheiden, welche Standards wir verwenden, weil keine enge Integration in bereits bestehende Applikationen notwendig ist.   

### 1.2 Backend
Das Backend wird mit Go Version 1.17.6 umgesetzt.   
Das Backend wird als JSON-REST-API umgesetzt.      
Für das Backend sind die Implementierungsrichtlinien der CLEAN-Architecture einzuhalten.   
Für die Datenbank-Interaktion wird ein [ORM](https://gorm.io) verwendet v1.22.5 -> Database first.
Für Gorm verwenden wir den SQLLite Connector [https://github.com/go-gorm/sqlite](https://github.com/go-gorm/sqlite) v

#### 1.2.1 Datenbank
Für die Datenbank haben wir den Standard SQLLite festgelegt.

### 1.3 Frontend
Für das Frontend haben wir den Standard VUE.JS festgelegt. 

#### 1.3.1 UI/UX 
Das User-Interface wird gemäß den Mockups in der Anforderungsspezifikation erstellt.   
Es gibt keine genauen Vorgaben für die Umsetzung der User-Effects.

## 2. Dokumentation 
Die Dokumentation beschränkt sich auf die im Rahmen des SYP-Unterrichts angefertigten Dokumente (Anforderungsspezifikation, Solution-Design).
Für die grafische Modellierung verwenden wir draw.io

<!-- Die Dokumentation verfügt einen Detailierungsgrad von 3. -->

### 3. Aufteilung der Arbeit und Code-Verwaltung
Die Aufteilung der Arbeit sowie die Projektverwaltung erfolgt über Github bzw Git.

## Solution-Modellierung
### Klassen
Bei der Modellierung der Klassen wurden die SOLID-Prinzipien berücksichtig.

<!-- Die Software soll nach dem Chill-Prinzip aufgebaut werden. -->

Falls Fehler aufkommen sollten die Benutzer diese mit Details was genau passiert ist an Waterbyte senden.
## Klassen
## Sequenz
<!-- ## Allgemein -->
## Software Architektur
Das System wird als Server-Client-Architektur umgesetzt. Die verwendeten Standards wurden in 1. festgelegt.

### Daten
Die Daten werden in einer SqlLite-Datenbank gespeichert.

## Deployment
Beim Deployment wird folgendermaßen vorgegangen:
### Backend
- Das Backend wird zu einer ausführbaren Binary-Datei (.exe) kompiliert.
- Anschließend wird die Datei und die SQLLite-Datenbank mittels [scp](https://linux.die.net/man/1/scp) auf den Server kopiert und dort ausgeführt.

### Frontend
- Am Deployment-Server muss ein Nginx-Server installiert sein und laufen
- Die VUE-Applikation wird mittels `vue build` kompiliert und der entstehende Build-Ordner wird mittels [scp](https://linux.die.net/man/1/scp) ins Verzeichnis `/var/www` des Servers kopiert.

## Security
Die finale Website soll nur über https erreichbar sein.

## Technologie-Stack
Siehe Punkt 1.

## Persistierung
Siehe Punkt 1.

## UI/UX
Siehe Anforderungsspezifikation

### Anhang
## Umsetzungskonzept NF-Anforderungen
Das User-Interface wird gemäß den Mockups in der Anforderungsspezifikation erstellt.   
Um eine möglichst schnelle Reaktion des Backends zu gewährleisten wurde der Standard Go gewählt.

## Standard-Beschreibung
Normal bruder

### Qualitätssicherung

## 1.1 Klassen



## 1.2 Testen
Modul-Tests und Unit-Tests werden im Anschluss an das Solution-Design erstellt, danach werden Entwicklungspakete inkl. Verifikation (Tests) auf die Projektmitarbeiter aufgeteilt. (Test-Driven-Development)
