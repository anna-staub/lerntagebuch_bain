---
title: "Funktion und Aufbau von Bibliothekssystemen"
date: 2024-02-27
---
Dieser Blogbeitrag fasst die Inhalte der dritten Lehrveranstaltung des Moduls "Bibliotheks- und Archivinformatik" zusammen. Die Veranstaltung fand am 27. Februar 2024 statt und trug den Titel "Funktion und Aufbau von Bibliothekssystemen".
Der Blogbeitrag zur zweiten Lehrveranstaltung "Technische Grundlagen 2" ist [hier](https://anna-staub.github.io/lerntagebuch_bain/2024/02/16/grundlagen2.html) zu finden, der Beitrag zur vierten Lehrveranstaltung "Funktion und Aufbau von Archivsystemen" [hier] .

-----

# Inhalte der Lehrveranstaltung
- Metadatenstandards in Bibliotheken
-	Vergleich MARC21 und Dublin Core
-	Koha

-----

## Metadatenstandards in Bibliotheken
MARC 21 wurde 1999 von der Library of Congress gegründet und ist bis zum heutigen Zeitpunkt der am weitesten verbreitete Metadatenstandard für den Austausch von Daten zwischen Bibliotheken oder Verlagen. Es gibt vereinzelt Software mit herstellerspezifischen Metadatenstandards, diese verfügen jedoch immer auch über eine Import- und Exportfunktion für MARC21. Die Daten werden in MARC21 in Feldern abgespeichert, welche jeweils mit Zahlen und Buchstaben gekennzeichnet sind (siehe [Verzeichnis](https://www.loc.gov/marc/bibliographic/bdsummary.html) - in moderneren Metadatenstandards wurde dieses System von sprechenden Feldnamen abgelöst. Weiter ist MARC21 medienzentriert, das heisst jegliche Angaben zu einem Medium sind in einem dazugehörigen Datensatz abgespeichert. So werden beispielsweise die Angaben zu den Autor:innen in jedem Datensatz neu erfasst – was Redundanzen erzeugt und die Wahrscheinlichkeit für Katalogisierungsfehler erhöht. Modernere Standards arbeiten nicht mehr medienzentriert sondern nach dem Prinzip von Linked Data – Urheber:innen, Werke und Instanzen werden also z.B. getrennt voneinander erfasst und im Anschluss verlinkt. MARC21 Dateien können entweder als XML gespeichert werden oder im standardeigenen Binärformat .mrc. Um.mrc Dateien zu lesen ist eine spezielle Software nötig, welche alle grösseren Bibliothekssysteme wie z.B. Koha integriert haben.
In Zukunft wird MARC21 von BIBFRAME abgelöst werden, einem ebenfalls von der Library of Congress erarbeiteten Standard, welches auf dem Prinzip von RDF bzw. dem bereits erwähnten Prinzip von Linked Data basiert. 

-----

## Vergleich MARC21 und Dublin Core
Dublin Core ist ein Standard, der im Gegensatz zu MARC21 weit über die Bibliothekswelt hinaus angewandt wird und in der Welt der Informationswissenschaft als kleinster gemeinsamer Nenner gilt. Der Standard beschränkt sich auf 15 Datenfelder, diese tragen sprechende Namen. Dublin Core ist damit besser menschenlesbar als MARC21, dafür können in MARC21 dank dessen verschachtelten Struktur spezifischere Angaben erfasst werden. In der Veranstaltung haben wir die beiden Standards noch etwas genauer miteinander verglichen, die Ergebnisse sind im [gemeinsamen Dokument](https://pad.gwdg.de/EC9WU7DITxiK1ciMll3ZOw#) zu finden. 
Hinweis: Datenformate und Regelwerke unterscheiden sich dahingehend, als dass Regelwerke die theoretische Grundlage für die Katalogisierung bildet, während das Datenformat die praktische Repräsentation des Katalogisates erlaubt. 

-----

## Bibliothekssystem Koha
Im Anschluss an die Metadatenstandards sahen wir uns noch gemeinsam das open source System Koha an. Mit einem Demo-Account konnten wir uns selbst ins System einloggen und einige Basisfunktionen ausprobieren. Besonders spannend fand ich das Open Source Geschäftsmodell: der Code von Koha steht unter einer GPL Lizenz, einer non-permissiven Lizenz, die besagt, dass alle Weiterentwicklungen und Verbesserungen der Software von allen Beteiligten ebenfalls unter den ursprünglichen Bedingungen zu lizenzieren sind und somit allen Beteiligten zu Gute kommt (Copyleft Prinzip).
