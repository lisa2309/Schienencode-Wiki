## Einarbeitung 
Zum Einarbeiten wurde ein Timer erstellt, der auf allen Clients Synchronisiert wird. In Mirror wird mit einem Server Client Prinzip gearbeitet. Zudem wird eine Klasse benötigt die einem leeren Gameobjekt zugeordnet wird und von der Klasse NetworkManager erbt. Außerdem wird eine weitere Klasse benötigt, die von NetworkBehavior erbt und dem Spieler zugeordnet wird. 

## Client
Am Anfang wird ein Spieler Gameobjekt erzeugt. Dieses wird so konfiguriert, dass man über das Internet mit dem Server kommunizieren kann. Hierfür muss das Spieler Gameobjekt über eine Network Identity Komponente verfügen. 
Wenn sich ein Spieler mit dem Spiel verbindet, wird für diesen ein eigenes Gameobjekt erstellt. Dieser Spieler hat nun ein zugehöriges Gameobjekt, welches Mirror importiert und wodurch es nun möglich ist, dass dieser mit dem Server kommuniziert. 

## Server
Bevor der Server eingerichtet werden kann, muss er zunächst erzeugt werden. Hierzu wird nur ein Gameobjekt benötigt, dass über drei folgenden Komponente verfügen muss:

1. Network Manager
2. KCP Transport
3. Network Manager HUD

### Wie man in Zukunft den Server einrichten könnte:
- Die Spieleranzahl muss definiert werden
- Die IP-Adresse des Hosts/Servers muss eingerichtet werden
- Der Verbindungsport 7777 muss eingerichtet werden
- Zudem muss entschieden werden, wie der Server mit afk (away from keyboard) Spielern umgeht. Wird die Verbindung zu diesem Spieler unterbrochen oder nicht? 
- Die Authentifikation der Spieler am Server (user, password)   

