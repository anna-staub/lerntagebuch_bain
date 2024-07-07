---
title: "Funktion und Aufbau von Archivsystemen"
date: 2024-03-12
---
Dieser Blogbeitrag fasst die Inhalte der vierten und fünften Lehrveranstaltungen des Moduls "Bibliotheks- und Archivinformatik" zusammen. Die Veranstaltungen fanden am 5. und am 12. März 2024 statt und trugen den Titel "Funktion und Aufbau von Archivsystemen".
Der Blogbeitrag zur vorherigen Lehrveranstaltung "Funktion und Aufbau von Bibliothekssystemen" ist [hier](https://anna-staub.github.io/lerntagebuch_bain/2024/02/27/bibliothekssysteme.html) zu finden, der Beitrag zur folgenden Lehrveranstaltung "Repository-Software für Publikationen und Forschungsdaten" [hier](https://anna-staub.github.io/lerntagebuch_bain/2024/03/26/repo-software_fuer_publikationen_und_forschungsdaten.html).
Dazwischen gibt es [hier](https://anna-staub.github.io/lerntagebuch_bain/2024/03/12/vergleich_archivespace_atom.html) noch einen Beitrag zur Übung "Vergleich von ArchiveSpaces und AtoM" .

-----

# Inhalte der Lehrveranstaltung
-	Metadatenstandards in Archiven (ISAD(G) und EAD)
-	ArchivesSpace
-	Unterschiede zwischen Bibliotheks- und Archivsystemen

-----

## Metadatenstandards in Archiven (ISAD(G) und EAD)
Der Standard [ISAD(G)](https://de.wikipedia.org/wiki/ISAD(G)) wurde bereits in zwei früheren Modulen thematisiert, besonders viel war mir aber zu Beginn der Lehrveranstaltung nicht mehr präsent. Die Abkürzung ISAD(G) steht für "International Standard Archival Description (General)" und bezeichnet den wichtigsten Verzeichnungsstandard im Archivwesen. Er wurde 1994 eingeführt und 2000 revidiert. Der Standard besteht aus einer mehrstufigen Verzeichnung im Provenienzprinzip, welche den Entstehungszusammenhang von Archivbeständen abbildet. Die baumartige Tektonik von ISAD(G) ermöglicht zwar die Vermeidung von Redundanzen in den Metadaten, da diese auf nachfolgenden Stufen nicht mehr eigegeben werden, sorgt aber auch dafür, dass die einzelnen Dokumente oftmals nur im Kontext verständlich werden. Angesichts dessen sowie dem Fakt, dass der Standard keine Vorgaben zur Digitalisierung oder zur digitalen Langzeitarchivierung enthält, stösst man mit ISAD(G) an die Grenzen. Deshalb wird aktuell ein neuer Standard namens RiC (Records in Context) erarbeitet. RiC basiert auf Linked Data Prinzipien und soll im Gegensatz zu ISAD(G) polydimensionale Beziehungen und Mehrfachzuordnungen von Dokumenten und Archivbeständen ermöglichen. 
[EAD](https://de.wikipedia.org/wiki/Encoded_Archival_Description) steht für Encoded Archival Description und ist ein XML-basiertes Austauschformat für die Beschreibung von Archivgut. EAD ist sehr flexibel gestaltet und lässt viele Wahlmöglichkeiten offen. Deshalb gibt es verschiedene Anwendungsprofile, die festlegen, welche Werte zugelassen sind. Da wir zu einem späteren Zeitpunkt noch mit EAD-Dateien arbeiten werden, bleibt es bei dieser kurzen Vorstellung des Austauschformates.

-----

## ArchivesSpace
Nach der Einführung in die archivarischen Metadatenstandards sahen wir uns noch ArchivesSpace an. ArchivesSpace ist eine Open Source Software für Archivinformationssysteme, mit der Archivmaterialien verwaltet und grundlegende archivarische Funktionen wie die Regelung des Zugangs, Ordnung und Beschreibung ebendieser Materialien ausgeführt werden können. Die Software ist nur formal Open Source: eine professionelle Nutzung der Software und wichtiger Dokumente wie z.B. des Nutzerhandbuches bedingt eine kostenpflichtige Mitgliedschaft. Über einen Demo-Zugang erstellten wir in Gruppen einen eigenen Datensatz in ArchivesSpace und machten diesen in der öffentlichen Ansicht sichtbar. Weiter importierten wir EAD-Beispieldaten in ArchivesSpace und exportierten sie wieder als MARCXML-Daten. 
Während ArchivesSpace vor allem in den USA eine grosse Community hat, ist der Markt in der Schweiz von den Produkten [scopeArchiv](https://www.scope.ch/de/produkteuebersicht/scopearchiv/) und [CMI AIS](https://cmiag.ch/akten-management/archivierung/ais/) dominiert.

-----

## Unterschiede zwischen Bibliotheks- und Archivsystemen
Bei Bibliothekssystemen liegt der Fokus auf der Mediennutzung und der Benutzerinteraktion. Sie sind auf wechselnde Bestände und Medien aus der Massenproduktion ausgerichtet, und arbeiten grösstenteils mit dem Metadatenstandard MARC21 bzw zukünftig BIBFRAME. Archivsysteme hingegen orientieren sich hingegen an analogen Findmitteln und sind auf beständigere Bestände und Unikate ausgerichtet und fokussieren stark auf den Entstehungszusammenhang von Dokumenten und Beständen. Ausserdem sind Zugriffsrechte bei Archivsystemen ein Thema, welches bei Bibliothekssystemen nicht vorkommt. Archivsysteme arbeiten grösstenteils mit dem Metadatenstandard EAD bzw. zukünftig RiC.
