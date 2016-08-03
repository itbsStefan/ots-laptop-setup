[README.md](https://github.com/vonneudeck/ots-laptop-setup "zum Ursprungs online GitHub Repository")
[otsLaptopsBerlin.md](https://github.com/itbsStefan/ots-laptop-setup/blob/master/otsLaptopsBerlin.md "Open Tech School Berlin Laptops")

gesponserte Hardware für offline Kurse 
======================================

Für [Learners Meetups](http://www.meetup.com/de-DE/opentechschool-berlin) 
und andere Aktivitäten werden vorinstallierte Laptops bereitgestellt.
Diese sind mit etwa einheitlicher Software und Konfiguration zu versehen und hier zu Dokumentieren!


Laptopausstattung und Konfiguration
-----------------------------------

[OTS Berlin](http://discourse.opentechschool.org/c/chapters/berlin "Open Tech School Berlin discourse")
http://discourse.opentechschool.org/t/stand-laptops/1836

Bei der Installation wird der Benutzer otsadmin eingerichtet, ohne sudo-Rechte werden dann weitere Accounts angelegt.
Der learners ist ein Benutzer welcher sich automatisch nach dem Systemstart auf die Desktopoberfläsche anmelden sollte.
Dieser hat voreingestellt die Sprache Englisch (auch Ordnernamen sind so für diesen in der Sprache), als zweiten Benutzer ist der User deutsch für ein deutschsprachigen Desktop.
Die Sprache kann jedoch beim Anmelden auf belibige vorinstallierten Sprachen umgestellt werden.
(dazu muss man als automatisch englischprachigen learners sich abmelden)
Beide Benutzer haben aus praktischen Gründen ein gleiches Passwort welches den Rechnernamen in Kleinbuchstaben entspricht.  


| Nr.  | Rechnername         | Benutzername     | Passwort          | abweichende Installation                     |   |   |   |
|------|---------------------|------------------|-------------------|----------------------------------------------|---|---|---|
| #001 | (hier nachtragen)   |                  |                   | nur Ubuntu ohne Partition                    |   |   |   |
| #002 | Suffragetten        | deutsch learners | ots  suffragetten |                                              |   |   |   |
| #003 | Arbeiter            | deutsch learners | ots  arbeiter     |                                              |   |   |   |
| #004 | Mechandros          | deutsch learners | ots  mechandros   |                                              |   |   |   |
| #005 | Studenten           | deutsch learners | ots  studenten    | bisher kein Laptop mit Installation begonnen |   |   |   |
| #006 | KalendarischerOrden |                  |                   | bisher kein Laptop mit Installation begonnen |   |   |   |


### Partitionierung der Festplatte
  ist noch hier nachzutragen

### Softwareausstattung 

 1. Ubuntu 14.04.4 LTS (Trusty Tahr)
 2. Linux Mint Qiana 17

### Installation mit OS Softwarerepository
[Standard software for an OTS machine](http://discourse.opentechschool.org/t/standard-software-for-an-ots-machine/1779 "Bitte aus den Seiten der OpentechSchool discourse hier her übertragen!")
  * GCompris
  * eToys
  * TuxPaint
...

### andere Softwarepakete mit URL Angabe
Beispiel zur Installation:
<code>
$ sudo add-apt-repository ppa:danielrichter2007/grub-customizer  
$ sudo apt-get update  
$ sudo apt-get install grub-customizer  
</code>
  * grub-customizer  ppa:danielrichter2007/grub-customizer

