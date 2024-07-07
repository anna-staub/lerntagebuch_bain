---
title: "Linked Data"
date: 2024-06-04
---
Dieser Blogbeitrag fasst die Inhalte der dreizehnten und letzten Lehrveranstaltung des Moduls "Bibliotheks- und Archivinformatik" zusammen. Die Veranstaltung fand am 03. Juni 2024 statt und trug den Titel "Linked Data".
Der Blogbeitrag zur vorherigen Lehrveranstaltung "Suchmaschinen und Discovery Systeme 2" ist [hier](https://anna-staub.github.io/lerntagebuch_bain/2024/05/21/suchmaschinen_discovery_systeme_2.html) zu finden, der abschliessende Beitrag mit einem Fazit zu meiner Lernerfahrung [hier](https://anna-staub.github.io/lerntagebuch_bain/2024/06/29/outro.html).

-----

# Inhalte der Lehrveranstaltung
-	Aktuelle Datenmodelle für Metadaten
-	Linked Open Usable Data (LOUD)

-----

## Aktuelle Datenmodelle für Metadaten (BIBFRAME und RiC)
Die aktuellen Datenmodelle für Metadaten sind Records in Context (RiC) im Archivwesen und BIBFRAME im Bibliothekswesen. BIBFRAME und RiC wurden bereits in den Lehrveranstaltungen zur Funktion und Aufbau von Bibliotheks- und Archivsystemen kurz erwähnt, jedoch in diesem Blog nicht genauer untersucht.

### BIBFRAME
BIBFRAME wird seit 2021 auf Initiative der Library of Congress entwickelt und löst MARC21 ab. BIBFRAME basiert auf den Functional Requirements for Bibliographic Records (FRBR) und orientiert sich zu einem grossen Teil an den Richtlinien des Resoucre Desctiption and Access (RDA) Regelwerks. BIBFRAME setzt sich zusammen aus dem BIBFRAME-Datenmodell und dem BIBFRAME-Vokabular. Das Datenmodell unterscheidet zwischen  *Work*, *Instance* und *Item*, wobei Work die höchste Ebene ist, und das konzeptionelle Wesen der katalogisierten Ressource repräsentiert. Mit einem Werk verknüpft BIBFRAME Entitäten wie Thema, Agents oder Ereignisse. Ein Werk (Work) kann verschiedene materielle  Instanzen (Instance) haben, beispielsweise kann ein Buch als Hardcover, Softcover oder E-Book in deutscher, englischer oder sonstiger Sprache veröffentlicht werden. BIBFRAME verknüpft Instanzen mit Entitäten wie einem Format oder einem Verlag. Von einer Instanz schliesslich können ganz viele einzelne Exemplare (Items) existieren, welche BIBFRAME mit Entitäten wie Barcode, Signatur oder Standort verknüpft. 

![grafik](https://github.com/anna-staub/lerntagebuch_bain/assets/90337803/2bf87913-73a6-48f8-b91f-5b0dd0bfb9b1)
 
(Bildquelle: [loc.gov](https://www.loc.gov/bibframe/docs/bibframe2-model.html))

Das BIBFRAME-Vokabular, ist eine Ontologie und definiert Konzepte und deren Eigenschaften zur Beschreibung der Entitäten im Datenmodell.
BIBFRAME fokussiert also auf die Erfassung und klare Identifikation von einzelnen Ressourcen oder Identitäten, und auf deren Beziehungen. MARC21 hingegen funktioniert sehr medienzentriert und verlangt Angaben wie z.B. Autorinnen nicht wie BIBFRAME als verlinkte Entität, sondern zwingt einen dazu, diese Entitäten in jedem Datensatz wieder neu zu erfassen, wobei natürlich Redundanzen entstehen und damit das Risiko für Fehler steigt.

### Records in Context (RiC)
RiC ist der aktuelle Metadatenstandard im Archivwesen. Auch er basiert auf den Prinzipien von Linked Data und ermöglicht neue und mehrfache Beziehungen zwischen Entitäten. Der Standard setzt jedoch andere Schwerpunkte als BIBFRAME, beispielsweise ist die Provenienz im Archivwesen und damit in RiC sehr wichtig. 


![RiC](https://github.com/anna-staub/lerntagebuch_bain/assets/90337803/3e30daa3-0dbc-4318-a961-38677de989f5)

(Bildquelle: [ica.org/](https://www.ica.org/standards/RiC/RiC-O_1-0-1.html))

-----

## Linked Open Usable Data (LOUD)
Das Konzept [Linked Open Usable Data (LOUD)](https://linked.art/loud/) erweitert das Konzept von [Linked Open Data (LOD)](https://de.wikipedia.org/wiki/Linked_Open_Data) um den Aspekt der Usability, indem es auf die Perspektive der Nutzenden fokussiert. Das Konzept orientiert sich an fünf Grundprinzipien:

A.	Das passende **A**bstraktionslevel für die Zielgruppe finden

B.	Möglichst wenig **B**arrieren für den Einstieg

C.	Verständlich(**C**omprehensible) durch Introspektion (Die Daten sind so gespeichert, dass Betrachterinnen verstehen worum es geht, ohne Ontologien und Vokabularien konsultieren zu müssen)

D.	**D**okumentation mit praktischen Beispielen

E.	Wenige Ausnahmen (**E**xceptions), viele konsistente Muster


