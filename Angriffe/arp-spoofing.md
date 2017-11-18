# ARP-Spoofing
Autor: Daniel Nagel
Datum: 28.11.2017

### Ziel:
* Abgreifen von Passwörtern, Daten und übernahme von Sessions
### Bedingung:
* Nur innerhalb des selben Netzwerkes möglich.


### Address Resolution Protocol (ARP)
Das **ARP** ist ein **Netzwerkprotokoll**, das zu einer Netzwerkadresse *(IP-Adresse)* der Internetschicht *(OSI-Schicht 3)* die physikalische Adresse *(MAC-Adresse)* der Netzzugangsschicht *(OSI-Schicht 2)* ermittelt und diese Zuordnung in den ARP-Tabellen der beteiligten Rechner hinterlegt. Soll dann ein Datenpaket an ein IP-Adresse gesendet werden, kann in der ARP-Tabelle überprüft werden welche MAC-Adresse für diese hinterlegt wurde, um das Datepaket an die richtige Netzwerkschnittstelle zu senden. Dieses Protokoll wird hauptsächlich im Zusammenhang mit **IPv4-Adressierung** verwendet.


### ARP-Spoofing Funktionsweise
Damit ein Angreifer innerhalb des selben Netzwerkes den Datenverkehr zwischen zwei Hosts abhören kann, sendet der Angreifer eine manipulierte ARP-Nachricht an die Hosts. Das heißt das der Angreifer die hinterlegte MAC-Adresse für die IP-Adressen in den ARP-Tabellen des jeweils anderen Hosts gegen seine eigene Austauscht, um vortäuschen zu können das es sich beim Angreifer um einen der Hosts handelt. So wird der gesamte Datenverkehr über den Angreifer geleitet. Der Angreifer arbeitet unbemerkt als Proxy. Dieser Angriff ist ein Man-In-The-Middle-Angriff.
Das folgende Schaubild erläutert diesen Angriff nochmal:

![ARP-Spoofing](http://2we26u4fam7n16rz3a44uhbe1bq2.wpengine.netdna-cdn.com/wp-content/uploads/120711_2318_VLANHacking1.png)
