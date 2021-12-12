# DE3: Ich kann VPN mittels Metadata konfigurieren

# Cloud-Init
In unsrem Fall werden die VPN Informationen für das Wireguard im Cloud-Init Script mitgegeben. 
Jedoch ist auf dem lernMAAS eine Konfiguration schon installiert die es ermöglicht durch ein (- und eine Zahl) bei der Benennung einer VM die VPN IP für diese VM zu vergeben. Doch zuerst muss die VM zu einem AZ hinzugefügt werden, das ermöglicht der VM die WireGuard Konfiguration zu übernehmen. 
Man muss jedoch aufpassen die Nummer 01 ist schon für den Gateway reserviert.

# Cloud Metadata
Jede Cloud gibt Metadaten zur Verfügung das sind z.B Cloud Region, Computer Name, Betriebssystem und noch vieles mehr. Diese Daten können benutzt werden um z.B das VPN einzurichten.
