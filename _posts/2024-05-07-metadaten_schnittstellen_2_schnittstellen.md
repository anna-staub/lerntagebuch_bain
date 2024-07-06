---
title: "Schnittstellen nutzen"
date: 2024-05-08
---
Dieser Blogbeitrag fasst die Inhalte der zehnten Lehrveranstaltung des Moduls "Bibliotheks- und Archivinformatik" zusammen. Die Veranstaltung fand am 7. Mai 2024 statt und trug den Titel "Metadaten modellieren und Schnittstellen nutzen 2/2".
Der Blogbeitrag zur vorherigen Lehrveranstaltung "Metadaten modellieren" ist [hier](https://anna-staub.github.io/lerntagebuch_bain/2024/03/12/metadaten_schnittstellen_1_openrefine.html) zu finden, der Beitrag zur folgenden Lehrveranstaltung "Suchmaschinen und Discovery Systeme 1" [hier](https://anna-staub.github.io/lerntagebuch_bain/2024/05/21/suchmaschinen_discovery_systeme_1.html).

-----

# Inhalte der Lehrveranstaltung
-	Ausgangsdaten
-	Schnittstellen
-	Konvertierung in MARC21

-----

## Ausgangsdaten
In den bisherigen Lehrveranstaltungen haben wir uns mit Metadaten in den Systemen Koha, ArchivesSpace, DSpace und OpenRefine beschäftigt. In der heutigen Veranstaltung ging es darum, wie Metadaten von ebensolchen Systemen geharvested und einheitlich in das Datenformat MARC21-XML konvertiert werden können (siehe Schaubild). Die Daten aus Koha (Format: MARC21-XML), ArchivesSpace (Format: EAD), DSpace (Format: Dublin Core) und OpenRefine (MARC21-XML) bilden also unsere Ausgangsdaten.

<img width="450" alt="grafik" src="https://github.com/anna-staub/lerntagebuch_bain/assets/90337803/b12b2234-0c12-4de9-a5a9-2ad7e37c6f63">


-----

## Schnittstellen
Um den Austausch von Daten zwischen verschiedenen Systemen zu ermöglichen, arbeitet man mit Schnittstellen. Diese verwenden sogenannte Austauschprotokolle. Im Bibliotheks- und Archivbereich gibt es zahlreiche solche Protokolle, drei davon sind besonders weit verbreitet:

-	[Z39.50](https://www.loc.gov/z3950/agency/) (Library of Congress)
-	[SRU](https://www.loc.gov/standards/sru/) – Search/Retrieve via URL (Library of Congress)
-	[OAI-PMH](https://www.openarchives.org/pmh/) – Open Archives Initiative Protocol for Metadata Harvesting (Open Archives Initiative

Z39.50 und SRU eignen sich besonders für Live-Abfragen oder gezielten Datenabruf mit vielen Parametern, während OAI-PMH vor allem auf grössere Datenabzüge und regelmässige Aktualisierungen abzielt. Z39.50 ist ausserdem recht alt und benötigt Spezialsoftware um Daten abzurufen, während mit SRU und OAI-PMH die Anfragen direkt über den Browser aufgerufen werden können. 
In der Veranstaltung befassten wir uns mit dem Protokoll OAI-PMH. Über einen Codespace und ein vorbereitetes Repository konnten wir Metadaten aus den Demoversionen von Koha, ArchivesSpace und DSpace in die Software VuFindHarvest importieren. 

-----

## Konvertierung
Die importierten Daten, die nun in verschiedenen Formaten vorlagen (MARC21, EAD und DC) sollten nun alle in MARC21-XML konvertiert werden. Die Konvertierung von einem Metadatenstandard zu einem anderen wird auch "Crosswalk" genannt. Für ein Crosswalk müssen die beiden beteiligten Metadatenstandards verglichen werden, und für jedes Datenfeld des Ausgangsformates ein entsprechendes Feld im Zielformat bestimmt werden. Für die gängigen Standards sind bereits solche Mappings verfügbar, beispielsweise das Mapping für die Konvertierung von MARC zu Dublin Core. 
Im Idealfall ist ein Crosswalk verlustfrei, das heisst jedes Datenfeld des Ausgangsformates hat ein entsprechendes Feld im Zielformat. 
Die Konvertierung selbst haben wir mit XSLT gemacht, einer Programmiersprache für die Transformation von XML-Dokumenten. Mit Hilfe von vorgefertigten XSL-Stylesheets benutzten wir ein [Transformationstool](http://xsltransform.net/), und erhielten die transformierten Daten im MARC21-XML Format zurück.
