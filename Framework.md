Im Laufe des Projekts hat die Einbindung des Frameworks wiederholt für Probleme gesorgt, weswegen wir uns gegen die Einbindung entschieden haben.   
Dennoch wollten wir eine gewisse Grundlage schaffen, die das Einbinden vereinfachen wird, sollte jemand das später umsetzen wollen.

Wir bedienen uns der vom Framework vorgegebenen Files *GameServer*, *SimpleJSON* und *ServerLoadingScene*.

In der Klasse GameServer wurden mithilfe von JSON-Dateien folgende Werte Hard gecodet erstellt, um:
* den Spielername
* die Spieleranzahl
* die Rundenanzahl und
* die anfangs Szene 
zu speichern.   

        private void LoadPlayerInfoMockup() 
        {    
            isHost = true;

            playerInfos = new JSONObject();
            gameInfos = new JSONObject();

            playerInfos.Add("name", "Mustermann");
            gameInfos.Add("playerAmount", 2);
            gameInfos.Add("rounds", 6);
            gameInfos.Add("board", "marin");
       }

Die ServerLoadingScene wird aufgrund von Konflikten mit anderen Scenes in der jetztigen Version nicht verwendet.