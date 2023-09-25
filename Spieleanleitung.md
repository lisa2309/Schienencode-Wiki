Inhaltsverzeichnis
- [Grundlagen](#grundlagen)
- [Ziel des Spiels](#ziel-des-spiels)
- [GUI](#gui)
- [Missionen](#missionen)
- [Bahnhöfe](#bahnhöfe)
- [Schienen platzieren und löschen](#schienen-platzieren-und-löschen)
- [Besondere Schienen](#besondere-schienen)

## Grundlagen

Willkommen im Spiel "Schienencode". Dieses Lernspiel dient der Vertiefung und Anwendung erlernter Kontrollstrukturen aus der Programmierung. 

## Ziel des Spiels

Ziel des Spiels ist es, den Zug vom Start bis zum Ende fahren zu lassen und dabei alle angezeigten Missionen abzuschließen. Um Missionen abzuschließen kann der Spieler Schienen platzieren und löschen, Weichen stellen und die Anzahl der Ladungen, die an einem Bahnhof abgeholt werden können, ändern.

## GUI

![gui_legende](uploads/e226ba89c0850c7b7c58475db286e85c/gui_legende.png)   
1: Missionsfenster    2: Löschmodus    3: Zug starten    4: Lautstärke    5: Hilfemenü    6: Schienenelemente 

## Missionen

Missionen sind der Schlüssel zum Sieg! Erreicht der Zug das Ende, bevor alle Missionen abgeschlossen sind, zählt dies als Niederlage.
Die abzuschließenden Missionen und der aktuelle Fortschritt werden an der linken Seite des Bildschirms angezeigt. 

## Bahnhöfe

Dreh- und Angelpunkt der Missionen sind Bahnhöfe. Dies sind die Gebäude, die verteilt am Streckenrand stehen. Ein Linksklick auf ein solches Gebäude offenbart ein Popup-Menü. Hier kann man einstellen, wie viel Liefergut von diesem Bahnhof eingesammelt werden soll, wenn der Zug daran vorbei fährt. Allerdings kann man nur begrenzt viel auf einmal einladen. Vielleicht kann man ja beim nächsten Besuch mehr abholen...?   
![mission_no_prog](uploads/c11dbf8ffa82ad92084abb3270812d57/mission_no_prog.png) ![Bahnhof](uploads/42c807c4666766a40a2ed2ab89dc8e88/Bahnhof.png) ![bahnhof_dropdown](uploads/d997d8a255d009b8cae28353a9ae67f3/bahnhof_dropdown.png) ![mission_prog](uploads/86e7e26dbefcde259de78cf4a7085117/mission_prog.png)

## Schienen platzieren und löschen

Natürlich ist nicht jede Strecke von Anfang an perfekt. Manchmal kann es vorkommen, dass die vorgegebene Strecke unvollständig ist. Dann liegt es am Spieler, die Strecke zu vervollständigen.   
Die Auswahl der Schienen erstreckt sich über den gesamten unteren Bildschirmrand. Hier kann zwischen Geraden, Kurven, Tunneln, Sammelschienen und Weichen ausgewählt werden.   
![Schienen](uploads/6bfce71388c7c1364202dd59a60e9596/Schienen.png)
Hat sich der Spieler für ein Schienenelement entschieden, erscheint noch ein kleines Popup. Hier kann man das gewählte Element noch im oder gegen den Uhrzeigersinn rotieren und die Auswahl mit dem Häkchen bestätigen.
Wenn man jetzt die Maus über den Bildschirm bewegt, kann man bereits an einer kleinen Vorschau sehen, wo das gewählte Element platziert wird. Ist man mit der Position zufrieden, kann man die Schiene mit Rechtsklick platzieren.
Ist man mit der gewählten Position doch nicht so zufrieden, wie man vor der Platzierung dachte, ist das kein Grund zur Panik. Mit dem Mülleimer-Button am oberen Bildschirmrand kann man jederzeit selbst platzierte Schienen wieder mit Linksklick löschen. Vom Spiel vorgegebene Schienen sind nicht löschbar!   
![lösch_inaktiv](uploads/f6b1031da0f217a68dc4d171c01aad4b/lösch_inaktiv.png)
*Löschmodus aus*   
![lösch_aktiv](uploads/a5f5e01991f2459f91c3c9df6213e003/lösch_aktiv.png)
*Löschmodus ein*

***Aber Achtung: Man kann im Löschmodus zwar weiterhin mit Rechtsklick Schienen platzieren, allerdings ist es nicht möglich, mit Bahnhöfen oder Weichen zu interagieren!***

## Besondere Schienen

Die Funktionen der meisten Schienen sind ziemlich selbsterklärend. Geraden und Kurven geben einfach nur die Strecke und Fahrtrichtung vor und Sammelschienen führen zwei verschiedene Strecken zueinander. Ein paar andere Schienen sind vielleicht nicht für jeden auf den ersten Blick eindeutig oder verstecken noch zusätzliche Funktionen...

### Start- und Zielschiene

Der Name ist ziemlich eindeutig. Vom Start fährt der Zug los und am Ziel soll er ankommen. Nur das Aussehen sollte einmal verdeutlicht werden. Nicht dass eine Strecke mal rückwärts gebaut wird...   
![start](uploads/cb36cce603864ad449bc62445a37a718/start.png) ![ziel](uploads/8c6ee047a9fac291d20f2c02225762ba/ziel.png)

### Tunnel

Tunnel helfen dabei, einen Zug schnell von einem Punkt zu einem anderen zu transportieren und symbolisieren zusätzlich sogenannte "Jumps", wie man sie aus dem Programmieren kennt.
Es gibt jeweils einen Ein- und Ausgangstunnel, die separat platziert werden können. 
Mit beiden Tunneln kann mit Linksklick interagiert werden. Der Ausgangstunnel wird dann mitteilen, dass er ein Ausgang ist und zusätzlich eine kurze Kennung anzeigen. Diese ist dem Eingangstunnel wichtig, denn bei ihm kann man festlegen zu welchem Ausgang er führt. Dabei können mehrere Eingänge zum selben Ausgang führen, allerdings kann ein Eingang nicht mehrere Ausgänge haben.   
![t_out_popup](uploads/dca89b8e27f95419eba66aa0654188b4/t_out_popup.png) ![t_in_popup](uploads/19d9e0b27ce1047b5bab2b254bfa8475/t_in_popup.png)

### Weichen

Weichen können vom Spieler platziert werden, um die Fahrtrichtung des Zuges festzulegen.   
![switch](uploads/9491d7f4593d3e068cab8f6dbf651897/switch.png)
*Achtung Verwechslungsgefahr: Weichen sehen Sammelschienen sehr ähnlich*

Nach der Platzierung einer Weiche hat diese erstmal keine Funktion. Dies lässt sich mit einem Linksklick beheben. Es erscheint ein Popup, bei dem man sich für einen von drei Typen entscheiden muss.   
![SwitchPopUp](uploads/230a18f7148b149eff8c7cb0318b382d/SwitchPopUp.png)   
*Es gibt 3 Typen: If-, While- und For-Weichen*

**If- und While-Weichen**   
In der aktuellen Version des Spiels haben If- und While-Weichen noch dieselbe Funktion, es ist jedoch denkbar in Zukunft mithilfe weiterer Prüfungen bei einer While-Weiche zumindest zu unterscheiden, ob diese auch wirklich wie vorgesehen durchlaufen wurde, oder vor einer Umkehrung der Bedingung bereits verlassen wurde.   
Bei diesen Weichen wird kontrolliert, wie viel eines ausgewählten Ladungstyps der Zug im Moment der Überfahrt transportiert. Ist die festgelegte Bedingung wahr, biegt der Zug ab. Ist sie falsch, fährt er weiter geradeaus.   
![IfSwitch](uploads/acfed72510263a05a9fca9b9f60cfb50/IfSwitch.png) ![WhileSwitchPopUp](uploads/722320bd6f0effea5a759e8e8681042c/WhileSwitchPopUp.png)   
*Aktuell dieselbe Funktion: If- und While-Weichen*

**For-Weichen**   
Bei einer For-Weiche wird mitgezählt, wie oft der Zug diese Weiche passiert hat. Solange die Anzahl unter der angegebenen liegt, biegt der Zug ab. Ist sie erreicht, fährt er geradeaus.   
![ForSwitchPopUp](uploads/ff2c0cb35786126e15215f65b5d6c986/ForSwitchPopUp.png)