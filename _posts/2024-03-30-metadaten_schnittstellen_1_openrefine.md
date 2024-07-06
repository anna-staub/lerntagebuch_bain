---
title: "Metadaten modellieren (Open Refine)"
date: 2024-03-30
---
Dieser Blogbeitrag fasst die Inhalte der achten und neunten Lehrveranstaltungen des Moduls "Bibliotheks- und Archivinformatik" zusammen. Die Veranstaltungen fanden am 23 und am 30. April 2024 statt und trugen den Titel "Metadaten modellieren und Schnittstellen nutzen 1/2".
Der Blogbeitrag zur vorherigen Lehrveranstaltung "Repository Software für Publikationen und Forschungdaten" ist [hier](https://anna-staub.github.io/lerntagebuch_bain/2024/03/12/repo-software_fuer_publikationen_und_forschungsdaten.html) zu finden, der Beitrag zur folgenden Lehrveranstaltung "Schnittstellen nutzen" [hier](https://anna-staub.github.io/lerntagebuch_bain/2024/05/07/metadaten_schnittstellen_2_schnittstellen.html).

-----

# Inhalte der Lehrveranstaltung
-	OpenRefine
-	Hauptfunktionen
-	Unterstützte Formate
-	Übungen mit OpenRefine

-----

## OpenRefine
[OpenRefine](https://openrefine.org/) ist eine Open Source Software, die es ermöglicht, Rohdaten aufzubereiten, zu normalisieren, zu bereinigen, zu analysieren und sie in andere Formate zu konvertieren. Ausserdem kann man mit OpenRefine auch Daten aus externen Quellen abrufen und den eigenen Datensatz damit abgleichen.
Ursprünglich war OpenRefine ein Projekt von Google und hiess GoogleRefine. Als Google beschloss, das Projekt nicht weiterzuführen, übergaben sie die Software an die Open Source Community, welche diese in OpenRefine umbenannte und bis heute sehr aktiv weiterentwickelt.

----

## Hauptfunktionen

**Facettierung**
Die Software ermöglicht eine Facettierung, das heisst, sie analysiert die Daten und erstellt Kategorien aufgrund von bestimmten Merkmalen. Dank dieser Funktion kann man in OpenRefine wie in jedem Suchkatalog nach Kategorien filtern und somit die Daten effizient durchsuchen und organisieren. 

**Clustering**
Die Software kann Daten anhand von Algorithmen clustern und so Vorschläge generieren, welche Daten zusammengehören könnten, sowie Inkonsistenzen finden.

**Reconciliation**
Mit OpenRefine kann man Daten aus externen Quellen abrufen und die eigenen Daten damit abgleichen, um zusätzliche Information zu erhalten oder Daten zu verifizieren. Die Software bietet dafür eine semiautomatische Funktion.

**Infinite Undo/Redo**
OpenRefine bietet eine unbegrenzte Anzahl an Undo und Redo Schritten und legt ein Änderungspotokoll über das gesamte Projekt hinweg an. Somit können Nutzende ihre Änderungen jederzeit rückverfolgen und auf jeden beliebigen Stand zugreifen.

**Privacy**
Die Software wird lokal auf dem Rechner installiert, somit ist die Verarbeitung von vertraulichen Daten unbedenklich. Nur bei der Datenabfrage aus externen Quellen ist Vorsicht geboten, da die in der Abfrage verwendeten Daten an den externen Service übermittelt werden.

**Wikibase**
Wikibase ist eine Erweiterung der Software, die es ermöglicht, Daten von Wikimedia zu beziehen und Daten auf Wikimedia hochzuladen.

-----

## Unterstützte Formate
OpenRefine unterstützt eine Vielzahl unterschiedlicher Formate. Am einfachsten ist die Nutzung mit tabellarischen Daten, z.B. CSV, XLS oder TXT mit festen Spaltenbreiten oder Trennzeichen. Auch einfache XML-Formate wie z.B. MARCXML oder JSON können gut verarbeitet werden. Schwieriger wird es bei komplexeren XML-Formaten mit hierarchischen Strukturen, z.B. EAD. Deren Verarbeitung ist möglich, benötigt aber zusätzliche Tools.

-----

## Übungen mit OpenRefine
In der Lehreinheit konnten wir über einen CodeSpace die Testversion von OpenRefine ausprobieren. In der ersten Veranstaltung importierten wir Daten und testeten selbstständig die Basisfunktionen der Facettierung, des Zusammenführens und Teilens von Zellen sowie des Clusterings. In der zweiten Veranstaltungen sahen wir uns noch die Funktion der Reconciliation an und glichen unseren Datensatz mit Wikidata ab.
