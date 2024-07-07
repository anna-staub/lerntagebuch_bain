---
title: "Suchmaschinen und Discovery Systeme 1"
date: 2024-05-21
---
Dieser Blogbeitrag fasst die Inhalte der elften Lehrveranstaltung des Moduls "Bibliotheks- und Archivinformatik" zusammen. Die Veranstaltung fand am 21. Mai 2024 statt und trug den Titel "Suchmaschinen und Discovery Systeme 1".
Der Blogbeitrag zur vorherigen Lehrveranstaltung "Schnittstellen nutzen" ist [hier](https://anna-staub.github.io/lerntagebuch_bain/2024/05/08/metadaten_schnittstellen_2_schnittstellen.html) zu finden, der Beitrag zur folgenden Lehrveranstaltung "Suchmaschinen und Discovery Systeme 2" [hier](https://anna-staub.github.io/lerntagebuch_bain/2024/06/03/suchmaschinen_discovery_systeme_2.html).

-----

# Inhalte der Lehrveranstaltung
- Discovery Systeme
- VuFind
- Solr
- Vergleich einer Suche in VuFind und Solr

-----

## Discovery Systeme
Unter einem Discovery System versteht man ein bibliothekarisches Suchsystem, das auf Suchmaschinentechnologien basiert. Discovery Systeme sind eine moderne Alternative zu den klassischen Bibliothekskatalogen. Während klassische Bibliothekskataloge möglichst genaue Ergebnisse liefern, liefern Discovery Systeme sehr viele Suchergebnisse, die, wie dies auch bei anderen Suchmaschinen der Fall ist, mit Hilfe eines Algorithmus nach Relevanz sortiert werden. Discovery Systeme bestehen aus einer Suchmaschine, in der alle Katalogeinträge indexiert werden, und einer Oberfläche, in der die Nutzenden ihre Suchanfragen eingeben. Die Oberfläche leitet die Anfrage an die Suchmaschine weiter, erhält von dieser eine Ergebnisliste zurück und bereitet diese grafisch auf für die Nutzenden.

-----

## VuFind
VuFind ist ein solches Discovery System. Es wurde in PHP geschrieben und basiert auf der Solr-Suchmaschine, auf die im nächsten Abschnitt noch eingegangen wird. Das System ermöglicht den Nutzenden eine umfassende Suche und Navigation durch (bibliografische) Datenbanken. Der Ablauf einer Suche mit VuFind funktioniert so, dass VuFind eine HTTP-Anfrage an Solr sendet, welches JSON-Daten zurücksendet. Aus diesen erstellt VuFind eine nutzerfreundlich dargestellte Trefferliste. Bibliotheken können VuFind in ihre Website integrieren, aber auch bibliotheksübergreifende Dienste wie z.B. Swisscovery arbeiten mit VuFind.

-----

## Solr
Solr ist eine weit verbreitete, sehr leistungsfähige Suchmaschine, die in Systeme wie VuFind integriert werden kann. Ein prominentes Beispiel, welches Solr als Suchmaschine verwendet, ist Netflix. Die Suche mit Solr funktioniert so, dass das System die eingegebenen Wörter auf ihre Grundform zurückführt (stemming), so dass auch nach weiteren Varianten der Wörter gesucht und damit mehr Ergebnisse gefunden werden. Auch Tippfehler kann die Suchmaschine korrigieren. 

-----

## Vergleich einer Suche in VuFind und Solr
Während der Veranstaltung haben wir die Benutzeroberflächen der Demoversionen von VuFind und Solr verglichen - wobei angemerkt werden muss, dass die Oberfläche von Solr nur zu Demonstrationszwecken dient. Solr hat entspreched eine etwas weniger benutzerfreundliche, eher technisch gestaltete Admin-Oberfläche, während VuFind offensichtlich mehr auf die Endnutzerinnen ausgerichtet ist und eine benutzerfreundlichere Oberfläche mit mehr Optionen (zitieren, exportieren etc) bietet. VuFind erstellt ausserdem bereits während der Eingabe Suchvorschläge, was darauf hindeutet, dass bereits während der Eingabe Suchabfragen durchgeführt werden.

