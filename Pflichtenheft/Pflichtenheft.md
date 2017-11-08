
Software Projekt (Alexa/Google Home)
====================================
Pflichtenheft
-------------

Fachhochschule Bielefeld

Campus Minden

Studiengang Informatik

----------

Beteiligte Personen:

Name                   | Matrikelnummer
---------------------- | ---------------
**Projektleiter**      | 
Jan-Hendrik Sünderkamp | 1153536
**Team Alexa**         | 
Philipp Clausing       | 1078231
Devin-Alexander Meier  | 1087170
Tobias Muth            | 1077429
**Team Google**        | 
Peter Dick             | 1050185
Alexander Jaksties     | 1077474
Daniel Nagel           | 1085754

07. November 2017

----------


Softwarespeziﬁkation
====================

Softwareanforderungen
---------------------
Fernsteuerung eines PC durch: Alexa, Google Home Mini
Desktopapp, Alexa skill, Google home anwendung

Funktionale Anforderungen | Nichtfunktionale Anforderungen
------------------------- | -------------------------------
**Desktopapp** | 
Konﬁgurierbarkeit der Desktop App | Selbsterklärende GUI der Desktop App
Speichern von Pfadangaben, ausführbaren Dateiendungen und anderen Geräten |
Optisches Feedback bei Ladezeiten |
Standardbefehle für Programme |
Vorkonﬁgurationen für bekannte Programme |
Vorkonﬁgurationen für neue Programme (Templates) |
Eintragen neuer Programme |
Kommandozeilenbefehle (o) &
Skripte starten (o) |
**Voice Assistenten** |
Shutdown Timer | Möglichst einheitliches Protokoll (z.B. Open-HAB)
Umsetzung innerhalb eines Netzwerkes |
Wake on LAN (o) |
----------

User Stories
------------
### Desktopanwendung

* Als Benutzer möchte ich eine intuitive Oberfläche der Desktopanwendung angezeigt bekommen, um keine Dokumentation lesen zu müssen.
* Als Benutzer möchte ich ein optisches Feedback bekommen, um zu wissen ob die Desktopanwendung mit ihrer Arbeit noch nicht fertig ist.
* Als Benutzer möchte ich Vorkonfigurationen für Programme angeboten bekommen, um Zeit zu sparen.
* Als Benutzer möchte ich vorgefertige Konfigurationen für neue Programme nutzen, um Zeit bei der Konfiguration zu sparen.
* Als Benutzer möchte ich Skripte ausführen können, um individuelle Operationen mit einem Befehl auszuführen.

### Voice Assistent

* Als Benutzer möchte ich meine Lieblingsprogramme mit meiner Stimme steuern, um meine Komfortabilität zu steigern.
----------

Use-Cases
---------

![Use-Case System](UseCase-Diagramme/KBP_UseCase_System.png "Use-Case System")

----------

Architekturdiagramm
-------------------

![Systemarchitektur](Systemarchitektur/KBP_System_Architektur.png "Systemarchitektur")

Das obige Diagramm stellt die Systemarchitektur dar. Auf der linken Seite des Diagramms sind vorerst nutzbare Voice Assistents an ein lokales Netzwerk angebunden. Ziel ist es, dass beliebige Voice Assistens an das finale System angebunden werden können. Über das Netzwerk wird eine Software auf einem PC-Client angesteuert. Diese Software soll sowohl bekannte Assistenten, als auch bekannte Programme speichern und verwalten können. Dazu bedient sie sich einer Datenbank.
