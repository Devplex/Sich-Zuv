# Penetrationstest - DOS
Autor: Devin-A. Meier

Datum: 21.11.17

### Ziel:
* Lahm legen eines Dienste zB Website eines Hosts damit auf diese nicht mehr zugegriffen werden kann
### Tools:
* hping3
* LOIC(Low Orbit Ion Cannon), HOIC, XOIC

### DOS - Denial of Service
engl. für „Verweigerung des Dienstes“ bezeichnet in der Informationstechnik die Nichtverfügbarkeit eines Internetdienstes, der eigentlich verfügbar sein sollte. Obwohl es verschiedene Gründe für die Nichtverfügbarkeit geben kann, ist die häufigste Art die Folge einer Überlastung des Datennetzes. Dies kann durch unbeabsichtigte Überlastungen verursacht werden oder durch einen konzentrierten Angriff auf die Server oder sonstige Komponenten des Datennetzes. Im Fall einer durch eine Unmenge von Anfragen verursachten Dienstblockade spricht man von einer durch Vielanfragen verbreiteten Verweigerung des Dienstes.

### Funktionsweise
Bei einem DOS-Angriff werden von einem Angreifer infizierte Systeme benutzt um ein gezieltes System mit sovielen Anfragen zu 'bombardieren', dass dieses die Anfragen nicht mehr verarbeiten kann und der Server abstürzt und keine Anfragen von normalen Usern mehr annehmen kann. Man kann den Angriff mit Tools wie hping3 oder LOIC sehr einfach ausführen.

