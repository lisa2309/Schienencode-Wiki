Es gibt noch einige Ideen die wir für das Spiel hatten, jedoch nicht umsetzen konnten. Diese Ideen sind hier festgehalten für das zukünftige Entwicklerteam. 

### Spielidee:
* Ein eigenständiges Tutorial
* Die Züge sollen in bestimmter Reihenfolge bei den Bahnhöfen eintreffen (Pünktlichkeit gewährleisten).
* Die Züge müssen mit den Bahnhöfen interagieren und auf Fahrgäste warten. Dies muss auch vom Spieler definiert werden.
* Es gibt Passagiere oder Ladungen mit bestimmten Eigenschaften (Gewicht, Dauer beim Einsteigen etc.)
* Berücksichtigung von Wetter- oder Umwelteinflüssen.
* Ein Punktesystem anstatt nur "gewonnen" und "verloren"
* Ein integrierter Timer -> Für die Schnelligkeit gibt es Bonuspunkte
* Züge haben Wagons und man muss die Ladung interaktiv in den Wagon laden
* Es gibt mehrere Züge, die verschiedene Farben haben und auch verschiedene Missionen besitzen. Diese muss man über die Kontrollstrukturen verschieden fahren lassen
* Mehrere verschiedene Level pro Schwierigkeitsgrad

### Spielbrett: 
* Es sollen als Kontrollstrukturen auch Schranken zugelassen werden, die einen wechselseitigen Ausschluss ermöglichen (erst sinnvoll, wenn mehrere Züge gleichzeitig fahren oder Umwelteinflüsse berücksichtigt werden müssen). 
* Die verschiedenen Spielbretter werden nicht nur händisch implementiert, sondern teilweise auch computergeneriert, um so mehr Abwechslung zu gewährleisten.
* Es könnten noch Hindernisse eingebaut werden.
* Es könnten Berge und Brücken hinzugefügt werden, da dies in unserem [Routenberechnung](Routenberechnung) Skript schon vorgesehen sind.
* Während der Zug über die verschiedenen Felder der Spieler fährt, soll die Kamera dem Zug folgen, damit dieser permanent sichtbar bleibt.
* Die Vorschau zu den potenziell erstellbaren Schienen sollte deaktiviert werden können.
* Das Spielbrett sollte bereits zu Beginn ausgewählt werden können.

### Fehlererkennung:
* Wenn Spielbretter nicht aus der Datenbank geladen werden können, soll eine Fehlermeldung erscheinen, die möglichst genau auf die Ursache des Ladeabbruchs hinweist (ungültige Definition des Spielbretts, Verbindungsabbruch, kein Zugriffsrecht etc.)
* Ein Raum ohne Spieler sollte erkannt und geschlossen werden.
* Wenn Spieler im Wartebereich die Verbindung verlieren, soll dies erkannt werden und die entsprechenden Spieler sollen aus der aktuellen Spielerliste entfernt werden.

### Alternativen zu Fehlermeldungen: 
* Es soll eine kurze Kollisionsanimation gestartet werden, sobald der Zug die Schienen verlässt und der Spieler hat das Spiel verloren
* Nach einer bestimmten Zeit das Spiel abgebrochen und der Spieler hat das Spiel verloren
* Wenn es im kooperativen Modus nicht gelingt einen Streckenabschnitt in den eines anderen Spielers zu überführen, wird an der entsprechenden Stelle erneut die Kollisionsanimation gestartet und alle Spieler haben das Spiel verloren.
* Eingesetzte Schienenteile, dessen Verhalten nicht mehr rechtzeitig vom Spieler definiert wurde, werden als defekte Schienenteile dargestellt und führen beim Überqueren durch einen Zug zu einer Kollisionsanimation. Der Spieler hat das Spiel verloren.

* Führt ein Tunnel ins nichts, vernimmt man ein bedrückendes Schreien. Der Spieler hat das Spiel verloren.


### Spielmodi:
* Weiterer Spielmodus: Im kompetitiven Spielmodus treten die Spieler gegeneinander an, anstatt miteinander. Hierbei besitzt jeder die gleiche Karte, damit es fair gestaltet ist
* Einen Einzelspielermodus
* Einen Mehrspielermodus für 3 und 4 Spieler

### Mirror
Ideen wie man in Zukunft den Server einrichten könnte, finden sie bei [Mirror](Mirror). 