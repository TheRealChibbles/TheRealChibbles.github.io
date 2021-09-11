# Das Blinken aus dem Nichts

In diesem Blog wollen wir aufzeigen wie man ein Mikrokontrollerprojekt von Grund auf aufbaut. Dabei wird der Programmcode auf dem PC entwickelt, compiliert , gelinked und anschließend auf den Mikrokontroller geschrieben. Wir werden jeden Schritt zu dem fertigen Projekt dokumentieren und erklären. Dabei beschreiben wir auch wie der Programmcode geschrieben werden muss, damit der Mikrokontroller ordnungsgemäß startet. 

## Aufbau
### Hartware
### Weichware

## Das Problem
* Was passiert beim starten des Mikrokontrollers
  * Hartwarenregister werden auf ihren initialwert gesetzt
  * Achtung wird auf den Programmzähler gerichtet
  * Wo liegt der Code
  * Vektortabelle
  * Unterbrechungsanfragenbearbeitenden
  * Das Programm wird im besten Falle vollständig ausgeführt
* Wie schreiben wir das Startprogramm in anbetracht der vorherigen Probleme?
  * Vektortabelle
    * Stapeladresse wird definiert
    * Name (passendes pronomen) Neustartbearbeitenden 
    * mögliche definition weiter* Unterbrechungsanfragenbearbeitende 
  * (passendes Pronomen einfügen) Neustartbearbeitende
    * Daten werden vom nicht flüchtigen Speicher in den flüchtigen Speicher kopiert
    * ein bestimmter Teil des flüchtigen Speichers wird mit nullen beschrieben
    * Haupt wird aufgerufen
  * Konfiguration des nicht flüchtigen Speichers
* übersetzen
* Verbinden und zusammesetzen
* das große Úberschreiben

## Wie lassen wir unsere Lampe blinken?
* Wie können wir Hartwaren befehle erteilen
  * Register
  * Adressen
  * Datenblatt
* Hartwarenverhalten
  * Signalweiche
  * Ein- und Ausgabennadeln für allgemeine Verwendungen
  * (passendes Pronomen) Uhr
  * (passendes Pronomen) Wachhund
* Hartwarenkontrolle durch (?p) Weichware
  * Treiber
  * aufruf des Treibers
