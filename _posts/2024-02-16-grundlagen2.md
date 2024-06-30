---
title: "Technische Grundlagen 2/2"
date: 2024-02-16
---
Dieser Blogbeitrag behandelt die Inhalte der zweiten Lehrveranstaltung des Moduls "Bibliotheks- und Archivinformatik". Die Veranstaltung fand am Nachmittag des 14. Februar 2024 statt und trug den Titel "Technische Grundlagen 2".
Den Beitrag zur vorhergehenden Lehrveranstaltung, welche am gleichen Tag am Vormittag stattfand, ist [hier](/2024-02-15-grundlagen1.md) zu finden.
Den Beitrag zur nachfolgenden Veranstaltung zum Thema "Funktion und Aufbau von Bibliothekssystemen" ist [hier](/2024-02-27-bibliothekssysteme.md) zu finden.

-----

# Inhalte der Lehrveranstaltung
- Codespaces: Time-Out Zeit erhöhen
- Grundlagen der Unix Shell
- Versionskontrolle mit Git
- Lerntagebuch mit GitHub Pages

-----

## Codespaces: Time-Out Zeit erhöhen
Die Einführung in die GitHub Codespaces wurde im ersten Blogpost beschrieben. In der zweiten Veranstaltung lernten wir dazu noch, wie man die Time-Out Zeit erhöht, sodass sich die Codespaces nicht wie per default nach 30 Minuten Inaktivität selbst beenden, sondern erst nach 240 Minuten.

-----

## Grundlagen der Unix Shell
Um die Grundlagen der Unix Shell kennenzulernen oder zu repetieren, lösten wir in eigenem Tempo Aufgaben der Library Carpentry Lessons zur Unix Shell unter Verwendung der GitHub Codespaces. Obwohl ich viele Shell-Befehle bereits einmal kennengelernt hatte, tat mir die Auffrischung sehr gut, da ich sich in der Zwischenzeit doch einiges wieder aus meinem Gedächtnis verflüchtigt hatte. So gelang mir z.B. die Navigation in der Shell auf Anhieb, die Arbeit mit Dateien und Befehlen wie less, mv oder history hingegen eher harzig. Da war ich froh, dass wir einige Übungen dazu ausführen konnten. Das Zählen und Durchsuchen von Dateiinhalten sowie das Sortieren von Dateien nach bestimmten Kriterien war mir neu.
Ein Befehl, den ich mir herausgeschrieben habe, ist ctrl+c zum Beenden jeglicher Prozesse in der Shell. Praktische Cheatsheets für die wichtigsten Befehle sind:
-	[Library Carpentry Reference](https://librarycarpentry.org/lc-shell/reference.html)
-	[Cheatsheet für Linux](https://devhints.io/linux)
-	[Cheatsheet für Shell-Skripte](https://devhints.io/bash)

-----

## Versionskontrolle mit Git
Im vorherigen Blogpost habe ich erwähnt, dass GitHub ein Internetdienst ist, der auf der Versionierungssoftware Git basiert. Was genau ist denn Git?
Git ist eine open-source Software, die von Linus Thorwald für die gemeinsame Softwareentwicklung entwickelt wurde. Mit Git können alle Arten von Textdateien (Code, Plain-Text, csv...) von mehreren Computern oder Personen bearbeitet und versioniert abgespeichert werden. Jedes Mal, wenn man eine Änderung an einer Datei vornimmt und diese als Commit abspeichert, wird eine neue Version der Datei abgespeichert. Man kann dann jeweils von der neusten Version aus weiterarbeiten, kann aber auch ältere Commits bearbeiten, weitere Branches erstellen und Branches und Änderungen wieder zusammenführen. Git funktioniert lokal auf einem Computer, man kann aber Git Repositorien auch im Netz bereitstellen, mit Hilfe von Plattformen wie eben GitHub oder auch GitLab. Die Repositorien können somit lokal und online synchronisiert werden.
Ein typischer Workflow bei open-source Projekten mit Git besteht daraus, dass man ein Repository, zu dem man etwas beitragen möchte, "forkt", also eine Kopie des Repositorys erstellt. In dieser Kopie arbeitet man dann unabhängig vom Ausgangsrepository. Ist man fertig mit der Bearbeitung erstellt man einen Pull Request, eine Anfrage an die Betreiber des Ausgangsrepositorys, um die eigenen Änderungen in das ebendieses aufzunehmen.

-----

## Lerntagebuch mit GitHub
Das Lerntagebuch, welches Sie gerade lesen, wurde ebenfalls mit GitHub erstellt. Es besteht aus einem Repository mit Markdown Dateien, wovon jede Datei einen Blogpost enthält. Das Repository wurde von einer Vorlage des Dozenten geklont und von mir mit Blogposts befüllt.
