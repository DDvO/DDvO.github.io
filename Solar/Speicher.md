---
title: "Batteriespeicher - Mini-Solaranlagen für daheim und unterwegs"
description: >-
  Online-Artikel von Dr. David von Oheimb
  mit wichtigen Hintergrund-Infos zum Thema Photovoltaik und
  vielen praktischen Tipps für Balkonkraftwerke und andere kleine Solar-Anlagen,
  einschließlich Hinweisen,
  welche Komponenten und Verwendungsformen sich unter welchen Umständen lohnen:
  exakte Simulationsergebnisse für Rentabilität, optimale Modul-Ausrichtung und
  die Verwendung von Wechselrichtern und Speicherbatterien inklusive Regelung.
created: ", erstellt in März 2022"
changed: ", letzte Änderung: "
lang: de
---

# (Gesamt-)Inhaltsverzeichnis {#Inhaltsverzeichnis}

-   [Hauptseite mit Zusammenfassung etc.](index.md)
-   [Photovoltaik und ihr möglicher Ertrag](PV.md)
-   [Stromverbrauch und Einspeisung im Haushalt](SV.md)
-   [Eigenverbrauch und seine Berechnung](EV.md)
-   [Nutzungsvarianten](SSG.md)
    -   [Direkte Netzeinspeisung (Steckersolargerät SSG, „Balkonkraftwerk“)](SSG.md#SSG)
    -   [Hausnetzeinspeisung mit Pufferspeicher](#Batteriespeicher)
        - [Lade-Kopplung des Speichers](#Kopplung)
        - [Regelungsstrategien für PV-Speicher](#Regelungsstrategien)
        - [Dimensionierung des Stromspeichers](#Dimensionierung)
        - [Kommerzielle SSG-Speicherlösungen](#kommerziell)
          - [Effizienzbetrachtung](#Effizienz)
        - [SSG-Speicherlösungen im Eigenbau](Speicher-Eigenbau.md)
    -   [Inselanlage (mit Speicherung) und Kombination](Insel.md)
-   [Auswahl und Nutzung von Komponenten](Komp.md)
-   [Beispiel-Konfigurationen](Bsp.md)

## Hausnetzeinspeisung mit Pufferspeicher {#Batteriespeicher}

![Bild: Balkonkraftwerk mit Pufferbatterie und Inselwechselrichter](
Pufferbatterie_und_Inselwechselrichter.png){:.right width="400"
style="margin-left: 40px"}
Statt den Solarstrom direkt einzuspeisen, kann man ihn auch in einer aufladbaren
Batterie zwischenspeichern und von dort zeitlich versetzt über einen
[netzgekoppelten Wechselrichter](Komp.md#Netzwechselrichter) ins Hausnetz einspeisen.
Diese Betriebsart kann man allgemein als *Strompufferung* bezeichnen.

Für die Auslastung eines Speichers gibt es eine Kennzahl, die von der
Kapazität des Speichers abstrahiert, nämlich die Zahl der *Vollzyklen*
in einem Zeitraum, typischerweise ein Jahr.
Sie ist definiert als die Menge, das in dem Zeitraum insgesamt aus dem
Speicher entnommen wird (nachdem sie natürlich vorher irgendwann eingespeichert
wurde), geteilt durch seine nutzbare Kapazität
(also bei LiFePO4-Batterien z.B. 90% der Nennkapazität).
Bei typischen Dach-PV-Anlagen mit üblicher Dimensionierung des Speichers liegt
die Zahl der Jahres-Vollzyklen bei etwa 200.
Aber je nach Größe der PV-Anlage und des Speichers sowie der zeitlichen
Verteilung von Ertrag und Verbrauch kann die Zyklenzahl auch
deutlich höher oder niedriger sein, z.B. 300 oder 100.
Bei einem Wert von 183 wird die verfügbare Speicherkapazität im Jahresschnitt
alle zwei Tage verwendet --- was aber nicht heißt, dass der Speicher im Schnitt
jeden zweiten Tag erst mal voll aufgeladen und dann wieder ganz entladen wird.

Die Strompufferung soll den Nutzen der PV-Anlage für den eigenen Stromverbrauch
erhöhen. Aber **finanziell lohnt sie sich für kleine PV-Anlagen fast nie** ---
außer wenn sie über eine nahezu optimale (lastgesteuerte)
[Lade- und Entladeregelung](#Regelungsstrategien) verfügt und man den
Speicher sehr günstig bekommt oder schon aus anderen Gründen hat, z.B. für
eine Notstromversorgung (mit Inselwechselrichter) oder als Fahrzeugbatterie.
Außerdem ist es für die ökologische Gesamtbilanz eigentlich besser, den
überschüssigen Strom an die Allgemeinheit (auch ohne Vergütung) abzugeben.

<!-- https://www.mydealz.de/comments/permalink/46085250 -->
In diesem Zusammenhang wird von Anbietern und Nutzer oft eine
naive (Milchmädchen-)Rechnung in folgender Art gemacht:
> Der Speicher hat eine nutzbare Kapazität von 1,5&nbsp;kWh und 6000 Ladezyklen. Damit lassen sich also 9000&nbsp;kWh einsparen, was bei 30&nbsp;ct/kWh 2700€ Ertrag bringt.

Das berücksichtigt aber keine Verluste und vor allem nicht, wie lange
es dauern würde, um auf die (angeblich erreichbare) Zyklenzahl zu kommen.
Pro Jahr hat man nur mäßig viele sonnige Tage, so dass man typischerweise auf
nur 150 bis 250 Vollzyklen im Jahr kommt, je nach PV-Leistung, Verbrauch und
Speicher-Dimensionierung. Somit werden 6000 Vollzyklen erst in ungefähr 30
Jahren erreicht, und so lange wird das Speicher-Equipment bestimmt nicht halten!
Zudem beträgt bei 30 Jahren Laufzeit die Rendite bei einem Einkaufspreis von
1500€ nur 6%, so dass man sich fragen muss, ob sich so eine Investition mit
sehr langfristiger Kapitalbindung überhaupt lohnt.
Wobei auch unklar ist, wie sich das Verhältnis
des Preises für so eine Speicheranlage zum Strompreis langfristig entwickelt.

Besser sieht es bei größeren PV-Anlagen aus.
<!-- https://www.mydealz.de/comments/permalink/44464786 -->
Hier das Ergebnis von Simulationen für ein Wohnhaus mit angenommenen 5000&nbsp;kWh
Jahresverbrauch und 200&nbsp;W Mindestlast und ansonsten typischem Lastprofil,
optimal ausgerichteter PV-Anlage in Süddeutschland mit 10&nbsp;kWp,
mit einem kleinen Speicher mit effektiv 2&nbsp;kWh
und typischen Verlusten/Wirkungsgraden.
Nehmen wir Einspeisevergütung und 30 - 8 = 22&nbsp;ct/kWh Strompreisdifferenz​ an.

* Wenn der Speicher <!--AC-gekoppelt ist und--> optimal lastabhängig geladen und
entladen wird, dann steigt der PV-Eigenverbrauch von 2020​ auf 2746​&nbsp;kWh im Jahr,
was bei den 22&nbsp;ct/kWh Strompreisdifferenz etwa 160€/Jahr Einsparung ausmacht.
<!--Bei einem [Eigenbau](Speicher-Eigenbau.md) mit günstigen Komponenten, die insgesamt 1000€ kosten, -->
Bei Systemen, die 1000€ kosten, amortisiert sich das nach gut 6 Jahren.
* Bei ansonsten gleichen Daten, aber 4&nbsp;kWh nutzbarer Speicherkapazität
steigt der Eigenverbrauch auf 3308&nbsp;kWh im Jahr, was 283€ Einsparung pro Jahr
bringt und bei 1500€ Kosten eine Amortisationszeit von knapp 6 Jahren bringt.
* Bei 6&nbsp;kWh Kapazität steigt der Eigenverbrauch noch etwas weiter auf 3734&nbsp;kWh,
bei 8&nbsp;kWh Kapazität auf 3988&nbsp;kWh, wobei sich Amortisationszeit kaum ändert.

<!--
* Wenn der Speicher AC-gekoppelt ist und optimal (also nur mit PV-Überschuss)
geladen, aber einfach zwischen 19 und 5 Uhr konstant mit 200&nbsp;W entladen wird,
dann steigt durch die Nachteinspeisung
der PV-Eigenverbrauch von 2020​ auf immerhin 2650​&nbsp;kWh im Jahr.
-->
<!--
./Solar.pl Lastprofil_17_teils_31.csv 5000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 10000  -peff 92 -tmy -load min 124 7:0..24 -capacity 2000 -max_charge 100 -max_discharge 100 -feed 200 19..5
Lastprofil-Datei            : Lastprofil_17_teils_31.csv
Nächtliche Durchschnittslast=  349 W von 0 bis 6 Uhr
Minimallast (Grundlast)     =  200 W am *-01-01 um 00:00
Maximallast                 =17762 W am *-12-03 um 14:44

PV-Daten-Datei              : Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv
Neigungswinkel, Azimut      = 35°, 0°
Breitengrad, Längengrad     = 48.215, 11.727
Simuliertes PV-Jahr         : TMY (2008..2020)

PV-Nennleistung             =10000 Wp
Max. PV-Bruttoleistung      =10087 W am TMY-04-15 um 13h
PV-Bruttoertrag             =12721 kWh
PV-DC-Ertrag                =11703 kWh, PV-System-Wirkungsgrad 92%
PV-Nettoertrag              =11001 kWh bei Wechselrichter-Wirkungsgrad 94%
Max. PV-Nettoleistung       = 8724 W am TMY-04-15 um 13h

Verbrauch                   = 5000 kWh über ein Jahr
Adaptierte minimale Last    =  200 W

Speicherkapazität           = 2000 Wh mit max. Ladehöhe 100%, max. Entladetiefe 100%, AC-gekoppelt
Optimale Ladestrategie (nicht gebrauchte Energie), max. Laderate 1 C
Konstanteinspeisung         =  200 W von 19 bis 5 Uhr, max. Entladerate 1 C
Verlust durch Überlauf      =    0 kWh weil AC-gekoppelt
Ladeverlust                 =   45 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =   35 kWh durch Speicher-Wirkungsgrad 95%
Verlust mit AC-Kopplung     =   40 kWh durch Entlade-WR-Wirkungsgrad 94%
PV-Nutzung über Speicher    =  624 kWh
Netzeinspeisung via Speicher= 3.18 kWh
max. Ladehöhe               = 2000 Wh am TMY-01-01 um 10:08
Zwischenspeicherung         =  703 kWh nach Ladeverlust
Vollzyklen                  =  351 (der effektiven Kapazität 2000 Wh)

PV-Eigenverbrauch           = 2650 kWh
Netzeinspeisung             = 8231 kWh
PV-Eigenverbrauchsanteil    =   24 % des PV-Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =   53 % des Verbrauchs (Autarkiegrad)
-->

<!--
* Wenn aber kein lastgeregeltes Überschussladen verwendet wird, sondern der
Einfachheit halber ein DC-gekoppeltes Ladegerät mit Bypass bei vollem Speicher,
das der Speicherladung Priorität gibt,
und Konstanteinspeisung mit 200&nbsp;W (was hier besser ist als nur Nachteinspeisung),
dann steigt der Eigenverbrauch von 2020 nur auf 2490&nbsp;kWh im Jahr,
was bei 22 ct/kWh Strompreisdifferenz nur etwa 103€/Jahr Einsparung ausmacht.​
Ohne lastabhängige Regelung zieht sich also (trotz etwas weniger Kosten für die
Komponenten) die Amortisation deutlich länger hin.
-->
<!--
./Solar.pl Lastprofil_17_teils_31.csv 5000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 10000  -peff 92 -tmy -load min 124 7:0..24 -capacity 2000 -max_charge 100 -max_discharge 100 -feed 200 -pass spill 0 -dc
Speicherkapazität           = 2000 Wh mit max. Ladehöhe 100%, max. Entladetiefe 100%, DC-gekoppelt
Speicher-Umgehung           =    0 W und für Überschuss, max. Laderate 1 C
Konstanteinspeisung         =  200 W, max. Entladerate 1 C
Verlust durch Überlauf      =    0 kWh
Ladeverlust                 =  102 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =   80 kWh durch Speicher-Wirkungsgrad 95%
Verlust während Entladung   =  691 kWh durch Entlade-WR-Wirkungsgrad 94%
PV-Nutzung über Speicher    =  920 kWh
Netzeinspeisung via Speicher=  512 kWh
max. Ladehöhe               = 2000 Wh am TMY-01-01 um 10:07
Zwischenspeicherung         = 1604 kWh nach Ladeverlust
Vollzyklen                  =  802 (der effektiven Kapazität 2000 Wh)
TODO Simulation-Fehler durch gleichzeitiges Laden und Entladen

PV-Eigenverbrauch           = 2496 kWh
Netzeinspeisung             = 8333 kWh
PV-Eigenverbrauchsanteil    =   21 % des PV-DC-Ertrags (Nutzungsgrad)
Eigendeckungsanteil         =   50 % des Verbrauchs (Autarkiegrad)
--->

Im Folgenden werden konkrete Zahlen gegeben für einen Haushalt mit 3000&nbsp;kWh
Jahresverbrauch (bei nächtlicher Durchschnittslast von 190&nbsp;W zwischen 0 und
6&nbsp;Uhr und tagsüber Durchschnittslast von 375&nbsp;W zwischen 8 und 16 Uhr)
mit einer typischen Balkonanlage in Süddeutschland mit optimal ausgerichteten
Modulen mit 850&nbsp;Wp Nennleistung und typischen Wirkungsgraden, der eine
Pufferbatterie mit 1&nbsp;kWh effektiv nutzbarer Kapazität hinzugefügt wurde.
Dazu passt sehr gut eine 25,6&nbsp;V 50&nbsp;Ah LiFePO4-Batterie,
also mit nominell 1,28&nbsp;kWh Kapazität, denn davon muss man ohnehin
mindestens 90% für eine gesunde Entladetiefe abziehen, und nochmal ungefähr 90%
für die durchschnittliche Degradation durch Alterungseffekte etc. Die
Eigenverbrauch-Ergebnisse wurden mit dem [o.g. SolBatSim](EV.md#SolBatSim) berechnet,
unter Annahme einer (effizienteren) [DC-Kopplung](#Kopplung)
mit Lade-Wirkungsgrad 94% und Speicherungs-Wirkungsgrad 95%.
Wie zuvor sind für den Wirkungsgrad des PV-Systems 92% angenommen
und für die Wechselrichtung (auch bei Entladung aus der Batterie) 94%.

Bei [optimaler Lade-/Entlageregelung, s.u.](#Regelungsstrategien) <!--,
die leider nur schwer zu realisieren ist,--> gibt es keinen Verlust durch Überlauf
des Speichers, und anstatt dass der PV-Überschuss von ca. 310&nbsp;kWh komplett
ins Netz eingespeist wird, kommt es nur noch zu 84&nbsp;kWh Netzeinspeisung.
Hinzu kommen kleine Verluste des Ladereglers und der Speicherbatterie
von etwa 14 + 11&nbsp;kWh. Durch die Verwendung des Speichers lässt sich somit
der jährliche Eigenverbrauch von ca. 610 auf etwa 810&nbsp;kWh und
der Eigenverbrauchsanteil von ca. 66 auf etwa 83% des Nettoertrags steigern.
Der PV-Bruttoertrag von 1062&nbsp;kWh bzw. Nettoertrag 918&nbsp;kWh wird also
gut genutzt. Der Speicher mit effektiv 1&nbsp;kWh Kapazität
ist mit ca. 225 Vollzyklen pro Jahr nur mäßig belastet.
Bei 30&nbsp;ct/kWh Strompreis ergibt sich durch die Hinzunahme des Speichers
eine jährliche Stromkosten-Einsparung von ca. 60€.

Selbst wenn die dafür nötigen Komponenten günstig für z.B. 600€ erworben werden,
würde die Amortisationszeit für die Aufrüstung etwa 10 Jahre betragen --
eher länger. Allerdings kann es sein, dass in dieser Zeitspanne bereits ein
Teil der nötigen Geräte erneuert werden muss. Vor Allem aber ist für kleine
PV-Anlagen eine optimale Regelung im [Eigenbau](Speicher-Eigenbau.md) schwer erreichbar,
<!--und auch eine Annäherung daran unverhältnismäßig aufwendig.-->
während [kommerzielle Lösungen](#kommerziell)) Stand Anfang 2026 noch zu teuer sind.

<!--
./Solar.pl Lastprofil_17_teils_31.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 850 -peff 92 -tmy
Lastprofil-Datei            : Lastprofil_17_teils_31.csv
Nächtliche Durchschnittslast=  189 W von 0 bis 6 Uhr
Tagsüber Durchschnittslast  =  375 W von 8 bis 16 Uhr

PV-Nennleistung             =  850 Wp
Max. PV-Bruttoleistung      =  920 W am TMY-03-23 um 12h
PV-Bruttoertrag             = 1062 kWh
PV-DC-Ertrag                =  977 kWh, PV-System-Wirkungsgrad 92%
PV-Nettoertrag              =  918 kWh bei Wechselrichter-Wirkungsgrad 94%
Max. PV-Nettoleistung       =  796 W am TMY-03-23 um 12h

Verbrauch                   = 3000 kWh über ein Jahr
PV-Eigenverbrauch           =  610 kWh
PV-Überschuss               =  309 kWh
Max. PV-Überschuss          = 4.05 kWh am TMY-03-24
Netzeinspeisung             =  309 kWh
PV-Eigenverbrauchsanteil    =   66 % des PV-Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =   20 % des Verbrauchs (Autarkiegrad)

./Solar.pl Lastprofil_17_teils_31.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 850 -peff 92 -tmy -dc -max_charge 100 -max_discharge 100 -capacity 1000

Speicherkapazität           = 1000 Wh mit max. Ladehöhe 100%, max. Entladetiefe 100%, DC-gekoppelt
Optimale Ladestrategie (nicht gebrauchte Energie), max. Laderate 1 C
Optimale Entladestrategie (so viel wie gebraucht), max. Entladerate 1 C
Verlust durch Überlauf      =    0 kWh
Ladeverlust                 =   14 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =   11 kWh durch Speicher-Wirkungsgrad 95%
Verlust während Entladung   =   57 kWh durch Entlade-WR-Wirkungsgrad 94%
PV-Nutzung über Speicher    =  201 kWh
Netzeinspeisung via Speicher=    0 kWh
max. Ladehöhe               = 1000 Wh am TMY-01-15 um 14:28
Zwischenspeicherung         =  225 kWh nach Ladeverlust
Vollzyklen                  =  225 (der effektiven Kapazität 1000 Wh)

PV-Eigenverbrauch           =  810 kWh
Netzeinspeisung             =   84 kWh
PV-Eigenverbrauchsanteil    =   83 % des PV-DC-Ertrags (Nutzungsgrad)
Eigendeckungsanteil         =   27 % des Verbrauchs (Autarkiegrad)
-->

Wenn man dieselben PV-Daten verwendet wie der [Stecker-Solar-Simulator der
HTW Berlin](https://solar.htw-berlin.de/rechner/stecker-solar-simulator/),
kommt man mit gleichen Speicher-Daten und einem ähnlichen Lastprofil
sowohl beim [Stecker-Solar-Simulator](EV.md#HTW)
als auch beim [PVTool](EV.md#PVTool) auf
[nahezu identische Ergebnisse](https://github.com/nick81nrw/PVTools/issues/58).

<!--
https://www.akkudoktor.net/pvtool-rechner/ Systemverluste PV: 14,5%
D-16356 Lindenberg, Ahrensfelde, Barnim, Brandenburg 52.6023748,13.524606
Lastprofil_3000_Haushalt_05-PVTool.csv

|Speicher|SolBatSim| HTW | PVTool |
|-------:|--------:|----:|-------:|
|   0 Wh |   480   | 490 | 437 kWh|
| 500 Wh |   610   | 613 | 610 kWh|
|1000 Wh |   680   | 685 | 680 kWh|
|1500 Wh |   725   | 723 | 724 kWh|
|2000 Wh |   754   |  -  | 753 kWh|
|3000 Wh |   775   |  -  | 771 kWh|
|4000 Wh |   777   |  -  | 773 kWh|
|5000 Wh |   777   |  -  | 773 kWh|
-->

<!--
./Solar.pl Lastprofile/Lastprofil_3196_Haushalt_05.csv 3000 Timeseries_Lindenberg_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 850 -only 2017 -curb 600 # -capacity 1250 -dc
Lastprofil-Datei            : Lastprofile/Lastprofil_3196_Haushalt_05.csv
Nächtliche Durchschnittslast=  160 W von 0 bis 6 Uhr
Minimallast (Grundlast)     =   38 W am *-02-21 um 00:12
Maximallast                 =24260 W am *-10-23 um 14:12

PV-Daten-Datei              : Timeseries_Lindenberg_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv
Neigungswinkel, Azimut      = 35°, 0°
Breitengrad, Längengrad     = 52.604, 13.524
Simuliertes PV-Jahr         : 2017

PV-Nennleistung             =  850 Wp nur während 2017
Max. PV-Bruttoleistung      =  853 W am 2017-04-30 um 11h
PV-Bruttoertrag             =  944 kWh
PV-DC-Ertrag                =  864 kWh, PV-System-Wirkungsgrad 91%
PV-Netto-Ertragsverlust     = 7.15 kWh während 167 h durch WR-Ausgangs-Drosselung auf 600 W
PV-Nettoertrag              =  805 kWh bei Wechselrichter-Wirkungsgrad 94%
Max. PV-Nettoleistung       =  600 W am 2017-02-16 um 12h

Verbrauch                   = 3000 kWh nur während 2017
PV-Eigenverbrauch           =  480 kWh
PV-Eigenverbrauchsverlust   = 0.41 kWh netto während 14 h durch WR-Ausgangs-Drosselung auf 600 W
Netzeinspeisung             =  326 kWh
PV-Eigenverbrauchsanteil    =   60 % des PV-Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =   16 % des Verbrauchs (Autarkiegrad)

https://solar.htw-berlin.de/rechner/stecker-solar-simulator/
2 * 300 Wp Module ohne Batteriespeicher
Stromerzeugung pro Jahr 820 kWh
Vermiedener Strombezug pro Jahr 490 kWh
Nutzungsgrad 60 %
Selbstversorgung 16 %
-->
<!--
./Solar.pl Lastprofile/Lastprofil_3196_Haushalt_05.csv 3000 Timeseries_Lindenberg_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 850 -only 2017 -curb 600 -max_charge 100 -max_discharge 100 -dc -capacity 1000
./Solar.pl Lastprofile/Lastprofil_3196_Haushalt_05.csv 3000 Timeseries_Lindenberg_SA2_850Wp_crystSi_14_35deg_0deg_2017.csv 850 -curb 600 -max_charge 100 -max_discharge 100 -dc -capacity 1000

Speicherkapazität           = 1250 Wh mit max. Ladehöhe 90%, max. Entladetiefe 90%, DC-gekoppelt
Optimale Ladestrategie (nicht gebrauchte Energie), max. Laderate 1 C
Optimale Entladestrategie (so viel wie gebraucht), max. Entladerate 1 C
Verlust durch Überlauf      =    0 kWh
Ladeverlust                 =   14 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =   11 kWh durch Speicher-Wirkungsgrad 95%
Verlust während Entladung   =   50 kWh durch Entlade-WR-Wirkungsgrad 94%
PV-Nutzung über Speicher    =  201 kWh
Netzeinspeisung via Speicher=    0 kWh
max. Ladehöhe               = 1125 Wh am 2017-01-27 um 12:24
Zwischenspeicherung         =  225 kWh nach Ladeverlust
Vollzyklen                  =  225 (der effektiven Kapazität 1000 Wh)

PV-Eigenverbrauch           =  680 kWh
PV-Eigenverbrauchsverlust   = 0.18 kWh netto - nur näherungsweise - während 6 h durch WR-Ausgangs-Drosselung auf 600 W
Netzeinspeisung             =  108 kWh
PV-Eigenverbrauchsanteil    =   79 % des PV-DC-Ertrags (Nutzungsgrad)
Eigendeckungsanteil         =   23 % des Verbrauchs (Autarkiegrad)

PV-Eigenverbrauchsanteil    =   84,4 % des PV-Nettoertrags (Nutzungsgrad)

https://solar.htw-berlin.de/rechner/stecker-solar-simulator/
2 * 300 Wp Module mit Batteriespeicher
Stromerzeugung pro Jahr 820 kWh
Vermiedener Strombezug pro Jahr 685 kWh
Nutzungsgrad 83 %
Selbstversorgung 23 %
-->

Eine wichtige Rolle spielt natürlich die Verteilung des Haushalts-Verbrauchs
über den Tag. Im o.g. typischen Fall ergab sich bei Durchschnittslast von
375&nbsp;W zwischen 8 und 16&nbsp;Uhr und Durchschnittslast von 190&nbsp;W
zwischen 0 und 6&nbsp;Uhr durch den Speicher ein Jahresgewinn von 200&nbsp;kWh.\
Wenn stattdessen die Durchschnittslast tagsüber nur 100&nbsp;W beträgt und
nachts 234&nbsp;W, dann steigt der Gewinn durch den Speicher auf 270&nbsp;kWh.\
Wenn andererseits die Durchschnittslast tagsüber sogar 600&nbsp;W beträgt und
nachts 124&nbsp;W, dann sinkt der Gewinn durch den Speicher auf 180&nbsp;kWh.

<!--
./Solar.pl Lastprofil_17_teils_31.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 850 -peff 92 -tmy -dc -max_charge 100 -max_discharge 100 -capacity 1000 -bend 1,1,1,1,2,2,2,2,.295,.295,.295,.295,.295,.295,.295,.285,2,2,2,2,1,1,1,1
Nächtliche Durchschnittslast=  234 W von 0 bis 6 Uhr
Tagsüber Durchschnittslast  =  100 W von 8 bis 16 Uhr

Speicherkapazität           = 1000 Wh mit max. Ladehöhe 100%, max. Entladetiefe 100%, DC-gekoppelt
Optimale Ladestrategie (nicht gebrauchte Energie), max. Laderate 1 C
Optimale Entladestrategie (so viel wie gebraucht), max. Entladerate 1 C
Verlust durch Überlauf      =    0 kWh
Ladeverlust                 =   17 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =   14 kWh durch Speicher-Wirkungsgrad 95%
Verlust während Entladung   =    0 kWh durch Entlade-WR-Wirkungsgrad 94%
PV-Nutzung über Speicher    =  242 kWh
Netzeinspeisung via Speicher=    0 kWh
max. Ladehöhe               = 1000 Wh am TMY-01-10 um 12:27
Zwischenspeicherung         =  271 kWh nach Ladeverlust
Vollzyklen                  =  271 (der effektiven Kapazität 1000 Wh)

PV-Eigenverbrauch           =  566 kWh
PV-Überschuss               =  594 kWh
Max. PV-Überschuss          = 4.81 kWh am TMY-03-24
Netzeinspeisung             =  323 kWh
PV-Eigenverbrauchsanteil    =   58 % des PV-DC-Ertrags (Nutzungsgrad)
Eigendeckungsanteil         =   19 % des Verbrauchs (Autarkiegrad)
-->
<!--
./Solar.pl Lastprofil_17_teils_31.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 850 -peff 92 -tmy -dc -max_charge 100 -max_discharge 100 -capacity 1000 -bend 1,1,1,1,1,1,1,1,2.45,2.45,2.45,2.45,2.45,2.45,2.44,2.44,1,1,1,1,1,1,1,1
Nächtliche Durchschnittslast=  124 W von 0 bis 6 Uhr
Tagsüber Durchschnittslast  =  600 W von 8 bis 16 Uhr

Speicherkapazität           = 1000 Wh mit max. Ladehöhe 100%, max. Entladetiefe 100%, DC-gekoppelt
Optimale Ladestrategie (nicht gebrauchte Energie), max. Laderate 1 C
Optimale Entladestrategie (so viel wie gebraucht), max. Entladerate 1 C
Verlust durch Überlauf      =    0 kWh
Ladeverlust                 =   11 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             = 8.95 kWh durch Speicher-Wirkungsgrad 95%
Verlust während Entladung   =    0 kWh durch Entlade-WR-Wirkungsgrad 94%
PV-Nutzung über Speicher    =  160 kWh
Netzeinspeisung via Speicher=    0 kWh
max. Ladehöhe               = 1000 Wh am TMY-03-15 um 11:03
Zwischenspeicherung         =  179 kWh nach Ladeverlust
Vollzyklen                  =  179 (der effektiven Kapazität 1000 Wh)

PV-Eigenverbrauch           =  877 kWh
PV-Überschuss               =  201 kWh
Max. PV-Überschuss          = 3.63 kWh am TMY-03-23
Netzeinspeisung             =   22 kWh
PV-Eigenverbrauchsanteil    =   90 % des PV-DC-Ertrags (Nutzungsgrad)
Eigendeckungsanteil         =   29 % des Verbrauchs (Autarkiegrad)
-->

### Lade-Kopplung des Speichers {#Kopplung}

Die Anbindung eines Speichers zum Laden über eine PV-Anlage erfolgt
entweder *DC-gekoppelt*, also schon gleichstromseitig,
oder *AC-gekoppelt*, also indirekt über das Wechselstromnetz im Haushalt.

{:style="clear:both"}

![Bild: DC-Kopplung](DC-Kopplung.jpg){:.left width="408"
style="margin-right: 2px"}
![Bild: AC-Kopplung](AC-Kopplung.jpg){:.right width="380"
style="margin-left: 2px"}
<!--
https://selecta-solar.de/stromspeicher/
https://solar.htw-berlin.de/effizienzleitfaden-fuer-pv-speichersysteme/
-->

{:style="clear:both"}

Das Laden der Batterie erfolgt am besten möglichst direkt aus der PV-Anlage
über einen [Solar-Laderegler](Komp.md#Laderegler), also per [*DC-Kopplung*](
https://www.photovoltaikforum.com/core/article/7-pv-und-batteriespeicher-besser-ac-oder-dc-gekoppelt/),
weil der Gleichstrom der PV-Module nicht umständlich und mit Zusatz-Verlusten
zwischendurch in Wechselstrom und dann wieder zurück gewandelt wird.
Ein weiterer Vorteil ist, dass der Speicher auch bei Stromausfall mit PV-Strom
geladen werden kann, was (in Zusammenhang mit einem Inselwechselrichter)
zu Verlängerung der Notstromfähigkeit führt.
Dem steht der Nachteil gegenüber, dass relativ dicke Gleichstromkabel bis zum
Standort des Speichers geführt werden müssen.

<!-- Man braucht also entweder eine
spezielle Leitung ins Haus oder muss den Speicher außerhalb platzieren, wobei zu
bedenken ist, dass LiFePO4-Batterien bei Minustemperaturen nicht geladen werden
dürfen, wobei man da mit einer thermostatgeregelten Heizmatte abhelfen kann. -->
Um eine DC-Verkabelung ins Haus zu vermeiden, kann man Laderegler, Speicher
und Wechselrichter auch im Freien (z.B. auf dem Balkon oder in einem Schuppen)
platzieren. Damit die Anlage dann auch bei Minustemperaturen nutzbar ist, wo
[Lithium-basierte Batterien nicht geladen werden sollten](
https://www.ipowerqueen.de/blogs/batteriewissenschaft/warum-ist-der-schutz-vor-niedrigen-temperaturen-fur-lithiumbatterien-wichtig),
sollte der Speicher mit einer Heizung versehen sein.
<!--[Kommerzielle DC-gekoppelte Lösungen](#kommerziell) für kleine PV-Anlagen wie
Balkonkraftwerke sind leider allesamt nicht rentabel. -->

Bei *AC-Kopplung* wird der PV-Strom zunächst ins Wechselstromnetz
eingespeist, so dass die Ladung (an einem beliebigen Ort, meist im Haus)
mit einem 230&nbsp;V-Ladegerät geschieht, wobei man zur Entladung einen zweiten
(Batterie-)Wechselrichter benötigt.
Ihr besonderer Vorteil ist eine große Flexibilität bei der Wahl der Komponenten,
auch bzgl. eines späteren Ausbaus und der Betriebsspannung der Komponenten,
weil die Batteriespannung von der Systemspannung der PV-Anlage unabhängig ist.
Außerdem kann man den Speicher bei Bedarf (z.B. wenn er zu leer geworden ist
oder zu Testzwecken) auch unabhängig von der PV-Anlage mit Netzstrom laden.\
Eine AC-Kopplung ist allerdings technisch umständlicher als eine DC-Kopplung
und hat einen schlechten Gesamt-Wirkungsgrad: etwa 75 bis 80%.

### Regelungsstrategien für PV-Speicher {#Regelungsstrategien}

Weil man für ins externe Netz eingespeisten Strom keine Vergütung bekommt oder
jedenfalls deutlich weniger erhält als man für vom Netz bezogenen Strom zahlen
muss, sollte zur Strom-Kostenersparnis
die Einspeisung vermieden und der Netzbezug minimiert werden.\
Daher wäre es es optimal, wenn zu jeder Zeit gilt:

<p style="text-align: center;">
Haushalts-Last + Auflade-Leistung in den Speicher
</p>
<p style="text-align: center;">
≥
</p>
<p style="text-align: center;">
PV-Leistung + Entlade-Leistung aus dem Speicher
</p>

Nachdem der Gesamt-Leistungssaldo am externen Netzanschluss des Haushalts gleich

<p style="text-align: center;">
(Haushalts-Last + Speicher-Aufladeleistung) −
(PV-Leistung + Speicher-Entladeleistung)
</p>

ist, kann die Ungleichung auch abgekürzt geschrieben werden als

<p style="text-align: center;">
Gesamt-Leistungssaldo ≥ 0
</p>

Wenn die Ungleichung erfüllt ist, dann wird trotz PV-Leistung
überhaupt kein Strom ins Netz eingespeist (sondern höchstens bezogen).

Wenn die PV-Leistung nie größer als die Last durch den Haushalt wäre,
bräuchte man dafür keinen Speicher, aber das ist nicht realistisch.
Mit Hilfe des Speichers kann die Ungleichung immerhin viel öfter erfüllt
werden als ohne, indem bei PV-Leistungsüberschuss der Speicher aufgeladen
und bei Mehrbedarf durch Last im Haushalt der Speicher entladen wird.

Aus der o.g. Regelungs-Ungleichung folgt nebenbei, dass es
nicht zielführend wäre, den Speicher gleichzeitig zu laden und zu entladen.
Das ist auch schon physikalisch-technisch gar nicht möglich.
Bei ungeschickter Laderegelung eines AC-gekoppelten Speichers könnte es aber
passieren, dass sowohl das Ladegerät als auch der Wechselrichter zur Entnahme
aus dem Speicher aktiv ist. Dies führt dazu, dass je nach Differenz aus Lade-
und Wechselrichter-Leistung der Speicher entweder geladen oder entladen wird
und dass das Minimum der beiden Leistungen sinnlos und mit Verlusten
zunächst in Gleichstrom und umgehend wieder in Wechselstrom gewandelt wird.

Für die Regelung wird die PV-Leistung und normalerweise auch die Last durch
den Haushalt als gegeben vorausgesetzt. Allerdings könnte die Regelung
durchaus gewisse [Überschuss-Verbraucher](SV.md#Stromverbrauch) steuern.
Als die wesentlichen Stellschrauben der Regelung bleibt die Lade- und
Entladeleistung des Speichers. \
Unter Berücksichtigung, dass ein Speicher mit gegebener Kapazität nur begrenzt
geladen und entladen werden kann und sich Laden und Entladen des Speichers
zeitlich ausschließen, ergibt sich folgende ideale Lade- und Entladeregelung:

* Solange der Speicher nicht voll ist,
wird immer genau der Anteil an PV-Leistung zum Laden verwendet, der übrig ist,
also aktuell nicht anderweitig direkt gebraucht werden kann.\
Dies wird *Lastvorrang* oder *Überschussladung* genannt.

* Solange sein [Ladezustand](Komp.md#Ladezustand) oberhalb der Entladegrenze ist,
wird der Speicher immer genau so stark entladen wie nötig ist, um den Anteil der
aktuellen Last auszugleichen, den die PV-Leistung nicht abdeckt.

Damit kann man eine sogenannte *Nulleinspeisung*
realisieren, also dass überschüssiger Strom nicht ins externe Netz fließt.
Bei vollem Speicher kann man aber auch einen *Bypass* erlauben, also dass
die gesamte PV-Leistung an der Batterie vorbei ins Hausnetz gespeist wird.
Dies geschieht bei AC-Kopplung automatisch,
weil bei vollem Speicher das Ladegerät abschaltet.
Durch den Bypass bei vollem Speicher wird überschüssiger Strom nach extern
abgegeben, solange die Last geringer als PV-Leistung ist.

Bei AC-Kopplung ist die Maximalleistung einer bedarfsgerechten Ausspeisung aus
dem Speicher übrigens ziemlich unerheblich. Etwa bei einem Jahresverbrauch von
3000&nbsp;kWh zeigen Simulationen, dass selbst wenn sie auf nur 100&nbsp;W begrenzt wird,
das für die Speichernutzung und den Eigenverbrauch so gut wie nichts ausmacht.
Daher genügt für AC-gekoppelte Pufferspeicher ein kleiner Wechselrichter.

In teilweiser Abweichung von den bisher genannten Punkten sollten zur Schonung
der Batteriezellen gewisse Lade- und Entladeströme nicht überschritten werden,
wobei die verwendeten Komponenten da ohnehin Grenzen setzen.
Außerdem ist die Reaktionsgeschwindigkeit der Lade- und Entladeregelung
aus verschiedenen Gründen begrenzt,
so dass es kurzzeitig z.B. zu unerwünschter Netzeinspeisung kommen kann.
Auch lassen sich Lastspitzen meist nicht ausgleichen.
Durch solche Randbedingungen leidet die Effizienz ein wenig.

Ein 'intelligentes' Energiemanagement berücksichtigt auch noch diverse weitere
Faktoren, etwa Uhrzeit, Sonnenstand, Temperatur, die bisherige Entwicklung
der PV-Leistung, der Last und des Speicher-Ladezustandes, der in nächster Zeit
erwartete PV-Ertrag, Verbrauch im Haushalt, Strompreis, usw.

Die [Implementierung einer Speicher-Regelung](Speicher-Eigenbau.md#Regelungsimplementierung),
welche [lastbasiert](Speicher-Eigenbau.md#lastgeregelt) sein sollte, ist regelungstechnisch
ziemlich aufwendig. Sie lohnt sich finanziell bislang eher nur für
größere PV-Anlagen und (wegen der Speicherkosten) für nicht sehr große Speicher.

Statt einer lastabhängigen Regelung ist es besonders für Steckersolargeräte
viel einfacher, aber leider wenig effizient,
die (gedrosselte) Ausgangsleistung des Wechselrichters und die Batteriekapazität
so abzustimmen, dass lediglich ein Großteil der Grundlast des Haushalts,
z.B. 100&nbsp;W, für eine Dauer von etwa 1-2 Tagen abgedeckt wird.
Wenn man diese [*Konstanteinspeisung*](Speicher-Eigenbau.md#Konstanteinspeisung) noch mit einer
Zeitschaltuhr (oder einem Helligkeitssensor) zur Beschränkung zwischen
Sonnenunter- und Aufgang kombiniert, bekommt man eine *Nachteinspeisung*.\
Ziel der Konstanteinspeisung ist zwar, die über die sonnenreiche Tageszeit
gesammelte Solarenergie auch über sonnenarme Zeiten gleichmäßig abzugeben
(solange die Ladung reicht, zumindest bis zum nächsten Vormittag),
und dabei möglichst wenig Strom nach extern zu verschenken.
Allerdings zeigen [Simulationsergebnisse](Speicher-Eigenbau.md#Konstanteinspeisung),
dass sich auf diese Weise nicht mal die Grundlast effizient abdecken lässt.

![Bild: Wasserspeicher als Analogie](Wasserspeicher.jpg){:.right width="400"
style="margin-left: 50px; margin-right: 50px"}
Hier als Analogie eine Skizze eines automatischen Wasserspeichers,
der z.B. über die Dachrinne eines Hauses gespeist wird. Wenn er voll genug ist,
läuft das Wasser über die rechte innere Trennwand und lässt eine leichte Kugel
aufschwimmen, die bis dahin den Auslass blockiert hat. Dann fließt das
Wasser aus dem Speicher langsam und gleichmäßig nach unten aus.
Wenn der Speicher fast leer ist, verschließt die Kugel den Auslass wieder.
Der Speicher füllt sich (auch schon zwischendurch) bei Wasserzufuhr wieder auf.
Zusätzlich ist der Speicher am Einlass mit einem Überlaufschutz
ausgestattet, der die Wasserzufuhr stoppt, wenn der Speicher voll ist
und das Wasser durch den kleinen Auslass nicht schnell genug abfließt.

### Dimensionierung des Stromspeichers {#Dimensionierung}

Zum Thema *Stromspeicher* in verschiedensten Formen
und Nutzungsmöglichkeiten im Zusammenhang mit Photovoltaik
[hier ein ausführlicher Artikel](https://www.net4energy.com/de-de/stromspeicher)
und [hier](
https://www.wegatech.de/ratgeber/photovoltaik/stromspeicher/speicher-kennzahlen/)
eine gute Erklärung der wichtigsten Begriffe in diesem Zusammenhang,
z.B. der *Entladetiefe* und der *Zyklenanzahl*.

Die meisten Nutzer legen ihren PV-Speicher zu groß aus,
was unnötigen Materialaufwand und überzogene Kosten verursacht.
Die effektiv nutzbare Kapazität des Speichers sollte nur so groß sein, dass damit
der typische PV-Überschuss eines mäßig ertragreichen Sonnentages aufgenommen
und diese Strommenge meist bis zum nächsten Morgen sinnvoll genutzt werden kann.
Es lohnt sich dabei nicht, Tage mit besonders hohem Ertrag oder besonders starkem
Verbrauch zu berücksichtigen.
Eine genaue Optimierungs kann durch Simulationen mit verschiedenen Speichergrößen
unter Berücksichtigung des Haushalts-Lastprofils erfolgen.

Für das [o.g. Balkonkraftwerk-Beispiel](#Batteriespeicher) beträgt der tägliche
PV-Überschuss maximal etwa 4&nbsp;kWh und im Jahres-Durchschnitt 0,85&nbsp;kWh.
An ca. 130 Tagen beträgt er über 1&nbsp;kWh, an nur 50 Tagen über 2&nbsp;kWh,
und sogar nur an 5 Tagen über 3&nbsp;kWh.
Erst ab effektiv ca. 4&nbsp;kWh Speicherkapazität gibt es ein paar Tage,
wo der gespeicherte Strom über Mitternacht reicht.\
Mit effektiv 1&nbsp;kWh Speicherkapazität liegt bei optimaler Regelung
die Steigerung des jährlichen Eigenverbrauchs bei 200&nbsp;kWh.
Eine Erhöhung der nutzbaren Speicherkapazität auf 2&nbsp;kWh bringt nur noch
etwa 60&nbsp;kWh weitere Steigerung und lohnt damit den Speicher-Aufpreis nicht.
Hingegen brächte schon eine effektive Speicherkapazität auf 0,5&nbsp;kWh eine
Steigerung des Eigenverbrauchs von 140&nbsp;kWh.

Deutlich interessanter wäre die Speichernutzung bei Verdoppelung der PV-Leistung
auf 1700&nbsp;Wp. Dann brächte 1&nbsp;kWh Speicherkapazität bei optimaler
Regelung eine Steigerung des jährlichen Eigenverbrauchs von 300&nbsp;kWh,
und bei 2&nbsp;kWh effektiver Kapazität immerhin nochmal 170&nbsp;kWh mehr.

<!--
./Solar.pl Lastprofil_17_teils_31.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 1700 -peff 92 -tmy -dc -max_charge 100 -max_discharge 100 -capacity 2000
Lastprofil-Datei            : Lastprofil_17_teils_31.csv
Nächtliche Durchschnittslast=  189 W von 0 bis 6 Uhr
Minimallast (Grundlast)     =   10 W am *-06-15 um 05:22
Maximallast                 =11028 W am *-12-03 um 14:44

PV-Daten-Datei              : Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv
Neigungswinkel, Azimut      = 35°, 0°
Breitengrad, Längengrad     = 48.215, 11.727
Simuliertes PV-Jahr         : TMY (2008..2020)

PV-Nennleistung             = 1700 Wp
Max. PV-Bruttoleistung      = 1841 W am TMY-03-23 um 12h
PV-Bruttoertrag             = 2124 kWh
PV-DC-Ertrag                = 1954 kWh, PV-System-Wirkungsgrad 92%
PV-Nettoertrag              = 1837 kWh bei Wechselrichter-Wirkungsgrad 94%
Max. PV-Nettoleistung       = 1592 W am TMY-03-23 um 12h

Verbrauch                   = 3000 kWh über ein Jahr

Speicherkapazität           = 2000 Wh mit max. Ladehöhe 100%, max. Entladetiefe 100%, DC-gekoppelt
Optimale Ladestrategie (nicht gebrauchte Energie), max. Laderate 1 C
Optimale Entladestrategie (so viel wie gebraucht), max. Entladerate 1 C
Verlust durch Überlauf      =    0 kWh
Ladeverlust                 =   33 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =   26 kWh durch Speicher-Wirkungsgrad 95%
Verlust während Entladung   =    0 kWh durch Entlade-WR-Wirkungsgrad 94%
PV-Nutzung über Speicher    =  468 kWh
Netzeinspeisung via Speicher=    0 kWh
max. Ladehöhe               = 2000 Wh am TMY-01-10 um 13:53
Zwischenspeicherung         =  525 kWh nach Ladeverlust
Vollzyklen                  =  262 (der effektiven Kapazität 2000 Wh)

PV-Eigenverbrauch           = 1310 kWh
PV-Überschuss               =  995 kWh
Max. PV-Überschuss          = 9.48 kWh am TMY-03-24
Netzeinspeisung             =  471 kWh
PV-Eigenverbrauchsanteil    =   67 % des PV-DC-Ertrags (Nutzungsgrad)
Eigendeckungsanteil         =   44 % des Verbrauchs (Autarkiegrad)
--->

Eine Stromspeicherung über mehrere Tage hinweg lohnt sich nicht &mdash; außer
man will oder muss (etwa bei mobiler Nutzung) längere Zeiten ohne Stromanschluss
überbrücken. Wer mit seiner Speicherbatterie zusätzlich eine
(Not-)Stromversorgung über eine [Inselanlage](Insel.md#Inselanlage) realisieren möchte,
wird die Kapazität je nach Anwendungsszenario entsprechend größer wählen.

Als Faustformel für die Dimensionierung [empfiehlt die Verbraucherzentrale NRW](
https://www.verbraucherzentrale.nrw/wissen/energie/lohnen-sich-batteriespeicher-fuer-photovoltaikanlagen-24589)
etwa 1&nbsp;kWh pro 1000&nbsp;kWh Jahresstromverbrauch
(also gut 1/3 des Verbrauchs pro 24 Stunden),
aber nicht mehr als 1&nbsp;kWh pro 1&nbsp;kWp PV-Nennleistung.


Die Forschungsgruppe Solarspeichersysteme der HTW Berlin
gibt [etwas genauere Empfehlungen und Begründungen](
https://solar.htw-berlin.de/publikationen/auslegung-von-solarstromspeichern/).
Kurz zusammengefasst:
Ein Batteriespeicher ist nur sinnvoll, wenn die PV-Leistung mind. 0,5&nbsp;kWp
je 1000&nbsp;kWh Jahresstromverbrauch beträgt.
Als Obergrenzen für die Kapazität empfiehlt sie
* 1,5&nbsp;kWh je 1000&nbsp;kWh Jahresverbrauch und
* 1,5&nbsp;kWh je kWp PV-Nennleistung.

Bei der Batterie-Dimensionierung sind noch folgende Punkte zu berücksichtigen:
* Die Speicherung des Stroms bringt je nach Lade- und Entladetechnik und
Art der [Batterie](Komp.md#Batterien) Verluste von etwa 10 bis 25% mit sich. Bei
AC-Kopplung kommt man selbst mit LiFePO4-Batterien kaum über 80% Wirkungsgrad.
* Man kann nicht die volle Nennkapazität entnehmen,
ohne dass die Akkuzellen leiden (d.h. schneller an Kapazität verlieren).
Bei LiFePO4 sind immerhin 90% Entladetiefe problemlos möglich.
* Im Interesse einer langen Lebensdauer sollte man die Batterie je nach Typ
auch höchstens kurzzeitig ganz voll geladen lassen (ansonsten eher zu 80 bis 90%).

### Kommerzielle SSG-Speicherlösungen {#kommerziell}

Aufgrund des wachsenden Interesses an Speicherlösungen auch für kleine
PV-Anlagen kamen 2023 die ersten steckerfertigen Lösungen auf den Markt.
Erst im Jahr 2025 waren die Produkte einigermaßen ausgereift.
Davor hatten sie teils noch sehr primitive Regelungen oder diverse
Kinderkrankheiten, wie [diese Zusammenstellung](Speicher-2024.md#kommerziell) vom Sommer 2024 zeigt.

Einen gute Übersicht, die zumindest bis November 2025 aktualisiert wurde,
findet sich [hier](https://www.energiemagazin.com/balkonkraftwerk/speicher/).
Die dortigen Aussagen zur Amortisation sind allerdings mit Vorsicht zu genießen,
u.A. weil sie von einer optimalen Lade- und Entladestrategie ausgehen.

Die kommerziellen Produkte haben Folgendes gemeinsam.
* Der Speicher ist proprietär &mdash; man muss also die (teils eher teuren)
  Batterien des jeweiligen Herstellers verwenden.
* Zentral für die Regelung der Geräte ist die aktuelle Zielleistung,
  die über den angeschlossenen Wechselrichter ins Hausnetz gespeist werden soll.
* Wenn die verfügbare PV-Leistung mindestens so groß wie die Zielleistung ist,
 wird diese Leistung eingespeist und der Rest zum Laden des Speichers verwendet.
* Wenn die aktuelle PV-Leistung unter der Zielleistung liegt, wird (je nach
  Gerät) die PV-Leistung eingespeist und/oder Strom aus dem Speicher entnommen.
* Die Speicher-Entladung wird durch die (typischerweise einstellbare)
  maximale Entladetiefe begrenzt.

Der Speicher ist je nach Gerät [AC- und/oder DC-gekoppelt](#Kopplung).
* AC-gekoppelte Speicher sind in der Verwendung sehr flexibel
  und können sogar ohne PV-Module betrieben werden.
* Bei DC-Koppluing wird der Speicher zusammen mit der Steuerung, 
  welche eine [MPPT](Komp.md#MPPT)-Regelung und [Batterie-Laderegelung](Komp.md#Laderegler)
  beinhaltet und teils direkt mit dem Speicher verbaut ist,
  zwischen PV-Module und Mikrowechselrichter gesteckt.
  Der wichtigste Vorteil davon ist größere Effizienz als mit AC-Kopplung.\
  Ein Nachteil ist, dass der Speicher meist außerhalb der Wohnung steht und
  eine Lithium-basierte Batterie bei Minustemperaturen nicht geladen sollte,
  so dass sie dann nur nutzbar ist, wenn sie auf über 0°C erwärmt wird.

#### Effizienzbetrachtung {#Effizienz}

Hier ein Vergleich des mit unterschiedlichen Ansätzen erzielbaren
Jahres-Eigenverbrauchs auf Basis von Simulationen mit dem [SolBatSim](EV.md#SolBatSim)
für einen Haushalt mit 3000&nbsp;kWh Jahresverbrauch
(nächtliche Durchschnittslast 190&nbsp;W zwischen 0 und 6&nbsp;Uhr,
tagsüber Durchschnittslast 375&nbsp;W zwischen 8 und 16&nbsp;Uhr)
mit optimal ausgerichteten 850&nbsp;Wp Modul-Nennleistung in Süddeutschland
und typischen Wirkungsgraden.
Der besseren Vergleichbarkeit halber wurde hier generell eine Speicherkapazität
von 1600&nbsp;Wh (mit 90% Entladetiefe) <!-- wie beim Anker Solix 2 --> vorausgesetzt
&mdash; ohnehin fällt sie kaum ins Gewicht.
* 610&nbsp;kWh Eigenverbrauch als Vergleichswert nur mit PV ohne Speicher-Nutzung
* 860&nbsp;kWh Eigenverbrauch (bei 1000&nbsp;Wh 810&nbsp;kWh, bei 2000&nbsp;Wh 880&nbsp;kWh)
  bei optimaler lastabhängiger Regelung
* 725&nbsp;kWh Eigenverbrauch bei [Anker Solix Solarbank 1](Speicher-2024.md#Solix1) Strategie mit optimal gewählter FLLR, hier 180&nbsp;W;\
  mit diesen Parametern werden 10&nbsp;kWh PV-Nettoleistung verworfen
* 735&nbsp;kWh Eigenverbrauch bei Konstanteinspeisung
  mit für diesen Fall optimaler Zielleistung, hier 260&nbsp;W

<!--
./Solar.pl Lastprofil_17_teils_31.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 850 -tmy
Nächtliche Durchschnittslast=  189 W von 0 bis 6 Uhr
PV-Eigenverbrauch           =  608 kWh

https://www.mydealz.de/comments/permalink/42396908
./Solar.pl Lastprofil_17_teils_31.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 850 -tmy -capacity 1600 -dc -max_charge 100 # Zendure, EcoFlow oder Maxxicharge 1600 Wh oder Solarbank 2 opt
PV-Eigenverbrauch           =  859 kWh   (bei 1000 Wh 810 kWh, 2000 Wh 881 kWh)

./Solar.pl Lastprofil_17_teils_31.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 850 -tmy -capacity 1600 -dc -max_charge 100 -pass spill 180 -feed excl 100  # Anker Solix Solarbank 1
Verworfene PV-Leistung      =   10 kWh
PV-Eigenverbrauch           =  725 kWh

./Solar.pl Lastprofil_17_teils_31.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 850 -tmy -capacity 1600 -dc -max_charge 100 -pass spill 200 -feed comp 200   # Konstanteinspeisung my Bypass
PV-Eigenverbrauch           =  740 kWh
./Solar.pl Lastprofil_17_teils_31.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 850 -tmy -capacity 2000 -dc -max_charge 100 -pass 260 -feed comp 260    # Konstanteinspeisung ohne Bypass
PV-Eigenverbrauch           =  734 kWh
-->

Wenn man eine optimale lastabhängige Lade- und Entladestrategie nutzen kann, ist
das Ergebnis mit Abstand am besten: ein Gewinn von etwa 250&nbsp;kWh im Jahr.\
Selbst mit mehreren geschickt eingesetzten Smart Plugs oder einer ausgefeilten
Uhrzeit-abhängigen Steuerung wird man kaum an diesen Maximalwert herankommen.\
Ansonsten ist es bei konstanter Zielleistung selbst mit günstigster Wahl dieses
Parameters und mit Bypass-Funktion ziemlich egal, welche Strategie im Detail
verfolgt wird &mdash; man erhält nur magere 135 bis 150&nbsp;kWh Gewinn pro Jahr.

Allerdings bringt selbst eine Eigenverbrauchs-Steigerung von 250&nbsp;kWh
bei 30&nbsp;ct/kWh nur 75€ Ersparnis pro Jahr.
Damit kann sich so ein Gerät, das je nach Speichergröße
(und Zusatzkosten wie für einen Shelly 3EM) ungefähr 1000€ kostet
und hoffentlich gut 10 Jahre Lebensdauer hat, meist nicht amortisieren.\
Noch schlechter sieht es für die [Anker Solix Solarbank 1](Speicher-2024.md#Solix1) aus, denn sie ermöglicht mit ihrer
ungünstigen Regelung eine Ersparnis von realistisch nur etwa 40€ pro Jahr.

Alle diese Lösungen sind für typische Balkonanlagen mit 2 Modulen
also einfach zu teuer, um rentabel zu sein.

<!--
./Solar.pl Lastprofil_17_teils_31.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 850 -tmy -bend 2,2,2,2,2,2,2,2,0.5,0.5,0.5,0.5,0.5,0.5,0.5,0.5,0.5,0.5,2,2,2,2,2,2
PV-Eigenverbrauch           =  366 kWh

./Solar.pl Lastprofil_17_teils_31.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 850 -tmy -capacity 1600 -dc -max_charge 100 -bend 2,2,2,2,2,2,2,2,0.5,0.5,0.5,0.5,0.5,0.5,0.5,0.5,0.5,0.5,2,2,2,2,2,2
PV-Eigenverbrauch           =  687 kWh
-->

Falls man tagsüber zwischen 8 und 18 Uhr nur halb so viel Verbrauch hatte wie
normal und in der übrigen Zeit entsprechend mehr (Durchschnittslast 294&nbsp;W
zwischen 0 und 6&nbsp;Uhr, 146&nbsp;W zwischen 8 und 16&nbsp;Uhr), wäre
die Stromspeicherung deutlich interessanter, und führt unter sonst gleichen
Bedingungen zu einer Steigerung des jährlichen Eigenverbrauchs von ungefähr
365&nbsp;kWh auf 685&nbsp;kWh. Dieses Szenario ist aber untypisch.
Die Amortisationszeit des Balkonkraftwerks ohne Speicher wäre dabei etwa doppelt
so lang wie normal, und die Hinzunahme des Speichers kann nur etwas mehr als das
kompensieren, was man durch die sehr ungünstige Verteilung des Stromverbrauchs
über die Tageszeiten verliert.

<!--
https://www.mydealz.de/deals/balkonkraftwerk-anker-solix-solarbank-2-e1600-pro-integrierter-800w-wechselrichter-4x-ja-solar-bifacial-440w-2385846#reply-48263080

 ./Solar.pl Lastprofil_17_teils_31.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 1800 -tmy
PV-Eigenverbrauch           =  859 kWh

./Solar.pl Lastprofil_17_teils_31.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 1800 -tmy -capacity 1600 -dc -max_charge 100
PV-Eigenverbrauch           = 1266 kWh

-->

Besser sieht es (wieder zurück bei einem typischen Lastprofil) dann aus, wenn man
<!--&mdash; etwa bei dem Zendure Hub 2000 oder der Anker Solix Solarbank 2 Pro &mdash; -->
vier Module nutzen kann, mit insgesamt z.B. 1800&nbsp;Wp.
Bei sonst gleichen Randbedingungen steigert ein 1,6&nbsp;kWh Speicher
den Eigenverbrauch pro Jahr etwa von 860&nbsp;kWh auf 1260&nbsp;kWh.
Die jährliche Ersparnis durch die Speicherlösung beträgt damit ungefähr 120€.
Bei einem Kaufpreis von ca. 1200€ amortisiert sich der Speicher also in 10 Jahren.

<!--
Zendure SolarFlow
https://www.mydealz.de/deals/balkonkraftwerk-750wp-set-mit-1kwh-speicher-wifi-22
36913
https://www.computerbild.de/artikel/cb-Tests-Energie-Zendure-SolarFlow-Akku-PV-Hub-Test-36635323.html
https://www.energiemagazin.com/zendure-solarflow-balkonkraftwerk-speicher/

Anker Solix
https://www.mydealz.de/comments/permalink/42351507
https://www.mydealz.de/comments/permalink/46690728

Habe jetzt mal meinen SolBatSim aufgebohrt, um auch diese Kompromiss-Strategie simulieren zu können.

Für einen Haushalt mit 3000&nbsp;kWh Jahresverbrauch und nächtlicher Mindestlast von 200 W
mit optimal ausgerichteten 880 Wp Modulen in Süddeutschland ergibt sich folgender Jahres-Eigenverbrauch:
* 611&nbsp;kWh ohne Speicher
* 875&nbsp;kWh mit 1,6&nbsp;kWh Speicher, DC-gekoppelt mit 90% Entladetiefe, bei optimaler Strategie
* 754&nbsp;kWh mit Speicher mit 140 W (Optimalwert) Bypass und Konstanteinspeisung 90 W (Optimalwert)
* 772&nbsp;kWh mit Speicher mit 180 W (Optimalwert) Bypass und Kompensation auf 110 W (Optimalwert), wie ich sie zuerst verstanden habe
* 760&nbsp;kWh mit Speicher mit 130 W (Optimalwert) Bypass und Anker Solix Entladestrategie (mit dem festen internen 100 W Grenzwert und 130 W konstanter Entladeleistung) - mit diesen Parametern werden immerhin nur 3,3&nbsp;kWh PV-Nettoleistung verworfen

Also, wenn man keine optimale lastabhängige Lade- und Entladestrategie fahren kann,
ist es bei DC-Kopplung und Ladestrategie mit einstellbarer konstanter Bypass-Leistung und vollem Bypass bei Überlauf der Batterie ziemlich egal,, welche sonstige Entladestrategie man hat/wählt,
sofern man die jeweils optimalen Parameter (Bypass-/Konstanteinspeisung-/Zielleistung) wählt.

Die Gewinne an Eigenverbrauch sind im Vergleich zur Situation ohne Speicher nicht berauschend: etwa 150&nbsp;kWh pro Jahr, also bei 35 ct/kWh um die 50€/Jahr.
So ein Gerät zum Preis von ca. 1000€ amortisiert sich daher nie.
--->
<!--

https://www.mydealz.de/comments/permalink/42371552
https://www.mydealz.de/comments/permalink/42363989 beide
https://www.mydealz.de/comments/permalink/44075989


Gut, dass es inzwischen bei anschlussfertig erhältlichen (aber immer noch
eigentlich zu teuren und damit nicht rentablen) Batteriepuffer-Produkten
für SSGs wie dem Zendure SolarFlow, Anker Solix oder GreenSolar Plug & Play
erste Ansätze gibt, Echtzeit-Lastmessgeräte wie das Shelly Pro 3EM
zur verbrauchsabhängigen Regelung zu verwenden, denn ohne eine solche Regelung
bleiben sie unrentables Nerd-Spielzeug bzw. teure Mogelpackungen.

https://www.mydealz.de/comments/permalink/44536868 Golem-Test
Doch wenn man einen [ersten Test-Artikel dazu](
https://www.golem.de/news/balkonkraftwerk-mit-shelly-pro-3em-den-zendure-batteriespeicher-steuern-2310-178813-3.html)
liest, drängt sich der Verdacht auf, dass der Verfasser und/oder Zendure
das nicht wirklich durchblicken und grobe Umsetzungs-Fehler gemacht haben,
so dass es (noch?) nicht so funktioniert wie es soll.
-->


<!--
Local IspellDict: german8
LocalWords: title keywords toc start refresh markdown pandoc width style margin
LocalWords: zusammenfassung Messgeraet CC BY Std webp Ferrariszaehler IAMKlaus
LocalWords: Unabhaengigkeitsrechner Stromwaechter Play SDM clams comment fazit
LocalWords: output calculation power unit rating Europe TSUN InGe DPM anker only
LocalWords: left right irradiance GHI buehneTop clear both png tgl RS solix eArc
LocalWords: potential csv grid tie inverter tmy peff ieff curb WiFi align Naja
LocalWords: standby xls jpg Balkonsolar center limiter off to html Rs Controler
LocalWords: blackout brownout panels busbars shingle panel up number solarbank
LocalWords: maximum point tracking sine wave efficiency boost true SG Shellys DL
LocalWords: converter step consumption pdf balancer equalizer mppt em Script
LocalWords: buck down SA SZ DW MQ EC LF small LY KREE Battery test br ATON Full
LocalWords: Charger Discharger Board Under Over Voltage Protection sub cpp img
LocalWords: Speicherungs current  Regelungs Eigenverbrauchsv WSW if PowerLimiter
LocalWords: telemetry gateway distort cell document sections profile Passthrough
LocalWords: post text standard conditions Reflexions PVSOL SOL assuming MG Stick
LocalWords: operating temperature Timeseries crystSi PVCalculator and NPB Komp
LocalWords: with entnahme bend OSO SSW SSO ready anlagen plugin date int limits
LocalWords: author today abstract This the ignored extension yaml txt interface
LocalWords: metadata add Austria description bagatellgrenze Loadprofiles
LocalWords: Yong Hui Green SolarPower backup net metering MPP Tracker SusEnergy
LocalWords: created changed nbsp pvroi ac dc break even fig SoC DoD MW Premium
LocalWords: Sense is end index output md ref of pv px Eff vs discussioncomment
LocalWords: my var pl zip load capacity feed spill deg magazine OC SC inrush
LocalWords: data transfer solar cut cells open short circuit voltage lim WLite
LocalWords: Ruecklaufsperre mdash Ueberlastung overpaneling LocalWords OW Heat
LocalWords: Bestrahlungsstaerke curves under different levels irradiation state
LocalWords: Microinverter What are Amps Volts SMF charge discharge Un Ent shunt
LocalWords: protector Micro Eco Worthy ISolar SPH GYVRM Cocar version cron job
LocalWords: Delivered Latest Downgraded shelly emeter file status returned MYPV
LocalWords: Zweirichtungszaehler issuecomment collect Notifications height ELWA
LocalWords: Plugs comments January Settings ons configuration states excl comp
LocalWords: sensor export float uksa tamorix custom firmware en Central zell TR
LocalWords: SmartShunt ComputerBase leistung meter Spaun easySuntower
-->
