---
title: "Suchmaschinen und Discovery Systeme 2"
date: 2024-06-03
---
Dieser Blogbeitrag fasst die Inhalte der zwölften Lehrveranstaltung des Moduls "Bibliotheks- und Archivinformatik" zusammen. Die Veranstaltung fand am 03. Juni 2024 statt und trug den Titel "Suchmaschinen und Discovery Systeme 2".
Der Blogbeitrag zur vorherigen Lehrveranstaltung "Suchmaschinen und Discovery Systeme 1" ist [hier](https://anna-staub.github.io/lerntagebuch_bain/2024/05/21/suchmaschinen_discovery_systeme_1.html) zu finden, der Beitrag zur folgenden Lehrveranstaltung "Linked Data" [hier](https://anna-staub.github.io/lerntagebuch_bain/2024/06/03/linked_data.html).

-----

# Inhalte der Lehrveranstaltung
-	Integration von Daten in VuFind
-	VuFind Konfiguration

-----

## Import von Daten in VuFind 
In der vorherigen Veranstaltung hatten wir uns die Benutzeroberfläche von VuFind angesehen, in der hier behandelten Veranstaltung ging es dann darum, Daten in VuFind zu importieren. Da ich leider nicht an der Veranstaltung teilnehmen konnte, verpasste ich auch die Gruppenübung, bei der die Klasse hands-on Daten in VuFind importierte. Stattdessen habe ich mir die Aufzeichnung angesehen und mich mit der [Dokumentation zum Import von MARC Daten in VuFind](https://vufind.org/wiki/indexing:marc) befasst.

In einem ersten Schritt müssen die Daten, die importiert werden sollen, aus dem Bibliothekssystem exportiert werden, entweder im binären MARC Format oder in MARC-XML. Die Dateiendungen der exportierten Daten sollte also .mrc oder .xml sein. Jeder exportierte Datensatz muss ausserdem über einen eindeutigen Identifier verfügen, so dass VuFind die Datensätze voneinander unterscheiden kann. In welchem Feld dieser Identifier steht, kann selbst in der *marc.properties* Datei festgelegt werden. 
Als nächstes müssen die Einstellungen des Import-Tools, insbesondere Dateipfade und URLs, geprüft und allenfalls angepasst werden. Das Import-Tool stützt sich auf die  Einstellungen in der Datei import.properties. Anpassungen können in dieser Datei vorgenommen werden – oder man weist das Import-Tool beim Import an, die Einstellungen aus einer anderen Datei anzuwenden.
Wenn die zu importierenden Daten bereitstehen und die Einstellungen des Import-Tools korrekt sind, kann man mit dem eigentlichen Importieren beginnen (Anmerkung: die hier erwähnten Shell-Befehle gelten für Linux-Systeme). Dazu bewegt man sich in der Shell zum VuFind Installations-Ordner wendet dort den folgenden Befehl an:

> ./import-marc.sh deine_importdatei.mrc

Möchte man das Import-Tool anweisen, die Einstellungen aus einer anderen Datei anzuwenden (z.B. wenn man unterschiedliche Datensätze mit unterschiedlichen Mappings importieren möchte), kann man dafür noch "-p" verwenden, das sieht dann folgendermassen aus:

> ./import-marc.sh  -p /usr/local/vufind/import/custom.properties deine_importdatei.mrc

-----

## VuFind Konfiguration
Für die Konfiguration von VuFind gibt es ein lokales und ein globales Verzeichnis. Generell wird empfohlen, Konfigurationsdateien im lokalen Konfigurationsverzeichnis abzuspeichern, da Änderungen an Dateien im lokalen Verzeichnis auch die entsprechenden Dateien im globalen Verzeichnis überschreiben. Die allgemeinen Einstellungen befinden sich in der Datei *config.ini*, in der viele Einstellungsmöglichkeiten mit Kommentaren erklärt sind. *config.ini* kann mit einem Text Editor bearbeitet werden, in der [Konfigurations-Dokumentation von VuFind](https://vufind.org/wiki/configuration) sind alle möglichen Einstellungen aufgezählt und erläutert.

