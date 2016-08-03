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
| #001 | OTS_BLN             | coop             | coop              | nur Ubuntu ohne Partition                    |   |   |   |
| #002 | (hier nachtragen)   | coup             | coup              | nur Ubuntu ohne Partition                    |   |   |   |
| #003 | Suffragetten        | deutsch learners | ots  suffragetten |                                              |   |   |   |
| #004 | Arbeiter            | deutsch learners | ots  arbeiter     |                                              |   |   |   |
| #005 | Mechandros          | deutsch learners | ots  mechandros   |                                              |   |   |   |
| #006 | KalendarischerOrden |                  |                   | bisher kein Laptop mit Installation begonnen |   |   |   |
| #007 | Studenten           | deutsch learners | ots  studenten    | bisher kein Laptop mit Installation begonnen |   |   |   |


### Partitionierung der Festplatte

  Sofern es die Größe der internen Festplatte erlaubt wäre eine Unterteilung in Patition angebracht.
  Der Standard GPT gegenüber MS-Dos Patition MBR wäre dem Vorzug zu geben auch ist dieser künftig bei ein UEFI-Boot Standard.

| Nr | Patition Funktion              | Name               | Größe      | Format | Mount in | Flags  |   |
|----|--------------------------------|--------------------|------------|--------|----------|--------|---|
| 01 | Grub                           | hiddenGrubpatition | 1-10 MB    |        |          |        |   |
| 02 | Boot                           | bootpatition       | 50-512 MB  | ext2   | /boot    |        |   |
| 03 | Operating System 1             | ubuntupart         | 32 GB      | ext3   | /        |        |   |
| 04 | Operating System 2             | mintpart           | 32 GB      | ext3   | /        |        |   |
| 05 | Offline & OS independend Space | otsMaterials       | 32 GB      | ext3   | /opt     |        |   |
| 06 | preinstalled Apache or similar | forInstalledApps   | <32 GB     | ext3   | /srv     |        |   |
| 07 | Swap                           | swap               | 4 GB       | swap   | swap     |        |   |



### Softwareausstattung 

 1. Ubuntu 14.04.4 LTS (Trusty Tahr)
 2. Linux Mint Qiana 17
 3. nach dem Projekt lernstick mit eigenen Anpassungen

### Installation mit OS Softwarerepository
[Standard software for an OTS machine](http://discourse.opentechschool.org/t/standard-software-for-an-ots-machine/1779 "Bitte aus den Seiten der OpentechSchool discourse hier her übertragen!")
  * GCompris
  * eToys
  * TuxPaint
  * Testdrive (Tool for HDs)
  * Synaptic
...

### andere Softwarepakete mit URL Angabe
Beispiel zur Installation:
<pre><code>
$ sudo add-apt-repository ppa:danielrichter2007/grub-customizer  
$ sudo apt-get update  
$ sudo apt-get install grub-customizer  
</code></pre>
  * grub-customizer  ppa:danielrichter2007/grub-customizer


