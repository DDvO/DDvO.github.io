---
title: "Mini-Solaranlagen für daheim und unterwegs"
description: >-
  Online-Artikel von Dr. David von Oheimb
  mit wichtigen Hintergrund-Infos zum Thema Photovoltaik und
  vielen praktischen Tipps für Balkonkraftwerke und andere kleine Solar-Anlagen,
  einschließlich Hinweisen,
  welche Komponenten und Verwendungsformen sich unter welchen Umständen lohnen:
  exakte Simulationsergebnisse für Rentabilität, optimale Modul-Ausrichtung und
  die Verwendung von Wechselrichtern und Speicherbatterien inklusive Regelung.
date: 2022-03-20 20:36:16 +0100
created: ", erstellt in März 2022"
changed: ", letzte Änderung: "
lang: de
keywords:
- Photovoltaik
- Sonnenenergie
- Solarenergie
- Globalstrahlung
- Diffusstrahlung
- Halbzellen
- Drittelzellen
- bifazial
- Schindel
- Solaranlage
- Steckersolaranlagen
- Steckersolargeräte
- Stecker-Solar-Geräte
- SSG
- Balkonkraftwerk
- Konstanteinspeisung
- Nachteinspeisung
- Inselanlage
- Komponenten
- Informationen
- Infos
- Tipps
- Erfahrungen
- Beispiel
- Konfiguration
- Solarzellen
- Teilverschattung
- Solarpanels
- Solarmodule
- Ausrichtung
- Selbstverschattung
- PV-Heizstab
- Speicherung
- Stromspeicher
- Batteriespeicher
- Pufferbatterie
- Spannungsregler
- Laderegler
- Wechselrichter
- Netzkopplung
- Netzparallelbetrieb
- Hybridwechselrichter
- Einspeisung
- Ertrag
- spezifisch
- PV-Jahresertrag
- Optimierung
- Nutzungsprofil
- Lastprofil
- Telemetrie
- OpenDTU
- Shelly
- Lastspitzen
- Abregelung
- Drosselung
- Bagatellgrenze
- Kappungsverlust
- Eigenverbrauch
- Eigenverbrauchsanteil
- Eigendeckung
- Eigendeckungsanteil
- Autarkiegrad
- Batterieentladung
- Genehmigung
- Wohnungseigentümergemeinschaft
- WEG
- Versicherung
- Bauvorschriften
- Amortisation
- Rendite
- Ökologie
- Umwelt
abstract: |
  This is the abstract.
---
<!-- https://jekyllrb.com/docs/front-matter/
     https://pandoc.org/MANUAL.html#extension-yaml_metadata_block-->

Wichtige Hintergrund-Infos zur Photovoltaik und viele praktische Tipps für
Balkonkraftwerke und andere kleine Stecker-Solaranlagen -- einschließlich Hinweisen,
welche Komponenten und Verwendungsformen sich unter welchen Umständen lohnen:
exakte Simulationsergebnisse für Rentabilität, optimale Modul-Ausrichtung und
die Verwendung von Wechselrichtern und Speicherbatterien inklusive Regelung.

# Zusammenfassung {#Zusammenfassung}

Mit einem sog. *Steckersolargerät* kann man sehr einfach und relativ günstig
Solarstrom gewinnen und über eine Steckdose direkt ins Hausnetz einspeisen.
Das spart Stromkosten und kann sich je nach verwendeten Komponenten
und deren Aufstellung schon nach wenigen Jahren Betrieb rechnen ---
allerdings nur soweit man den Strom auch gleichzeitig selbst verbraucht.
Weil diese Betriebsart den überschüssigen Strom an die Allgemeinheit weitergibt
und keine Batterie benötigt, ist sie für die ökologische Gesamtbilanz am besten.

Für eine gewisse Unabhängigkeit von der nicht ständig kräftig vorhandenen
Sonneneinstrahlung und vom allgemeinen Stromnetz
braucht man eine aufladbare Batterie als Stromspeicher und weitere Geräte,
was das Ganze deutlich aufwendiger und teurer macht.\
Durch eine *Strompufferung* mit einer geeigneten vom aktuellen Verbrauch im
Haushalt abhängigen Regelung lässt sich überschüssige Energie zwischenspeichern
und bei Bedarf wieder abrufen und damit der Eigenverbrauchsanteil erhöhen.\
Eine sog. *Inselanlage* ist auch während Stromausfällen verwendbar,
soweit die Speicherkapazität und die Einstrahlung zum Nachladen reichen.

![Bild: Balkonkraftwerk und Dach-PV-Anlage](
Balkonkraftwerk_und_Dach-PV-Anlage.jpg)
<!--https://www.handelsblatt.com/adv/firmen/balkonkraftwerk-solar.html-->
<!--https://cdn.daa.net/images/photovoltaik/balkonkraftwerk.jpg-->
<!--https://www.solaranlagen-portal.com/photovoltaik/balkonkraftwerk-->

# Zielsetzung und Abgrenzung {#Zielsetzung}

Hier geht es nicht um *Solarthermie*, also die direkte Gewinnung von Wärme
durch Sonneneinstrahlung, sondern um die Erzeugung von elektrischem Strom.
Es geht auch nicht primär um „große“ Photovoltaik-Anlagen etwa auf Hausdächern
(dazu gibt es z.B. einen fundierten [Leitfaden von der HTW Berlin](
https://solar.htw-berlin.de/wp-content/uploads/HTW-PV-Wegweiser.pdf)),
wobei viele Aspekte natürlich gleich oder leicht übertragbar sind.

Meine Motivation als Autor ist vor allem physikalisch-technische Bildung ---
also relevante Zusammenhänge zu verstehen und möglichst hilfreich darzustellen.
Ich verfolge keinerlei kommerzielle Interessen (Verkauf, Sponsoring, o.ä.) ---
finanziell geht mir es darum, wie ich selbst und Andere mit vertretbarem Aufwand
und geringen Kosten möglichst viel Nutzen aus eigenem Solarstrom ziehen können.

Alle Inhalte sind von mir selbst recherchiert (meist online) und beschrieben,
wobei ich viele Quellen verlinke, die ich interessant und hilfreich finde.
Sehr viel praktisch Relevantes habe ich durch den Austausch zu PV-Angeboten
auf [myDealz.de](https://www.mydealz.de/) mitbekommen, überprüft und eingebaut.
Auch über das [Photovoltaik-Forum](https://www.photovoltaikforum.com/)
und PV-Enthusiasten vom [Solar2030](https://solar2030.de/) e.V.,
bei dem ich sei der Gründung Mitglied bin, kamen einige wertvolle Hinweise.\
Um möglichst verlässliche und detaillierte Werte zum nutzbaren Ertrag von
PV-Anlagen auch mit besonderen Eigenschaften ohne oder mit Speicher zu erhalten,
habe ich einen eigenen [Simulator](EV.md#SolBatSim) mit vielen Optionen entwickelt,
dessen Ergebnisse an mehreren Stellen maßgeblich eingeflossen sind.

Als Privatperson und auch als naturwissenschaftlich-technisch versierter
Nichtprofi kann ich natürlich keine offiziellen Informationen bzw. absolut
verlässliche Hinweise geben und für die Inhalte keine Gewähr oder gar Haftung
übernehmen. Wer bezüglich Stecker-PV-Anlagen etwas Offizielleres sucht,
der sei z.B. auf den schönen [Leitfaden von SmartGridsBW](
https://smartgrids-bw.net/public/uploads/2020/04/IBZ-Leitfaden_Balkon-PV-Online.pdf)
und die [„Fachinformation“ des DKE](https://www.dke.de/de/arbeitsfelder/energy/mini-pv-anlage-solar-strom-balkon-nachhaltig-erzeugen)
verwiesen.

# Nutzungslizenz {#Nutzungslizenz}

Die Verlinkung, Weitergabe und sonstige Weiterverwendung dieser Inhalte,
auch in geeigneten Auszügen, ist ausdrücklich erlaubt und erwünscht.
Bedingungen sind dabei Quellenangabe und Weitergabe unter gleichen Bedingungen,
was bei Verlinkung automatisch der Fall ist.\
Lizenzkürzel:
[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/deed.de)

<!-- markdown-toc start - Run M-x markdown-toc-refresh-toc -->
<!--
**Inhaltsverzeichnis**

- [Zusammenfassung { # Zusammenfassung}](#zusammenfassung-zusammenfassung)
-->
<!-- markdown-toc end -->

<!-- pandoc -s - -toc index.md -o output.md -->

# Inhaltsverzeichnis {#Inhaltsverzeichnis}

-   [Zusammenfassung](#Zusammenfassung)
-   [Zielsetzung und Abgrenzung](#Zielsetzung)
-   [Nutzunglizenz](#Nutzunglizenz)
-   [Inhaltsverzeichnis](#Inhaltsverzeichnis)
-   [Photovoltaik und ihr möglicher Ertrag](PV.md#Photovoltaik)<a name="Photovoltaik"></a>
    -   [Sonneneinstrahlung](PV.md#Sonneneinstrahlung)<a name="Sonneneinstrahlung"></a>
    -   [Nennleistung und Jahresertrag](PV.md#Nennleistung)<a name="Nennleistung"></a>
    -   [Optimale Ausrichtung von Solarmodulen](PV.md#Ausrichtung)<a name="Ausrichtung"></a>
        - [Aufteilung in mehrere Orientierungen](PV.md#Aufteilung)<a name="Aufteilung"></a>
-   [Stromverbrauch und Einspeisung im Haushalt](SV.md#Stromverbrauch)<a name="Stromverbrauch"></a>
    - [Strommessung](SV.md#Strommessung)<a name="Strommessung"></a>
        - [Einphasige Strommessung](SV.md#einphasig)<a name="einphasig"></a>
        - [Gesamt-Strommessung](SV.md#Gesamtstrom)<a name="Gesamtstrom"></a>
        - [Details zum Shelly 3EM](SV.md#Shelly3EM)<a name="Shelly3EM"></a>
    - [Stromzähler und Rücklaufsperre](SV.md#Stromzähler)<a name="Stromzähler"></a>
-   [Eigenverbrauch und seine Berechnung](EV.md#Eigenverbrauch)<a name="Eigenverbrauch"></a>
    -   [Typische Rentabilität kleiner PV-Anlagen](EV.md#rentabel)<a name="rentabel"></a>
    -   [Online-Berechnung](EV.md#online)<a name="online"></a>
        - [Stecker-Solar-Simulator und Unabhängigkeitsrechner](EV.md#HTW)<a name="HTW"></a>
        - [PV*SOL](EV.md#PVSOL)<a name="PVSOL"></a>
        - [PVTool@AkkuDoktor](EV.md#PVTool)<a name="PVTool"></a>
        - [brodsoft Stromverlauf](EV.md#brodsoft)<a name="brodsoft"></a>
        - [PV Calculator](EV.md#PVCalculator)<a name="PVCalculator"></a>
    -   [Ökonomisch orientierte PV-Rechner](EV.md#PV-Rechner)<a name="PV-Rechner"></a>
    -   [SolBatSim: Hochauflösende flexible Simulation](EV.md#SolBatSim)<a name="SolBatSim"></a>
-   [Nutzungsvarianten](SSG.md#Nutzung)<a name="Nutzung"></a>
    -   [Direkte Netzeinspeisung (Steckersolargerät SSG, „Balkonkraftwerk“)](SSG.md#SSG)<a name="SSG"></a>
        - [Hintergrund der Beschränkung auf 600 bzw. 800&nbsp;W](SSG.md#Bagatellgrenze)<a name="Bagatellgrenze"></a>
        - [Kappungsverlust durch Drosselung auf 600 bzw. 800&nbsp;W](SSG.md#Kappungsverlust)<a name="Kappungsverlust"></a>
    -   [Hausnetzeinspeisung mit Batteriepuffer](#Batteriepuffer)
        - [Regelungsstrategien für PV-Speicher](#Regelungsstrategien)
        - [Dimensionierung des Stromspeichers](#Speicherbatterie)
        - [Kommerzielle SSG-Speicherlösungen](#SSG-Speicher)
          - [Zendure SolarFlow und AIO 2400](#SolarFlow)
          - [Anker Solix](#Solix)
          - [Maxxisun Maxxicharge](#Maxxicharge)
          - [Tentek Tribune bzw. Anfuote EMS](#Tentek)
          - [Weitere Produkte](#SSG-Speicher-sonstige)
          - [Zusammenfassung und Effizienzbetrachtung](#SSG-Speicher-Effizienz)
        - [SSG-Speicherlösungen im Eigenbau](#SSG-Speicher-Eigenbau)
          - [Implementierung der Speicher-Regelung](#Regelungsimplementierung)
          - [Einfache und günstige Lösung: OpenDTU-OnBattery](#OpenDTU-OnBattery)
          - [Weiteres Beispiel für DC-gekoppelten Speicher](#SSG-DC-gekoppelt)
          - [Ladung des Stromspeichers](#Ladung)
          - [Konstanteinspeisung](#Konstanteinspeisung)
          - [Lastgeregelte Einspeisung](#lastgeregelt)
    -   [Inselanlage (mit Batteriespeicherung)](#Inselanlage)
    -   [Kombination aus Hausnetzeinspeisung und
        Inselanlage](#Kombination)
-   [Auswahl und Nutzung von Komponenten](Komp.md#Komponenten)<a name="Komponenten"></a>
    -   [PV-Module](Komp.md#PV-Module)<a name="PV-Module"></a>
        - [Elektrischer Anschluss](Komp.md#Anschluss)<a name="Anschluss"></a>
        - [Anbringung und Rechtliches](Komp.md#Anbringung)<a name="Anbringung"></a>
    -   [Mikrowechselrichter und andere Stromrichter](Komp.md#Stromrichter)<a name="Stromrichter"></a>
        - [MPPT-Solarregler](Komp.md#MPPT)<a name="MPPT"></a>
        - [Solar-Laderegler](Komp.md#Laderegler)<a name="Laderegler"></a>
        - [Wechselrichter](Komp.md#Wechselrichter)<a name="Wechselrichter"></a>
        - [Netzwechselrichter](Komp.md#Netzwechselrichter)<a name="Netzwechselrichter"></a>
        - [Inselwechselrichter](Komp.md#Inselwechselrichter)<a name="Inselwechselrichter"></a>
        - [Hybridgeräte: Solar-Laderegler mit Wechselrichter](Komp.md#Hybrid)<a name="Hybrid"></a>
        - [Gleichspannungswandler](Komp.md#Gleichspannungswandler)<a name="Gleichspannungswandler"></a>
    -   [Speicherbatterien](Komp.md#Batterien)<a name="Speicherbatterien"></a>
        - [Batterie-Ladezustand](Komp.md#Ladezustand)<a name="Ladezustand"></a>
        - [Batterie-Kapazität](Komp.md#Kapazität)<a name="Kapazität"></a>
        - [Batterie-Strukturierung](Komp.md#Strukturierung)<a name="Strukturierung"></a>
        - [Kombination aus Batterie und Wechselrichter](Komp.md#Kaskadierte)<a name="Kaskadierte"></a>
        - [Tiefsetzsteller](Komp.md#Tiefsetzsteller)<a name="Tiefsetzsteller"></a>
        - [Spannungswächter](Komp.md#Spannungswächter)<a name="Spannungswächter"></a>
-   [Beispiel-Konfigurationen](Bsp.md#Beispiele)<a name="Beispiele"></a>
    -   [Mobile Inselanlage](Bsp.md#Mobilanlage)<a name="Mobilanlage"></a>
<!-- -   [Steckersolargerät](Bsp.md#Steckeranlage)<a name="Steckeranlage"></a> -->
    -   [Kombi-Anlage](Bsp.md#Kombianlage)<a name="Kombianlage"></a>

### Hausnetzeinspeisung mit Pufferung in Batteriespeicher {#Batteriepuffer}

![Bild: Balkonkraftwerk mit Pufferbatterie und Inselwechselrichter](
Pufferbatterie_und_Inselwechselrichter.png){:.right width="400"
style="margin-left: 40px}
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
Bei einem Eigenbau mit günstigen Komponenten, die insgesamt 1000€ kosten,
würde sich das nach gut 6 Jahren amortisieren.
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
unter Annahme einer (effizienteren) [DC-Kopplung](#Ladung)
mit Lade-Wirkungsgrad 94% und Speicherungs-Wirkungsgrad 95%.
Wie zuvor sind für den Wirkungsgrad des PV-Systems 92% angenommen
und für die Wechselrichtung (auch bei Entladung aus der Batterie) 94%.

Bei [optimaler Lade-/Entlageregelung, s.u.](#Regelungsstrategien),
die leider nur schwer zu realisieren ist, gibt es keinen Verlust durch Überlauf
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
PV-Anlagen eine optimale Regelung im Eigenbau schwer erreichbar, und kommerziell
erhältliche Lösungen ([siehe unten](#SSG-Speicher)) sind bislang zu teuer.
<!--und auch eine Annäherung daran unverhältnismäßig aufwendig.-->

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

#### Regelungsstrategien für PV-Speicher {#Regelungsstrategien}

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

Die Anbindung des Speichers an die PV-Anlage erfolgt
entweder *DC-gekoppelt*, also schon gleichstromseitig,
oder *AC-gekoppelt*, also indirekt über das Wechselstromnetz im Haushalt.
Details dazu im Abschnitt [Ladung des Stromspeichers](#Ladung).

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

Die [Implementierung einer Speicher-Regelung](#Regelungsimplementierung),
welche [lastbasiert](#lastgeregelt) sein sollte, ist regelungstechnisch
ziemlich aufwendig. Sie lohnt sich finanziell bislang eher nur für
größere PV-Anlagen und (wegen der Speicherkosten) für nicht sehr große Speicher.

Statt einer lastabhängigen Regelung ist es besonders für Steckersolargeräte
viel einfacher, aber leider wenig effizient,
die (gedrosselte) Ausgangsleistung des Wechselrichters und die Batteriekapazität
so abzustimmen, dass lediglich ein Großteil der Grundlast des Haushalts,
z.B. 100&nbsp;W, für eine Dauer von etwa 1-2 Tagen abgedeckt wird.
Wenn man diese [*Konstanteinspeisung*](#Konstanteinspeisung) noch mit einer
Zeitschaltuhr (oder einem Helligkeitssensor) zur Beschränkung zwischen
Sonnenunter- und Aufgang kombiniert, bekommt man eine *Nachteinspeisung*.\
Ziel der Konstanteinspeisung ist zwar, die über die sonnenreiche Tageszeit
gesammelte Solarenergie auch über sonnenarme Zeiten gleichmäßig abzugeben
(solange die Ladung reicht, zumindest bis zum nächsten Vormittag),
und dabei möglichst wenig Strom nach extern zu verschenken.
Allerdings zeigen die [u.g. Simulationsergebnisse](#Ladung),
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

#### Dimensionierung des Stromspeichers {#Speicherbatterie}

Zum Thema *Stromspeicher* in verschiedensten Formen
und Nutzungsmöglichkeiten im Zusammenhang mit Photovoltaik
[hier ein ausführlicher Artikel](https://www.net4energy.com/de-de/stromspeicher)
und [hier](
https://www.wegatech.de/ratgeber/photovoltaik/stromspeicher/speicher-kennzahlen/)
eine gute Erklärung der wichtigsten Begriffe in diesem Zusammenhang,
z.B. der *Entladetiefe* und der *Zyklenanzahl*.

Die meisten Nutzer legen ihren PV-Speicher zu groß aus,
was unnötigen Materialaufwand und überzogene Kosten verursacht.
Die effektiv nutzbare Kapazität des Speichers sollte nur so groß sein, dass
damit der typische PV-Überschuss eines ertragreichen Sonnentages aufgenommen
und diese Strommenge bis zum nächsten Morgen sinnvoll genutzt werden kann.

Für das [o.g. Balkonkraftwerk-Beispiel](#Batteriepuffer) beträgt der tägliche
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
(Not-)Stromversorgung über eine [Inselanlage](#Inselanlage) realisieren möchte,
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
besser auch nicht ganz voll laden, sondern eher nur zu etwa 90%.

#### Kommerzielle SSG-Speicherlösungen {#SSG-Speicher}

Aufgrund des wachsenden Interesses an Speicherlösungen auch für kleine
PV-Anlagen gibt es seit 2023 ein paar steckerfertige Lösungen zu kaufen.
Eine brauchbare Übersicht findet sich
[hier](https://www.energiemagazin.com/balkonkraftwerk/speicher/) &mdash;
wobei das, was dort zur Amortisation geschrieben wurde, irreführend ist, weil es
unrealistischerweise von einer optimalen Lade- und Entladestrategie ausgeht.

Alle diese Produkte haben u.A. Folgendes gemeinsam.
* Der Speicher ist proprietär &mdash; man muss also die (recht teuren)
  Batterien des jeweiligen Herstellers verwenden.
* Der Speicher ist [DC-gekoppelt]((#Ladung)).
  Er wird also zusammen mit der Steuerung, welche eine MPPT-Laderegelung
  beinhaltet und teils direkt mit dem Speicher verbaut ist,
  zwischen PV-Module und Mikrowechselrichter gesteckt.
  Der wichtigste Vorteil davon ist größere Effizienz als mit AC-Kopplung.\
  Ein Nachteil ist, dass der Speicher meist außerhalb der Wohnung steht und
  eine Lithium-basierte Batterie bei Minustemperaturen nicht geladen sollte,
  so dass sie dann nur nutzbar ist, wenn sie auf über 0°C erwärmt wird.
* Zentral für die Regelung der Geräte ist die aktuelle Zielleistung,
  die über den angeschlossenen Wechselrichter ins Hausnetz gespeist werden soll.
* Wenn die verfügbare PV-Leistung mindestens so groß wie die Zielleistung ist,
 wird diese Leistung eingespeist und der Rest zum Laden des Speichers verwendet.
* Wenn die aktuelle PV-Leistung unter der Zielleistung liegt, wird (je nach
  Gerät) die PV-Leistung eingespeist und/oder Strom aus dem Speicher entnommen.
* Die Speicher-Entladung wird durch die (typischerweise einstellbare)
  maximale Entladetiefe begrenzt.

Hier eine Übersicht zu den jeweils unterstützten Lade- und Entladestrategien.

##### Zendure SolarFlow und AIO 2400 {#SolarFlow}

![Bild: Zendure SolarFlow](Zendure_SolarFlow.png){:.right width="400"}

Das wohl erste und bekannteste Produkt seiner Art ist das [Zendure SolarFlow](
https://www.chinahandys.net/zendure-solarflow-im-test-der-speicher-fuer-das-balkonkraftwerk/).
<!--
https://www.energiemagazin.com/zendure-solarflow-balkonkraftwerk-speicher/
https://www.allround-pc.com/artikel/2023/test-zendure-solarflow-speicher-fuer-dein-balkonkraftwerk
-->
Das Gerät verfügt über zwei PV-Eingänge mit getrennten MPPT.\
Soweit vorhanden, wird zur Einspeisung PV-Strom verwendet
und die ggf. zur Zielleistung fehlende Differenz aus dem Speicher entnommen.\
Wenn der Speicher voll ist, wird im Bypass-Modus der gesamte Ertrag eingespeist.\
Zur Bestimmung der Zielleistung gibt es inzwischen im Wesentlichen drei Modi:
* Im *Terminmodus* kann man abhängig von der Uhrzeit eine feste
Einspeiseleistung (in gewissen Stufen) einstellen, also im Wesentlichen eine
[Konstanteinspeisung bzw. Nachteinspeisung](#Konstanteinspeisung).
Dem einfachen Spezialfall, ständig 100&nbsp;W einzuspeisen,
hat Zendure den Namen *Batterieprioritätsmodus* gegeben.
* Im sog. *Intelligenten Matching-Modus* wird mindestens so viel eingespeist
wie nötig, um den Verbrauch aller Geräte abzudecken, die an mit dem SolarFlow
online gekoppelten *Smart Plugs* (intelligente Steckdosen) hängen &mdash;
mindestens 100&nbsp;W und [meist deutlich mehr](
https://www.hartware.de/2023/08/21/zendure-solarflow-im-test/4/) als nötig.
* [Seit November 2023](https://www.prnewswire.com/news-releases/zendure-erreicht-bahnbrechende-integration-mit-shelly-pro-3em-shelly-3em-shelly-plus-plug-s-und-shelly-plug-s-und-verbessert-das-intelligente-energiemanagement-301985902.html)
gibt es den *Smart-CT-Modus*, bei dem die Einspeiseleistung dynamisch an den
über ein Shelly (Pro) 3EM gemessen Gesamtverbrauch im Haushalt angepasst wird.\
Nur diese Option ermöglicht eine effiziente Nutzung des PV-Ertrags.
Allerdings [zeigten Praxistests](https://youtu.be/YzKCvYB-axw&t=148s), dass die
Regelung auf Verbrauchs- und Ertrags-Schwankungen träge und ungenau reagiert.

Die größere (1.920&nbsp;Wh) Batterie hat eine eingebaute Heizung bei Minusgraden.

Ende Februar 2024 brachte Zendure die AIO 2400 heraus &mdash; [hier](
https://www.computerbase.de/2024-02/zendure-aio-2400-test-balkonkraftwerk-akku-speicher/)
eine Rezension dazu.
Sie scheint die selbe Steuerung wie beim SolarFlow zu verwenden.

##### Anker Solix {#Solix}

Das zweite relativ bekannte Produkt die [Anker Solix Solarbank](
https://www.energiemagazin.com/anker-solix-solarbank-balkonkraftwerk-speicher/).
<!--https://www.chinahandys.net/anker-solix-solarbank-test/-->
Es hat nur einen MPPT.
Der einzige Betriebsart ist Einspeisung mit einer von der Uhrzeit abhängigen
Zielleistung, welche hier *Familienlastleistungsrate* (FLLR) genannt wird.
Sie kann 0&nbsp;W sein (keine Einspeisung)
und ist ansonsten zwischen 100 und 800&nbsp;W in Stufen von 10&nbsp;W wählbar.
Aufgrund einer Design-Einschränkung kann das Gerät diese Leistung nur entweder
direkt aus PV-Strom oder aus dem Speicher erbringen, also nicht gleichzeitig
aus beiden Quellen. Deshalb ist die Regelung etwas eigenartig:

![Bild: Anker Solix Strategie](Anker_Solix_Strategie.png){:.right width="560"}
* Wenn die PV-Leistung mindestens so hoch ist wie die FLLR,
  wird mit FLLR eingespeist und der Rest in den Speicher geladen
  (außer wenn er voll ist, dann erfolgt ein Bypass).
* Wenn die PV-Leistung mindestens 100&nbsp;W unter der FLLR liegt und höchstens
  100&nbsp;W beträgt, wird die FLLR dem Speicher entnommen
  (solange die Kapazität reicht) und die PV-Leistung geht verloren.\
  Dieser Verlust passiert zum Glück nicht groß, siehe u.g. Simulationsergebnisse.
* Ansonsten, also wenn die PV-Leistung zwischen 100&nbsp;W und der FLLR liegt
  oder weniger als 100&nbsp;W unter der FLLR
  (was bei einer FLLR von 200&nbsp;W aufs Gleiche hinausläuft),
  wird dem Speicher nichts entnommen und die verfügbare PV-Leistung eingespeist.

Das Produkt hat offenbar noch diverse Kinderkrankheiten, von denen z.B. [hier](
https://www.giga.de/test/anker-solix-solarbank-im-test-bezahlbarer-balkonkraftwerk-speicher-mit-schwaechen/)
berichtet wurde.
Im Jahr 2024 [will Anker Verbesserungen bringen](
https://www.energiemagazin.com/anker-solix-solarbank-balkonkraftwerk-speicher/#unser-test-fazit-zur-anker-solix-solarbank),
um auch Smart Plugs und Lastmessgeräte (Smart Home Integration) zu unterstützen.

<!-- https://www.mydealz.de/comments/permalink/45921047 -->
Es gibt Bastler, die dem Solix eine [nachgelagerte lastabhängige Drosselung](
https://community.home-assistant.io/t/using-anker-solix-solarbank-e1600-in-ha/636063)
über einen regelbaren Wechselrichter verpassen, so dass er über Nacht nur so
viel einspeisen kann wie gerade verbraucht wird. Das macht ihn zwar relativ
effizient, aber wer diesen Aufwand treibt, kann sich eigentlich gleich besser
und v.A. günstiger etwas eigenes bauen wie [dies](#SSG-Speicher-Eigenbau).
(Zusätzlich auch tagsüber in die merkwürdige Solix-Steuerung einzugreifen oder
sie zu umgehen wäre noch deutlich komplizierter und würde wohl wenig bringen.)

##### Maxxisun Maxxicharge {#Maxxicharge}

Bislang kaum bekannt und erst ab März 2024 allgemein lieferbar ist der
[Maxxicharge Batteriespeicher](https://www.maxxisun.de/maxxicharge).
Seine Entwicklung erfolgt(e) in Zusammenarbeit mit Hochschule Anhalt komplett
in Deutschland und macht einen sehr soliden Eindruck.
<!-- Es wird 10 Jahre Garantie gegeben. -->
Im Gegensatz zu allen vergleichbaren Produkten wurde er von vornherein auf
[optimale lastabhängige Regelung der Speichernutzung konzipiert](https://www.maxxisun.de/post/zum-ersten-mal-wird-strom-aus-einem-balkonkraftwerk-wirklich-intelligent-verwaltet).

![Bild: Maxxicharge Batteriespeicher](Maxxicharge.jpg){:.right width="798"}

Bei der Steuereinheit, genannt Central Control Unit (CCU), wird entweder ein
[Shelly (Pro) 3EM](SV.md#Shelly3EM) mitgeliefert oder eine Variante des
[powerfox poweropti](https://poweropti.powerfox.energy/), welcher die CCU
mit Last-Daten im Sekundentakt versorgt, und zwar in einem eigens aufgespannten
WLAN, wobei die Reichweite durch eine mitgelieferte Antenne vergrößert wird.

In den Batterien ist eine Heizung eingebaut, die auch an einem Aufstellort
außerhalb des Hauses eine Ladung bei Minustemperaturen (bis -20°C) ermöglicht.\
Die größte Variante hat 5&nbsp;kWh nutzbare Kapazität und unterstützt bis zu 3&nbsp;kWp
Modulleistung. Es können auch mehrere Speicher zusammengeschaltet werden
(bis zu 80&nbsp;kWh). Der Regelungsalgorithmus berücksichtigen auch unterschiedliche
effektive Kapazitäten und Ladungsstände der [einzelnen Batterie(zell)en](
https://www.maxxisun.de/post/maxxicharge-batteriespeichersysteme-denken-mit).\
Nachdem normale SSGs künftig rechtlich auf 2000&nbsp;Wp Modulleistung beschränkt
sollen, wurde Hilfe bei der Anmeldung von Anlagen mit mehr Leistung
[in Aussicht gestellt](https://www.akkudoktor.net/forum/postid/148774/).
Am Ende [dieses Artikels](
https://energiewende-tipps.de/balkonkraftwerke-mit-nulleinspeisung-durch-maxxicharge-batteriespeicher/) dazu der interessante Hinweis, dass der Batteriespeicher
nicht ortsfeste PV-Anlagen offenbar nicht angemeldet werden müssen.


##### Tentek Tribune bzw. Anfuote EMS {#Tentek}

![Bild: Tentek_Tribune_EMS_Controler](
Tentek_Tribune_EMS_Controler.png){:.right width="300"}

Seit März 2024 lieferbar ist der [Tentek Tribune EMS Controller](
https://www.notebookcheck.com/Balkonkraftwerke-effizient-nutzen-Neues-Dreiphasen-Energie-Steuersystem-von-Tentek-ist-vielseitig-und-anpassungsfaehig.775205.0.html)
bzw. baugleich die [Anfuote EMS-Steuerung](https://www.solarpower.anfuote.com/).

Dies ist das offenbar erste käufliche Steuergerät, das nicht nur mit allen
möglichen Netzwechselrichtern, sondern auch mit [angeblich so gut wie jeder Art
von Speicherbatterie mit 48&nbsp;V Systemspannung)](
https://www.tentekenergy.com/index.php/products/324.html) verwendbar ist.
Es hat [je nach Variante 2 bis 4 MPPT](
https://www.photovoltaikforum.com/thread/221060-tentek-tribune-ems-anfuote/?postID=3667554#post3667554)
zur Anbindung der PV-Module mit je 30&nbsp;A Ladeleistung
für einen DC-gekoppelten Speicher und bietet eine
[sehr gute lastabhängige Einspeise-Regelung](https://youtu.be/vRo15Xi9tMo),
wobei zur Messung des Haushalts-Lastsaldos ein mitgelieferter
WiFi-Energiemonitor [oder wahrscheinlich auch ein Shelly (Pro) 3EM](
https://www.youtube.com/watch?v=LFtjLljnRvA) verwendet werden kann.
<!--
https://www.mydealz.de/deals/balkonkraftwerkspeicher-plugplay-speicher-balkonkraftwerk-anfuote-tentek-2310245#comments
https://www.photovoltaikforum.com/thread/221060-tentek-tribune-ems-anfuote/?pageNo=8
-->

Für das Gerät soll man in Deutschland inklusive WiFi-Energiemonitor
[selbst mit MwSt-Befreiung 599€](https://titansolar.de/products/tentek) zahlen,
so dass man auch mit einer günstigen max. 2,5 kWh Batterie auf etwa 1000€ kommt.
Das wäre für ein Balkonkraftwerk ca. 300€ zu teuer,
denn [wie unten ausgeführt](#SSG-Speicher-Effizienz) kann man damit in einem
durchschnittlichen Fall nur etwa 70€ pro Jahr sparen, so dass man selbst bei
700€ Kosten schon eine grenzwertig lange Amortisationszeit von 10 Jahren hat.

Direkt aus China ist das Gerät angeblich für unter 300€ erhältlich.
Das wäre aufgrund der Ausstattung auch realistischer, denn es leistet nicht
mehr als eine Eigenbau-Lösung mit [OpenDTU-OnBattery](#OpenDTU-OnBattery) und
zwei MPPT-Ladereglern, was man mit mäßigem Aufwand selbst mit soliden Victron
BlueSolar-Geräten für ca. 140€ hinbekommen kann, mit einem MPPT für 100€.


##### Weitere Produkte {#SSG-Speicher-sonstige}

Es gibt weitere ähnliche Lösungen, etwa
* [EcoFlow PowerStream](
  https://www.chinahandys.net/ecoflow-powerstream-im-test/), welches ähnliche
  Modi bietet wie das ursprüngliche Zendure SolarFlow, also zeitabhängige
  Konstanteinspeisung oder die Verwendung von Smart Plugs,
  aber keine von der Gesamtlast abhängige Regelung.
* [GreenSolar Plug & Play Balkonkraftwerk Basisspeicher](
https://greensolar.de/produkt/plug-play-balkonkraftwerk-batteriespeicher-set-basisspeicher-erweiterungsspeicher)
  von der österreichischen Firma Green Solar
  (nicht zu verwechseln mit GreenAkku bzw. Bosswerk aus Deutschland), welches
  etwas günstiger ist, aber nur eine simple Konstanteinspeisung bietet, und
<!--
https://www.mydealz.de/deals/plug-play-balkonkraftwerk-batteriespeicher-basisspeicher-22-kwh-2249574#comments
https://www.notebookcheck.com/Deal-Balkonkraftwerk-Speicher-2-24-kWh-mit-Plug-Play-von-Greensolar-jetzt-mit-25-Rabatt-erhaeltlich.754099.0.html
https://www.homeandsmart.de/green-solar-speicher-ankuendigung
https://www.infranken.de/ratgeber/wohnen/energiesparen/balkonkraftwerk-speicher-fuer-899-euro-besser-als-anker-zendure-ecoflow-art-5639603
-->


##### Zusammenfassung und Effizienzbetrachtung {#SSG-Speicher-Effizienz}

Viele dieser Produkte haben mehr oder weniger starke Einschränkungen und
funktionieren in der Praxis nicht so gut und effizient wie vom Marketing behauptet.
Stand Anfang 2024 unterstützen nur Zendure SolarFlow und AIO 2400,
der Maxxisun Maxxicharge das Tentek/Anfuote EMS eine lastabhängige Regelung
und können damit unter realistischen Bedingungen rentabel sein.

Hier ein Vergleich des mit den unterschiedlichen Ansätzen erzielbaren
Jahres-Eigenverbrauchs auf Basis von Simulationen mit dem [SolBatSim](EV.md#SolBatSim)
für einen Haushalt mit 3000&nbsp;kWh Jahresverbrauch
(nächtliche Durchschnittslast 190&nbsp;W zwischen 0 und 6&nbsp;Uhr,
tagsüber Durchschnittslast 375&nbsp;W zwischen 8 und 16&nbsp;Uhr)
mit optimal ausgerichteten 850&nbsp;Wp Modul-Nennleistung in Süddeutschland
und typischen Wirkungsgraden.
Der besseren Vergleichbarkeit halber wurde hier generell eine Speicherkapazität
von 1600&nbsp;Wh (mit 90% Entladetiefe) wie beim Anker Solix vorausgesetzt
&mdash; ohnehin fällt sie kaum ins Gewicht.
* 610&nbsp;kWh Eigenverbrauch als Vergleichswert nur mit PV ohne Speicher-Nutzung
* 840&nbsp;kWh Eigenverbrauch (bei 1000&nbsp;Wh 800&nbsp;kWh, bei 2000&nbsp;Wh 860&nbsp;kWh)
  bei optimaler lastabhängiger Regelung
* 710&nbsp;kWh Eigenverbrauch bei Anker Solix Strategie mit optimaler FLLR, hier 160&nbsp;W;\
  mit diesen Parametern werden 10&nbsp;kWh PV-Nettoleistung verworfen
* 725&nbsp;kWh Eigenverbrauch bei Konstanteinspeisung
  mit für diesen Fall optimaler Zielleistung, hier 200&nbsp;W

Wenn man eine optimale lastabhängige Lade- und Entladestrategie nutzen kann, ist
das Ergebnis mit Abstand am besten: ein Gewinn von etwa 230&nbsp;kWh im Jahr.\
Selbst mit mehreren geschickt eingesetzten Smart Plugs oder einer ausgefeilten
Uhrzeit-abhängigen Steuerung wird man kaum an diesen Maximalwert herankommen.\
Ansonsten ist es bei konstanter Zielleistung selbst mit günstigster Wahl dieses
Parameters und mit Bypass-Funktion ziemlich egal, welche Strategie im Detail
verfolgt wird &mdash; man erhält nur magere 100 bis 125&nbsp;kWh Gewinn pro Jahr.

Allerdings bringt selbst eine Eigenverbrauchs-Steigerung von 230&nbsp;kWh
bei 30&nbsp;ct/kWh nur 70€ Ersparnis pro Jahr.
Damit kann sich so ein Gerät, das je nach Speichergröße
(und Zusatzkosten wie für einen Shelly 3EM) ungefähr 1000€ kostet
und hoffentlich gut 10 Jahre Lebensdauer hat, meist nicht amortisieren.\
Noch schlechter sieht es für das Anker Solix aus, denn es ermöglicht mit seiner
ungünstigen Regelung eine Ersparnis von realistisch nur etwa 35€ pro Jahr.\
Sprich, alle diese Lösungen sind einfach zu teuer, um wirklich rentabel zu sein.

<!--
./Solar.pl Lastprofil_17_teils_31.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 850 -tmy
Nächtliche Durchschnittslast=  189 W von 0 bis 6 Uhr
PV-Eigenverbrauch           =  608 kWh

https://www.mydealz.de/comments/permalink/42396908
./Solar.pl Lastprofil_17_teils_31.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 850 -tmy -capacity 1600 -dc -max_charge 100 # EcoFlow oder Maxxicharge 1600 Wh opt
PV-Eigenverbrauch           =  843 kWh   (bei 1000 Wh 798 kWh, 2000 Wh 861 kWh)

./Solar.pl Lastprofil_17_teils_31.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 850 -tmy -capacity 1600 -dc -max_charge 100 -pass spill 160 -feed excl 100  # Anker Solix
Verworfene PV-Leistung      =   10 kWh
PV-Eigenverbrauch           =  710 kWh   (bei 2000 Wh 716 kWh)

./Solar.pl Lastprofil_17_teils_31.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 850 -tmy -capacity 1600 -dc -max_charge 100 -pass spill 200 -feed comp 200   # Konstanteinspeisung
PV-Eigenverbrauch           =  726 kWh   (bei 2000 Wh 737 kWh)
-->
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


#### SSG-Speicherlösungen im Eigenbau {#SSG-Speicher-Eigenbau}

Wer für sein Balkonkraftwerk einen rentablen Stromspeicher haben will, kommt
derzeit um einen Eigenbau nicht herum, allein schon wegen der Batteriepreise.
Außerdem muss man sich technisch gut auskennen und einige Arbeit investieren,
um eine effiziente Regelung hinzubekommen.
In diesem Abschnitt einige Hinweise und Beispiele,
wie es gelingen kann und wie es nicht wirklich effizient wird.

##### Implementierung der Speicher-Regelung {#Regelungsimplementierung}

Wie im Abschnitt über [Regelungsstrategien](#Regelungsstrategien) erklärt,
ist die wesentliche Eingangsgröße der Regelung eines Speichers
der Gesamt-Leistungssaldo am externen Netzanschluss des Haushalts.
Er lässt sich mit digitalem Zugang an einem modernen Stromzähler
oder mit einem Zusatzgerät im Unterverteiler messen,
wie im Abschnitt [Gesamt-Strommessung](SV.md#Gesamtstrom) beschrieben.

Über das Leistungssaldo sollte ein am Speicher angeschlossener dynamisch
drosselbarer [Netzwechselrichter](Komp.md#Netzwechselrichter) so geregelt werden,
dass durch Entladung des Speichers zumindest ein Teil der Haushalts-Last
kompensiert wird, aber nicht durch zu starke Entladung Energie aus dem Speicher
ins externe Netz eingespeist und damit verschenkt wird.

Wenn der Wechselrichter, der zur Entladung des Speicherbatterie verwendet wird,
mehrere Eingänge hat, kann man an die übrigen Eingänge auch noch direkt
PV-Module anschließen, deren Ertrag dann nicht über die Batterie gepuffert wird.

Für die Ladung des Speichers ist es eine grundsätzliche Entscheidung, ob diese
DC- oder AC-gekoppelt geschehen soll &mdash; Details dazu im Abschnitt zur
[Ladung des Stromspeichers](#Ladung).

Bei DC-Kopplung bietet es sich an, einen [Solar-Laderegler](Komp.md#Laderegler) zu
verwenden, denn der kümmert sich automatisch um die Regelung der Batterieladung.
Unabhängig davon, dass ein Wechselrichter angeschlossen und zeitweise mehr oder
weniger aktiv ist, versucht der Laderegler immer, die Batterie voll zu machen.
Je nachdem, wie viel Strom der Wechselrichter liefern soll, nimmt er dem Ausgang
des Ladereglers bzw. der Batterie entsprechend Strom weg, so dass zum Laden der
Batterie weniger oder gar nichts mehr übrig bleibt. Wenn der Wechselrichter
sich mehr Strom nimmt als der Laderegler liefert, wird die Batterie entladen.\
Für eine optimale [lastabhängige Regelung](#lastgeregelt)
muss also der Laderegler nicht von außen gesteuert werden,
sondern es genügt, die Ausgangsleistung des Wechselrichters so anzupassen,
dass der aktuelle Leistungssaldo am Einspeisepunkt der Haushalts
(der sich aus Haushalts-Last abzüglich PV-Leistung
und bisheriger Ausgangsleistung des Wechselrichters ergibt)
möglichst Null ist, jedenfalls nicht negativ.
Je nachdem, ob dabei die Differenz aus aktueller PV-Leistung und
Abruf durch den Wechselrichter positiv oder negativ ausfällt,
wird der Speicher mit dieser Differenz-Leistung geladen oder entladen.

Bei AC-Kopplung muss die Speicher-Ladung unabhängig von der PV-Erzeugung
erfolgen und erfordert ein steuerbares 230&nbsp;V-Ladegerät mit extra Regelung.
<!-- TODO Netzladegerät -->

Die (Lade- und) Entladeregelung wird auf irgendeine Weise programmiert und
muss ständig laufen, z.B. auf einen etwas stärkeren Einplatinen-Computer
wie Raspberry Pi 4 oder nebenbei auf einem Home-Server. Meist erfolgt
die Programmierung unter Zuhilfenahme einer Heimautomatisierungs-Software.

[Home Assistant](https://www.home-assistant.io/) ist da am bekanntesten.
Das bietet eine recht hübsche und flexible grafische Bedienungs-Oberfläche,
sowie eine relativ einfache Anbindung von Hardware-Komponenten z.B. von Shelly,
aber hat eine grauenhafte YAML -und Python-basierte Programmierumgebung mit nur
teilweise hilfreicher Dokumentation und schlechter Debugging-Unterstützung.

Wesentlich angenehmer programmierbar ist wohl die Perl-basierte „Freundliche
Hausautomation und Energie-Messung“ [(FHEM)](https://fhem.de/fhem_DE.html).

Weitere Möglichkeiten sind der [iobroker](https://www.iobroker.net/?lang=de#de/)
und das Projekt [Solaranzeige.de](https://solaranzeige.de/) für Raspberry Pi.


##### Einfache und günstige Lösung: OpenDTU-OnBattery {#OpenDTU-OnBattery}

Inzwischen gibt es eine relativ einfache und kostengünstige Möglichkeit, mit
wenig Arbeitsaufwand und ohne eigene Programmierung zu einer recht effizienten
Speicherlösung für ein SSG/Balkonkraftwerk zu kommen, und zwar dank des
Projekts [OpenDTU-OnBattery](https://github.com/helgeerbe/OpenDTU-OnBattery).
Dies ist eine Weiterentwicklung der
[OpenDTU](https://github.com/tbnobody/OpenDTU), welche wie im Abschnitt zur
[Einspeisung aus einer Batterie](#lastgeregelt) beschrieben einen Mikrocontroller
zur offenen Kommunikation per WLAN mit einem Hoymiles-Wechselrichter einrichtet.

![Bild: OpenDTU-OnBattery.jpg](OpenDTU-OnBattery.png){:.right width="755"}
* Der Clou dabei ist, den OpenDTU Mikrocontroller auch gleich zur lastbasierten
Regelung der Einspeisung des Wechselrichters zu verwenden, statt irgendwo
anders z.B. Home Assistant oder iobroker laufen lassen zu müssen.
* Zudem wird natürlich ein dreiphasiges Leistungsmessgerät mit Dateninterface
([Shelly 3EM](SV.md#Shelly3EM), Eastron SDM oder Stromzähler-Lesekopf mit
[Tasmota](https://www.tasmota.info/)-Software) benötigt, um den aktuellen
Leistungssaldo des Haushalts in Sekundenauflösung zu erhalten.
* Die Ladung des Speichers erfolgt effizient mit DC-Kopplung, und zwar über
einen [Solar-Laderegler](Komp.md#Laderegler) von Victron, dessen [VE.Direct interface](
https://www.victronenergy.com/live/vedirect_protocol:faq) zur Regelung benötigt
wird, weil sich damit die PV-Leistung abfragen lässt.
Je nach der maximalen Gesamtspannung der hierbei meist in Reihe geschalteten
PV-Module genügt teils schon ein BlueSolar 75/15 und
sicherlich ein 100/15 (der 100&nbsp;V Eingangsspannung verträgt).
Die Batteriespannung muss für den (direkten) Anschluss des Wechselrichters
mindestens 24&nbsp;V betragen, was von allen Victron-Varianten unterstützt wird.
Für eine Batteriespannung von 48&nbsp;V eignet sich etwa der 100/20.
* Die aktuelle Batteriespannung kann über ein BMS-Interface, den Laderegler
und den Wechselrichter abgefragt werden, benötigt also kein Extra-Gerät.
* Außerdem werden nur noch ein USB-Anschluss o.ä. zur Stromversorgung sowie ein
paar Kabel zur Verbindung von Laderegler, Batterie und Wechselrichter gebraucht.
* Bei Betrieb des Speichers z.B. auf dem Balkon empfiehlt sich eine Heizmatte
mit Thermostat, um die Batterie auch bei Minustemperaturen laden zu können.

[Hier](https://github.com/helgeerbe/OpenDTU-OnBattery/wiki/Dynamic-Power-Limiter)
die Übersicht der konfigurierbaren Regelungsparameter.\
Der Regelungsalgorithmus, welcher in der C++-Quelldatei [PowerLimiter.cpp](
https://github.com/helgeerbe/OpenDTU-OnBattery/blob/development/src/PowerLimiter.cpp)
implementiert ist, arbeitet im Wesentlichen wie folgt:\
Berechne in einer Endlosschleife immer wieder einen neuen Zielwert (Limit)
für die Wechselrichter-Ausgangsleistung, sende ihn an das Gerät und warte, bis
positive Rückmeldung erfolgt, was beim Hoymiles meist 5-10&nbsp;Sekunden dauert.
Für den Zielwert gibt es verschiedene Fälle:

|Batterie-Ladezustand|PV-Leistung| resultierendes Wechselrichter-Limit | Effekt auf die Batterie |
|:-------------------|:----------|:------------------------------------|:------------------------|
|gering     |<&nbsp;20&nbsp;W|Wechselrichter aus   |Ladung ggf. mit schwacher PV-Leistung|
|gering     |≥&nbsp;20&nbsp;W|min(Last,PV−Leistung)|Ladung ggf. mit PV-Überschuss        |
|ausreichend|                |Last<!--img width=16ex/-->|Entladung&nbsp;falls&nbsp;Last&nbsp;>&nbsp;PV−Leistung,&nbsp;sonst&nbsp;Ladung|
|ausreichend|                |max(Last,PV−Leistung)|Entladung falls Last > PV−Leistung, keine Ladung falls (Full) Solar-Passthrough aktiviert|

Die Regelung ist so flink wie möglich, aber berücksichtigt nicht die
<!-- im [Abschnitt zur Einspeisung](lastgeregelt) genannten -->
bei Betrieb an einer 24&nbsp;V Batterie
[teils groben Abweichungen eines Hoymiles-Geräts](
https://www.photovoltaikforum.com/thread/221194-hm-400-an-batterie-limitierung-%C3%BCber-opendtu-eigenartig/?postID=3660691#post3660691)
von großen Limit-Sollwerten.

Geht man davon aus, dass ein SSG mit Hoymiles-Wechselrichter bereits vorhanden
ist und angesichts dessen, dass
für ein SSG eine Nenn-Speicherkapazität von 1,28&nbsp;kWh ausreichend ist,
ergeben sich (Stand März 2024) bei günstigem Einkauf in etwa folgende Kosten:
* LiFePO4-Batterie 25,6&nbsp;V 50 Ah mit BMS: 200€
* Victron MPPT Laderegler: je nach Variante ca. 70€
* Shelly 3EM: 80€
* ESP32-Mikrocontroller plus passendes WLAN-Modul, fertig konfektioniert: 30€
* Heizmatte mit Thermostat: 20€
* Kleinteile wie Kabel und Stecker: 20€

Das ergibt in Summe 420€.
Wie [oben](#Batteriepuffer) ausgeführt, lassen für ein Balkonkraftwerk in einem
Durchschnittshaushalt mit effektiv 1 kWh Speicherkapazität etwa 200&nbsp;kWh
zusätzlicher Eigenverbrauch pro Jahr erzielen, was ungefähr 60€ entspricht.
Damit amortisiert sich diese Speicherlösung in etwa 7 Jahren.


##### Weiteres Beispiel für DC-gekoppelten Speicher {#SSG-DC-gekoppelt}

Hier ein Beispiel für eine gelungene, aber etwas aufwendigere effiziente Lösung
mit DC-gekoppelter Anbindung eines 48&nbsp;V LiFePO4 Speichers
(bestehend aus einer oder zwei Batterien), wozu je ein Victron
SmartSolar MPPT 100/20-48V [Solar-Laderegler](Komp.md#Laderegler) verwendet wird.
Sowohl für die sofortige Nutzung des erzeugten PV-Stroms als auch für das
bedarfsgerechte Laden und Entladen des Speichers kommt ein
(derzeit auf max. 600&nbsp;W Leistung gedrosselter) Hoymiles HM-800
[Netzwechselrichter](Komp.md#Netzwechselrichter) zum Einsatz,
der per Heimautomatisierung über eine Ahoy-DTU oder OpenDTU geregelt wird.\
Optional wird hier ein Victron Phoenix 48&nbsp;V 800&nbsp;W
[Inselwechselrichter](Komp.md#Inselwechselrichter) verwendet,
was dann Notstrom-Fähigkeit mit Batterie-gepufferter Sonnenenergie bietet.

![Bild: SSG-mit-DC-gekoppeltem-Speicher.png](
SSG-mit-DC-gekoppeltem-Speicher.png){:.right width="798"}

Weil die Batteriespannung für eine Balkonanlage recht hoch ist
und die Solar-Laderegler bis zu 100&nbsp;V Eingangspannung vertragen,
können und müssen die PV-Module in Reihe geschaltet werden,
und die Kabelquerschnitte können auch auf DC-Seite relativ gering bleiben,
ohne dass es zu nennenswerten Leitungsverlusten kommt.\
Die hier beschriebene Lösung wäre aber auch basierend auf einem 24&nbsp;V Speicher
gut möglich, zumal der Eingangspannungs-Bereich des verwendeten Wechselrichters
auch den Bereich um 24&nbsp;V umfasst und die Kabel zwischen Laderegler,
Speicher und Wechselrichter kurz gehalten werden können.

Damit die Batterien auch bei Minusgraden geladen werden können,
kommt hier eine [Pflanzen-Heizmatte wie diese](
https://www.ebay.de/itm/354441767526?var=623842819621Plfan) zum Einsatz, welche
man dann allerdings noch temperaturgeregelt mit Strom versorgt werden muss.
Einfacher wäre, eine Wärmematte mit verbundenem Thermostat zu verwenden.

Die Regelung sollte nach den Optimierungs-Prinzipien erfolgen, die im Abschnitt
zu [Regelungsstrategien für Stromspeicher](#Regelungsstrategien) erklärt sind.
Die dazu nötige Messung des Gesamt-Leistungssaldos am Einspeisepunkt des Haushalts,
also wie viel gerade aus dem externen Netz gezogen oder dorthin eingespeist
wird, erfolgt wie im Abschnitt [Gesamt-Strommessung](SV.md#Gesamtstrom) beschrieben.
Wenn dazu (wie im Bild dargestellt) Tibber Pulse verwendet wird, kann die
Nutzung des Speichers auch vom aktuellen Strompreis abhängig gemacht werden.

Die Batteriespannung (damit indirekt der ungefähre [Ladezustand](Komp.md#Ladezustand)
des Speichers) und die PV-Leistung kann z.B. über ein Victron VE.Direct USB-Kabel
von der [Victron Venus Firmware auf einem Raspberry Pi](
https://www.victronenergy.com/blog/2017/09/06/raspberry-pi-running-victrons-venus-firmware/)
(hier genügt 2. oder 3. Generation) abgefragt werden.

Als Grundlage für die selbst programmierte Regelung wurde hier die Perl-basierte
[(FHEM)](https://fhem.de/fhem_DE.html) auf einem Raspberry Pi 4 verwendet.
Alternativen dazu und Details zur DC-Kopplung sind im
[Abschnitt zur Implementierung der Speicher-Regelung](#Regelungsimplementierung)
aufgeführt.

In Minimalausstattung würde die Anlage mit ECO-WORTHY 48&nbsp;V 2,5&nbsp;kWh Speicher
ohne PV-Module unter 1000€ kosten.
Mit allen optionalen Komponenten inkl. Inselwechselrichter hat die Anlage
mit 5&nbsp;kWh Speicherkapazität ohne PV-Module im Herbst 2023 knapp 2200€ gekostet.\
Details zu der Anlage können bei
[Michael Steigemann](mailto:michael.steigemann) von
[Solar2030.de](https://solar2030.de/) erfragt werden.

##### Ladung des Stromspeichers {#Ladung}

Das Laden der Batterie erfolgt am besten möglichst direkt aus der PV-Anlage
über einen [Solar-Laderegler](Komp.md#Laderegler). Dies nennt man [*DC-Kopplung*](
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
und Wechselrichter auch draußen (z.B. auf dem Balkon oder in einem Schuppen)
platzieren. Damit die Anlage dann auch bei Minustemperaturen nutzbar ist, wo
[Lithium-basierte Batterien nicht geladen werden sollten](
https://www.ipowerqueen.de/blogs/batteriewissenschaft/warum-ist-der-schutz-vor-niedrigen-temperaturen-fur-lithiumbatterien-wichtig),
kann man den Speicher mit einer Heizung versehen und gegen Kälte isolieren.
Dafür bietet sich Wärmematte mit Thermostat an, welche es auch schon
[für 15€ gibt](https://www.amazon.de/KIPIDA-Reptilienheizmatte-Einstellbar-Reptilienw%C3%A4rmematte-Temperaturregelung/dp/B0CG3FCJ9H).
Die Heizmatte braucht nur dann aktiv sein, wenn bei unter 0°C die Sonne scheint.

[Kommerzielle DC-gekoppelte Lösungen](#SSG-Speicher) für kleine PV-Anlagen wie
Balkonkraftwerke sind leider allesamt nicht rentabel. Mit etwas Eigenarbeit
lässt sich aber mit Hilfe von [OpenDTU-OnBattery](#OpenDTU-OnBattery) und einem
Victron-Laderegler eine günstige und effiziente Lösung zusammenbauen.

Bei *AC-Kopplung* hingegen wird der PV-Strom zunächst ins Wechselstromnetz
eingespeist, so dass die Ladung (an einem beliebigen Ort, meist im Haus)
mit einem 230&nbsp;V-Ladegerät geschieht, wobei man zur Entladung einen zweiten
(Batterie-)Wechselrichter benötigt.
Ihr besonderer Vorteil ist eine große Flexibilität bei der Wahl der Komponenten,
auch bzgl. eines späteren Ausbaus und der Betriebsspannung der Komponenten,
weil die Batteriespannung von der Systemspannung der PV-Anlage unabhängig ist.
Außerdem kann man den Speicher bei Bedarf (z.B. wenn er zu leer geworden ist
oder zu Testzwecken) auch unabhängig von der PV-Anlage mit Netzstrom laden.\
Eine AC-Kopplung ist im Allgemeinen aber nicht zu empfehlen, weil sie recht
umständlich ist und einen schlechten Wirkungsgrad hat: etwa 80%.

Für eine kleine Anlage kann man zur AC-Kopplung wie in
[diesem Video](https://www.youtube.com/watch?v=fcFFUN3Pkbo&t=300s) beschrieben
ein regelbares Netzteil wie den
[MeanWell HLG-600H](MeanWell_HLG-600H.pdf)-30AB LED-Treiber verwenden
und über einen [Shelly Plus 0-10V Dimmer](
https://www.shelly.com/de/products/shop/shelly-plus-0-10-v-dimmer)) und
geeignete Software so steuern, dass PV-Überschuss in die Batterie geladen wird.

![Bild: MeanWell_HLG-600H-36AB-im_Schaltkasten.jpg](
MeanWell_HLG-600H-36AB-im_Schaltkasten.jpg){:.right width="798"}
Die Steuerung kann auch über einen Mikrocontroller erfolgen, der ein PWM-Signal
erzeugt, das dann in ein 0-10&nbsp;V Analogsignal gewandelt wird, wie in
[diesem Vorgänger-Video](https://www.youtube.com/watch?v=WK9PQ1_TpU8) erklärt.

Manche verwenden zu diesem Zweck ein [Meanwell NPB Batterieladegerät](
https://www.elkoba.com/magazin/produkt/npb-1200-24/),
welches über sein CAN-Bus-Interface verfügt und über einen
[*Trucki2MeanWell Gateway (T2MG)*](https://trucki.de/t2mg/) Stick
gesteuert werden kann.
Allerdings sind als Ladestrom offenbar nur [50-100% des Nennstroms einstellbar](
https://www.digikey.de/de/product-highlight/m/mean-well/npb-series).
Außerdem wird jede Änderung normalerweise ins interne EEPROM gespeichert,
was bei sehr vielen Schreibzugriffen das Gerät beschädigen würde,
weshalb man ihre Frequenz z.B. auf 30 Sekunden einschränken sollte &mdash;
bzw. bei Modellen ab 2024 kann man diese Schreibfunktion wohl abschalten.

Wie im [Abschnitt über Regelungsstrategien](#Regelungsstrategien) beschrieben,
sollte die Aufladung der Batterie zu jeder Zeit nur in dem Maße erfolgen, wie
der PV-Strom gerade nicht anderweitig direkt genutzt werden kann (Lastvorrang).
Das optimiert die Speichernutzung in mehrfacher Hinsicht:
* Eine Speicherung ist im Vergleich zur direkten Nutzung
  immer mit zusätzlichen Verlusten verbunden.
* Je intensiver eine Batterie genutzt wird, desto schneller sinkt ihre Kapazität
  --- daher sollte die Zahl der Lade-/Entladezyklen nicht unnötig groß sein.
* Je voller der Strompuffer ist, desto größer die Wahrscheinlichkeit, dass er
  keine zusätzliche Ladung mehr aufnehmen kann und der Überschuss verloren geht.

Der Lastvorrang bringt für die Effizienz fast so viel wie eine optimale
[lastabhängige Entnahme](#lastgeregelt) aus der Batterie.

##### Konstanteinspeisung {#Konstanteinspeisung}

In diesem und dem [folgenden Abschnitt](#lastgeregelt)
werden für die Entnahme von Energie aus einem Stromspeicher
verschiedene Strategien und mögliche Umsetzungen mit einem
[Netzwechselrichter](Komp.md#Netzwechselrichter) behandelt.

Die einfachsten Anlagen verwenden eine *Konstanteinspeisung*,
wobei der Netzwechselrichter immer die gleiche Leistung abgibt.
Eine zeitgesteuerte Variante wird *Nachteinspeisung* genannt.

Anlagen mit Konstanteinspeisung, bei der die PV-Erzeugung
nur in den Speicher geleitet wird (also ohne Überschussableitung oder
eine deutlich aufwendigere lastabhängige Batterie-Regelung),
bringen selbst bei optimierter Wahl der Entnahmeleistung sehr wenig,
weil bei voller Batterie relativ viel überschüssige Energie verloren geht.
Eine höhere konstante Entnahmeleistung oder eine Überschussableitung verringert
zwar den Komplettverlust des Überschusses, führt aber dazu, dass mehr Energie
im Haushalt nicht genutzt und stattdessen ins externe Netz abgegeben wird.

Bei einer Konstanteinspeisung sollte man die Einspeiseleistung so einstellen,
dass sie sicher unter der Minimallast bleibt und anderseits so hoch ist,
dass man die gespeicherte Energie auch bis zum nächsten Laden verbraucht.
Auch sollte man irgendwie dafür sorgen, dass maximal so viel geladen wird,
wie gerade tatsächlich an PV-Überschuss vorliegt (also die aktuelle Erzeugung
größer als der Verbrauch ist), aber auch nicht zu wenig geladen wird,
so dass der Speicher am Ende des Tages möglichst voll ist.
Je größer die Speicherkapazität im Vergleich zum Verbrauch und zur Erzeugung,
desto schwieriger ist das ohne lastabhängige Regelung hinzubekommen.\
Viele scheitern schon an der Bestimmung der [Minimallast](SV.md#Strommessung),
den diese ist geringer als etwa die (leichter bestimmbare) Durchschnittslast in
der Nacht. Wer die Konstanteinspeisung auf die nächtliche Durchschnittslast
einstellt, verschenkt über die meiste Zeit, wo periodisch laufende Geräte
wie Kühlschränke nicht laufen, mehr oder weniger teurer gespeicherten Strom.

Wenn die [o.g. Balkonanlage mit 1&nbsp;kWh Pufferspeicher](#Batteriepuffer) nur eine
Konstanteinspeisung verwendet (wobei hier eine Entladeleistung von nur 40&nbsp;W
optimal ist), ergibt sich mit der optimalen Ladestrategie eine Steigerung des
Jahres-Eigenverbrauchs durch die Speichernutzung um immerhin 115&nbsp;kWh auf 575&nbsp;kWh.
Das sind allerdings 65&nbsp;kWh weniger als wenn auch die Entladung lastoptimiert
wäre, weil 66&nbsp;kWh nicht genutzt und ins externe Netz abgeführt werden.\
Eine Erhöhung der nutzbaren Speicherkapazität auf 2&nbsp;kWh brächte nur 10&nbsp;kWh mehr.

<!--
TODO check/update ./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 600 -peff 92 -tmy -capacity 1250 -dc -feed 45

Speicherkapazität           = 1250 Wh mit max. Ladehöhe 90%, max. Entladetiefe 90%, DC-gekoppelt
Optimale Ladestrategie (nicht gebrauchte Energie), max. Laderate 1 C
Konstanteinspeisung         =   40 W, max. Entladerate 1 C
Verlust durch Überlauf      =    0 kWh
Ladeverlust                 =   11 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =    9 kWh durch Speicher-Wirkungsgrad 95%
PV-Nutzung über Speicher    =  112 kWh
Zwischenspeicherung         =  185 kWh (nach Ladeverlust)
Vollzyklen pro Jahr         =  185 der effektiven Kapazität

PV-Eigenverbrauch           =  575 kWh
Netzeinspeisung             =   65 kWh
PV-Eigenverbrauchsanteil    =   87 % des Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =   19 % des Verbrauchs (Autarkiegrad)
-->
<!--
TODO check/update ./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 600 -peff 92 -tmy -capacity 2500 -dc -feed 35

Speicherkapazität           = 2500 Wh mit max. Ladehöhe 90%, max. Entladetiefe 90%, DC-gekoppelt
Optimale Ladestrategie (nicht gebrauchte Energie), max. Laderate 1 C
Konstanteinspeisung         =   35 W, max. Entladerate 1 C
Verlust durch Überlauf      =    0 kWh
Ladeverlust                 =   11 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =    9 kWh durch Speicher-Wirkungsgrad 95%
PV-Nutzung über Speicher    =  122 kWh
Zwischenspeicherung         =  189 kWh (nach Ladeverlust)
Vollzyklen pro Jahr         =   95 der effektiven Kapazität

PV-Eigenverbrauch           =  585 kWh
Netzeinspeisung             =   55 kWh
PV-Eigenverbrauchsanteil    =   89 % des Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =   20 % des Verbrauchs (Autarkiegrad)
-->

Die hier aufgeführten Entnahme-Varianten geben keinen Lastvorrang,
sondern führen den erzeugten Solarstrom vorzugsweise in die Batterie.
Das ist natürlich am einfachsten, hat aber den großen Nachteil, dass zu den
Zeiten, wo die Batterie voll ist, **viel PV-Energie verloren geht** ---
etwa an sonnenreichen Tagen am Nachmittag, wenn die Solarleistung relativ groß
ist im Vergleich zur Batteriekapazität bzw. dem Verbrauch durch die Grundlast.

Wenn die Anlage eine Konstanteinspeisung hat und den PV-Strom nur auf diese
Weise nutzt, ergibt sich Folgendes: Selbst bei optimierter Entnahmeleistung
(in diesem Fall 180&nbsp;W) bringt die Batteriepufferung fast nichts: der
Eigenverbrauch steigt durch Speichernutzung gerade mal um 29&nbsp;kWh auf 489&nbsp;kWh.
Das liegt hier vor Allem an einer Netzeinspeisung von 74&nbsp;kWh
und am Verlust durch Überlauf von 29&nbsp;kWh,
außerdem an Lade- und Speicherverlusten von 38 + 30&nbsp;kWh bei 631 Vollzyklen.\
Eine Erhöhung der nutzbaren Kapazität auf 2&nbsp;kWh
brächte immerhin einen Eigenverbrauch von 532&nbsp;kWh
bei einer dann optimalen Konstanteinspeisung von 125&nbsp;W.

<!--
TODO check/update ./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 600 -peff 92 -tmy -capacity 1250 -dc -pass 0 -feed 180

Speicherkapazität           = 1250 Wh mit max. Ladehöhe 90%, max. Entladetiefe 90%, DC-gekoppelt
Speicher-Umgehung           =    0 W, max. Laderate 1 C
Konstanteinspeisung         =  180 W, max. Entladerate 1 C
Verlust durch Überlauf      =   29 kWh
Ladeverlust                 =   38 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =   30 kWh durch Speicher-Wirkungsgrad 95%
PV-Nutzung über Speicher    =  489 kWh
Zwischenspeicherung         =  631 kWh (nach Ladeverlust)
Vollzyklen pro Jahr         =  631 der effektiven Kapazität

PV-Eigenverbrauch           =  489 kWh
Netzeinspeisung             =   74 kWh
PV-Eigenverbrauchsanteil    =   74 % des Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =   16 % des Verbrauchs (Autarkiegrad)
-->
<!--
TODO check/update ./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 600 -peff 92 -tmy -capacity 2500 -dc -pass 0 -feed 130

Speicherkapazität           = 2500 Wh mit max. Ladehöhe 90%, max. Entladetiefe 90%, DC-gekoppelt
Speicher-Umgehung           =    0 W, max. Laderate 1 C
Konstanteinspeisung         =  125 W, max. Entladerate 1 C
Verlust durch Überlauf      =    7 kWh
Ladeverlust                 =   39 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =   31 kWh durch Speicher-Wirkungsgrad 95%
PV-Nutzung über Speicher    =  532 kWh
Zwischenspeicherung         =  653 kWh (nach Ladeverlust)
Vollzyklen pro Jahr         =  327 der effektiven Kapazität

PV-Eigenverbrauch           =  532 kWh
Netzeinspeisung             =   51 kWh
PV-Eigenverbrauchsanteil    =   81 % des Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =   18 % des Verbrauchs (Autarkiegrad)
-->


Man kann bei Konstanteinspeisung mit einer zusätzlichen *Überschussableitung*
(Bypass) dafür sorgen, dass bei vollem Speicher der Solarstrom an der Batterie
vorbei geleitet wird (und zwar möglichst in den Netzwechselrichter,
der auch zur Ausspeisung aus der Batterie verwendet wird).
In diesem Fall sind für die Konstanteinspeisung etwa 100&nbsp;W Entnahme optimal,
und der Eigenverbrauch steigt durch die Speichernutzung ein wenig mehr,
nämlich um 54&nbsp;kWh auf 514&nbsp;kWh.\
Eine Erhöhung der nutzbaren Kapazität auf 2&nbsp;kWh
brächte einen Eigenverbrauch von 539&nbsp;kWh,
wobei die optimale Leistung der Konstanteinspeisung hier bei 110&nbsp;W liegt.

<!--
TODO check/update ./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 600 -peff 92 -tmy -capacity 1250 -dc -pass spill 0 -feed 100

Speicherkapazität           = 1250 Wh mit max. Ladehöhe 90%, max. Entladetiefe 90%, DC-gekoppelt
Speicher-Umgehung           =    0 W und für Überschuss, max. Laderate 1 C
Konstanteinspeisung         =  100 W, max. Entladerate 1 C
Verlust durch Überlauf      =    0 kWh
Ladeverlust                 =   32 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =   25 kWh durch Speicher-Wirkungsgrad 95%
PV-Nutzung über Speicher    =  425 kWh
Zwischenspeicherung         =  537 kWh (nach Ladeverlust)
Vollzyklen pro Jahr         =  537 der effektiven Kapazität

PV-Eigenverbrauch           =  514 kWh
Netzeinspeisung             =   89 kWh
PV-Eigenverbrauchsanteil    =   78 % des Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =   17 % des Verbrauchs (Autarkiegrad)
-->
<!--
TODO check/update ./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 600 -peff 92 -tmy -capacity 2500 -dc -pass spill 0 -feed 110

Speicherkapazität           = 2500 Wh mit max. Ladehöhe 90%, max. Entladetiefe 90%, DC-gekoppelt
Speicher-Umgehung           =    0 W und für Überschuss, max. Laderate 1 C
Konstanteinspeisung         =  100 W, max. Entladerate 1 C
Verlust durch Überlauf      =    0 kWh
Ladeverlust                 =   37 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =   29 kWh durch Speicher-Wirkungsgrad 95%
PV-Nutzung über Speicher    =  508 kWh
Zwischenspeicherung         =  619 kWh (nach Ladeverlust)
Vollzyklen pro Jahr         =  309 der effektiven Kapazität

PV-Eigenverbrauch           =  539 kWh
Netzeinspeisung             =   55 kWh
PV-Eigenverbrauchsanteil    =   82 % des Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =   18 % des Verbrauchs (Autarkiegrad)
-->

Das Signal für die Überschussableitung wird wohl am besten vom Laderegler
kommen (z.B. optisch über die Ladekontrollleuchte). Es kann aber auch von der
Batteriespannung abhängig gemacht werden, wobei dann auch (meist ohne Probleme)
vorkommen kann, dass Laderegler und Wechselrichter gleichzeitig aktiv sind.

Wenn man schon einen Solar-Wechselrichter hat und diesen für eine ganz einfache
Netzeinspeisung verwenden möchte, könnte es schon genügen, ihn (über eine
Sicherung und wenn nötig eine gesonderte automatische Unterspannungsabschaltung)
mit der Batterie zu verbinden und nach Bedarf über einen Schalter zu steuern ---
natürlich nur, wenn die Batteriespannung im Eingangsspannungsbereich des
Wechselrichters liegt und es passt, ihn mit seiner vollen oder fest limitierten
Leistung zu betreiben. Dazu kann man beispielsweise einen auf 300&nbsp;W begrenzten
PV-Eingang nutzen oder die Drosselung konfigurieren, wie man es z.B. beim Deye
[selbst machen](https://www.photovoltaikforum.com/thread/191715-deye-sun600-umstellen-auf-800w/?pageNo=9#post3019090)
oder vom Kundendienst (Mail an service@deye.com.cn) programmieren lassen kann.

![Bild: Netzwechselrichter aus Batterie gespeist](
Netzwechselrichter-aus-Batterie-gespeist.jpg){:width="600" .right}
Etwas besser ist allerdings, die Einspeisung manuell regelbar zu gestalten.
Dazu bietet sich ein Netzwechselrichter wie von
[Soyosource](https://de.aliexpress.com/item/1005001445871590.html) bzw.
[PMSUN](https://www.amazon.de/PMSUN-netzgekoppelter-Wechselrichter-einstellbare-Batterieentladung/dp/B0B4RZNHF3)
an, der für die Verwendung an einer Batterie als Quelle ausgelegt ist
und dessen Ausgangsleistung innerhalb gewisser Grenzen einstellbar ist.

Wer zudem bereits eine Powerstation hat,
kann zwischen ihren Wechselstrom-Ausgang und den Netzwechselrichter ein
regelbares Netzteil hängen, wie [von Andreas Schmitz vorgeschlagen](
https://www.youtube.com/watch?v=ZXHAXrJS9CU),
was allerdings zu Zusatz-Verlusten durch Hin- und Her-Wandlung des Stroms führt.

Man kann auch einen normalen Solar-Wechselrichter verwenden und ihm
einen günstigen [Gleichspannungswandler](Komp.md#Gleichspannungswandler)
mit regelbarer Strombegrenzung (engl. _limiter_) vorschalten.
Allerdings passiert es dann leicht, dass sich die Regelungen der beiden Geräte
ins Gehege kommen. Daher stellt man die Eingangsspannung für den Wechselrichter
besser etwas unterhalb des [MPPT](Komp.md#MPPT)-Bereichs ein,
aber (zumindest anfangs) oberhalb seiner Anlaufspannung.
Außerdem kann es sein, dass der Wechselrichter versucht,
stets seine maximale Ausgangsleistung zu liefern, was bei eher geringer
Eingangsspannung zu einem entsprechend hohen Eingangsstrom führt,
der auch über der Stärke liegen kann, die das Gerät über längere Zeit verträgt.
Daher und aus Effizienzgründen ist es zu empfehlen, einen Wechselrichter zu
wählen, der direkt elektronisch regelbar ist, und das lastabhängig zu machen.

<!--
Allerdings hat keine der in diesem Abschnitt genannten Anlagen mit
Pufferspeicher eine Überschussableitung (Bypass) oder gar eine optimale Laderegelung.
* Bei bedarfsgerechter Einspeisung
  aus dem Speicher ohne Überschussableitung bei der Ladung des Speichers
  fällt die Steigerung des Eigenverbrauchs durch die Speichernutzung
  identisch aus, also wieder 128&nbsp;kWh auf 588&nbsp;kWh. Die Zahl der Vollzyklen
  pro Jahr (658) und die Lade- und Speicherverluste sind fast gleich.
  Darüber hinaus fällt wieder nur ein gleich kleiner Verlust von 3 kWh an, in
  diesem Fall nicht durch Netzeinspeisung, sondern durch Überlauf des Speichers.\
  Auch hier *bringt eine Erhöhung der nutzbaren Speicherkapazität praktisch nichts,
  und eine Verringerung auf 0,5&nbsp;kWh liefert aber wesentlich weniger*: 545&nbsp;kWh.

[//]: #
-->
<!--
TODO check/update ./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 600 -peff 92 -tmy -capacity 1250 -dc -pass 0 -feed lim 600

Speicherkapazität           = 1250 Wh mit max. Ladehöhe 90%, max. Entladetiefe 90%, DC-gekoppelt
Speicher-Umgehung           =    0 W, max. Laderate 1 C
Maximaleinspeisung          =  600 W, max. Entladerate 1 C
Verlust durch Überlauf      =    2 kWh
Ladeverlust                 =   40 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =   31 kWh durch Speicher-Wirkungsgrad 95%
PV-Nutzung über Speicher    =  588 kWh
Zwischenspeicherung         =  658 kWh (nach Ladeverlust)
Vollzyklen pro Jahr         =  658 der effektiven Kapazität

PV-Eigenverbrauch           =  588 kWh
Netzeinspeisung             =    0 kWh
PV-Eigenverbrauchsanteil    =   89 % des Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =   20 % des Verbrauchs (Autarkiegrad)
-->
<!--
TODO check/update ./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 600 -peff 92 -tmy -capacity 1875 -dc -pass 0 -feed lim 600

Speicherkapazität           = 1875 Wh mit max. Ladehöhe 90%, max. Entladetiefe 90%, DC-gekoppelt
Speicher-Umgehung           =    0 W, max. Laderate 1 C
Maximaleinspeisung          =  600 W, max. Entladerate 1 C
Verlust durch Überlauf      =    0 kWh
Ladeverlust                 =   40 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =   31 kWh durch Speicher-Wirkungsgrad 95%
PV-Nutzung über Speicher    =  590 kWh
Zwischenspeicherung         =  660 kWh (nach Ladeverlust)
Vollzyklen pro Jahr         =  440 der effektiven Kapazität

PV-Eigenverbrauch           =  590 kWh
Netzeinspeisung             =    0 kWh
PV-Eigenverbrauchsanteil    =   89 % des Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =   20 % des Verbrauchs (Autarkiegrad)
-->
<!--
TODO check/update ./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 600 -peff 92 -tmy -capacity 625 -dc -pass 0 -feed lim 600

Speicherkapazität           =  625 Wh mit max. Ladehöhe 90%, max. Entladetiefe 90%, DC-gekoppelt
Speicher-Umgehung           =    0 W, max. Laderate 1 C
Maximaleinspeisung          =  600 W, max. Entladerate 1 C
Verlust durch Überlauf      =   51 kWh
Ladeverlust                 =   37 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =   29 kWh durch Speicher-Wirkungsgrad 95%
PV-Nutzung über Speicher    =  545 kWh
Zwischenspeicherung         =  610 kWh (nach Ladeverlust)
Vollzyklen pro Jahr         =  1220 der effektiven Kapazität

PV-Eigenverbrauch           =  545 kWh
Netzeinspeisung             =    0 kWh
PV-Eigenverbrauchsanteil    =   82 % des Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =   18 % des Verbrauchs (Autarkiegrad)
-->
<!--
* Bei Anlagen mit konstanter (nicht bedarfsgeregelter) Einspeisung hingegen
gibt es wie [oben beschrieben](#Ladung) auf die eine oder andere Weise
große Verluste, so dass die Steigerung des Eigenverbrauchs sehr gering ausfällt.
-->

{:style="clear:both"}

[![Bild: Balkonkraftwerk mit Speicher - PV&E](
Balkonkraftwerk_mit_Speicher.png){:.right width="380"
style="margin-left: 40px}](
https://www.youtube.com/watch?v=N6NqMXQHP2I)
Auf jeden Fall muss für die Situation, dass die Batterieladung zur Neige geht
(bei LiFePO4 spätestens bei 90% Entladung) eine automatische Abschaltung
vorhanden sein, damit die Batterie nicht durch Tiefentladung geschädigt wird.
Wenn für den Notfall stets eine gewisse Strommenge zur Verfügung bleiben soll,
muss die Abschaltung schon entsprechend früher erfolgen.

Wenn der Solar-Laderegler einen Lastausgang mit einstellbarer Schutzabschaltung
hat, wie z.B. der Victron BlueSolar, kann man ihn so verwenden, wie Tobias Volk
(PV&E) in [diesem schönen Video](https://youtu.be/N6NqMXQHP2I) zeigt. Zudem
kann dessen Straßenlichtfunktion für die zeitliche Steuerung genutzt werden.

Eine Konstanteinspeisung auch noch zeitlich z.B. auf 18 Uhr abends bis 6 Uhr
morgens einzuschränken (also eine Nachteinspeisung) erweist sich aber als
völlig kontraproduktiv, weil der Speicher dann
sehr oft und schnell überläuft und damit massiv Energie verschwendet wird.
Es ergibt sich für die o.g. Anlage selbst bei einer optimierten Entnahmeleistung
von 80&nbsp;W dann nur noch ein Eigenverbrauch von 269&nbsp;kWh, also im Vergleich
zur Basis-Anlage ohne Speicher eine Verringerung um 190&nbsp;kWh!\
Durch Erhöhung der nutzbaren Speicherkapazität auf 2&nbsp;kWh
lassen sich zwar immerhin 398&nbsp;kWh Eigenverbrauch erreichen,
aber auch dann bleibt der Ansatz kontraproduktiv.

<!--
TODO check/update ./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 600 -peff 92 -tmy -capacity 1250 -dc -pass 0 -feed 80 18..6

Speicherkapazität           = 1250 Wh mit max. Ladehöhe 90%, max. Entladetiefe 90%, DC-gekoppelt
Speicher-Umgehung           =    0 W, max. Laderate 1 C
Konstanteinspeisung         =   80 W von 18 bis 6 Uhr, max. Entladerate 1 C
Verlust durch Überlauf      =  344 kWh
Ladeverlust                 =   19 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =   15 kWh durch Speicher-Wirkungsgrad 95%
PV-Nutzung über Speicher    =  269 kWh
Zwischenspeicherung         =  316 kWh (nach Ladeverlust)
Vollzyklen pro Jahr         =  315 der effektiven Kapazität

PV-Eigenverbrauch           =  269 kWh
Netzeinspeisung             =   13 kWh
PV-Eigenverbrauchsanteil    =   41 % des Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =    9 % des Verbrauchs (Autarkiegrad)

TODO check/update ./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 600 -peff 92 -tmy -capacity 2500 -dc -pass 0 -feed 150 18..6

Speicherkapazität           = 2500 Wh mit max. Ladehöhe 90%, max. Entladetiefe 90%, DC-gekoppelt
Speicher-Umgehung           =    0 W, max. Laderate 1 C
Konstanteinspeisung         =  150 W von 18 bis 6 Uhr, max. Entladerate 1 C
Verlust durch Überlauf      =  144 kWh
Ladeverlust                 =   31 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =   24 kWh durch Speicher-Wirkungsgrad 95%
PV-Nutzung über Speicher    =  398 kWh
Zwischenspeicherung         =  516 kWh (nach Ladeverlust)
Vollzyklen pro Jahr         =  257 der effektiven Kapazität

PV-Eigenverbrauch           =  398 kWh
Netzeinspeisung             =   62 kWh
PV-Eigenverbrauchsanteil    =   60 % des Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =   13 % des Verbrauchs (Autarkiegrad)

-->

Eine zusätzliche Überschussableitung bringt das Ergebnis zwar wieder ins
Positive, so dass sich bei dann optimaler Entnahmeleistung von 75&nbsp;W ein Gewinn
an Eigenverbrauch von 33&nbsp;kWh auf 493&nbsp;kWh ergibt, aber lohnenswert ist das nicht,
denn auch dann fällt der Gewinn immer nach geringer aus als ohne Einschränkung
auf die Nachtstunden (wo der [Gewinn 54&nbsp;kWh](#Ladung) beträgt).\
Eine Erhöhung der nutzbaren Kapazität auf 2&nbsp;kWh
brächte beim Eigenverbrauch nur 10&nbsp;kWh mehr.

<!--
TODO check/update ./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 600 -peff 92 -tmy -capacity 1250 -dc -pass spill 0 -feed 75 18..6

Speicherkapazität           = 1250 Wh mit max. Ladehöhe 90%, max. Entladetiefe 90%, DC-gekoppelt
Speicher-Umgehung           =    0 W und für Überschuss, max. Laderate 1 C
Konstanteinspeisung         =   75 W von 18 bis 6 Uhr, max. Entladerate 1 C
Verlust durch Überlauf      =    0 kWh
Ladeverlust                 =   19 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =   15 kWh durch Speicher-Wirkungsgrad 95%
PV-Nutzung über Speicher    =  268 kWh
Zwischenspeicherung         =  313 kWh (nach Ladeverlust)
Vollzyklen pro Jahr         =  312 der effektiven Kapazität

PV-Eigenverbrauch           =  493 kWh
Netzeinspeisung             =  134 kWh
PV-Eigenverbrauchsanteil    =   75 % des Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =   16 % des Verbrauchs (Autarkiegrad)
-->
<!--
TODO check/update ./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 600 -peff 92 -tmy -capacity 2500 -dc -pass spill 0 -feed 110 18..6

Speicherkapazität           = 2500 Wh mit max. Ladehöhe 90%, max. Entladetiefe 90%, DC-gekoppelt
Speicher-Umgehung           =    0 W und für Überschuss, max. Laderate 1 C
Konstanteinspeisung         =  110 W von 18 bis 6 Uhr, max. Entladerate 1 C
Verlust durch Überlauf      =    0 kWh
Ladeverlust                 =   27 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =   21 kWh durch Speicher-Wirkungsgrad 95%
PV-Nutzung über Speicher    =  363 kWh
Zwischenspeicherung         =  445 kWh (nach Ladeverlust)
Vollzyklen pro Jahr         =  222 der effektiven Kapazität

PV-Eigenverbrauch           =  503 kWh
Netzeinspeisung             =  109 kWh
PV-Eigenverbrauchsanteil    =   76 % des Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =   17 % des Verbrauchs (Autarkiegrad)
-->

{:style="clear:both"}

[![Bild: Balkonkraftwerk mit Speicher - Solaranlage](
Balkonkraftwerk_mit_Speicher.jpg){:.right width="350"}](
https://www.youtube.com/watch?v=f-iz6WE8GD8)
Um die Einspeisung automatisch in Abhängigkeit vom Ladezustand der Batterie
ein- und auszuschalten, kann man auch einen recht simplen
[programmierbaren Batteriespannungswächter](Komp.md#Spannungswächter) verwenden,
wie im [Video von Dimitri](https://www.youtube.com/watch?v=f-iz6WE8GD8) gezeigt.

Der Spannungswächter wird so eingestellt,
dass er beim Erreichen einer Batteriespannung, die
z.B. annähernd einer Vollladung entspricht, den Wechselrichter einschaltet und
z.B. in der Nähe der Batterie-Entladeschlussspannung diesen wieder ausschaltet.

Wie [oben ausgeführt](#Ladung) haben allerdings Anlagen mit Konstanteinspeisung
wie die gerade erwähnten Bastellösungen von Tobias Volk (PV&E) und von
Dimitri selbst mit zusätzlicher Überschussableitung eine miserable Rentabilität.


##### Lastgeregelte Einspeisung {#lastgeregelt}

Deutlich effizienter als eine [Konstanteinspeisung](#Konstanteinspeisung)
ist es, das Ausspeisen aus einer Speicherbatterie ins Wechselstromnetz
lastabhängig zu machen und damit eine Nulleinspeisung zu realisieren.

{:style="clear:both"}

[![Bild: Y&H Sun-1000 GTIL Netzwechselrichter mit Limiter.png](
Sun-1000_GTIL_Wechselrichter_mit_Limiter.png){:.right width="500"}](
https://www.youtube.com/watch?v=jPgWE-qQ3SE&t=1012s)
Ein Netzwechselrichter mit eingebauter lastbasierter Strom-Begrenzungs-Regelung,
engl. _Grid Tie Inverter with Limiter (GTIL)_ wie der [Sun GTIL](
https://de.aliexpress.com/item/32840070519.html) von Y&H
oder ein ähnliches Gerät von [Soyosource](
https://mona-stefan.de/index.php?option=com_content&view=article&id=765)
<!--, gibt es mit 1000 und 2000&nbsp;W Leistung -->
ermöglicht eine einphasige Nulleinspeisung ohne Basteln und Programmieren.
Man muss nur den Limiter-Sensor im Unterverteiler (Sicherungskasten)
an der Phase anbringen, über die die Einspeisung laufen soll.
Dann lässt sich der Wechselrichter so einstellen, dass er maximal so viel
einspeist wie zum Ausgleich der aktuellen Last auf dieser Phase benötigt wird,
wie [von Dimitri vorgeführt](https://youtu.be/jPgWE-qQ3SE).
Für dreiphasige Anwendung ist gedacht, je Phase ein solches Gerät einzusetzen,
was sich eher nur für größere Anlagen lohnt. Man kann sich aber auch
einen 3-Phasen-Sensor für ein Gerät zusammenstricken, etwa wie [hier](
https://www.photovoltaikforum.com/thread/193693-sun1000-gti-nulleinspeisung-mit-3-phasen-limiter/?pageNo=1)
beschrieben.

Am Elegantesten und Flexibelsten, aber **deutlich aufwendiger** ist es,
einen per Software regelbaren Netzwechselrichter zu verwenden.
Wenn in die Regelung ein elektronisch auslesbarer möglichst
[dreiphasiger Lastsensor](SV.md#Gesamtstrom) eingebunden wird,
lässt sich die Einspeisung abhängig vom aktuellen Stromverbrauch (mit einer
gewissen Verzögerung) etwa über [OpenDTU-OnBattery](#OpenDTU-OnBattery)
<!-- einen mit einer Heimautomatisierung entsprechend programmierten Raspberry Pi-->
so regeln, dass eine Nulleinspeisung erreicht wird.
Mehr zum Thema Automatisierungssoftware im Abschnitt zur
[Implementierung einer Speicher-Regelung](#Regelungsimplementierung).

[![Bild: Balkonsolar mit Akku - AkkuDoktor](
Balkonsolar_AkkuDoktor.png){:.center}](
https://www.youtube.com/watch?v=yOcoux9IbzM)
Eine Möglichkeit wäre, vor einen Netzwechselrichter einen elektronisch
regelbaren DC-DC-Wandler zu hängen, z.B. den [Joy-IT DPM8616](
https://www.idealo.de/preisvergleich/ProductCategory/10314.html?q=DPM8616),
wobei die Regelung den aktuellen Verbrauch über einen
[„Volkszähler“](https://www.volkszaehler.org/) mitgeteilt bekommt, wie in einem
[Video von Andreas Schmitz](https://www.youtube.com/watch?v=yOcoux9IbzM)
vorgeführt, aber das diente eigentlich nur Demonstration der Idee.

{:style="clear:both"}

Inzwischen recht weit verbreitet ist,
einen Hoymiles Wechselrichter zu verwenden und über sein
[DTU-Interface](https://www.hoymiles.com/de/products/microinverter/dtu/)
(*Datenübertragungseinheit*,
engl. *data transfer unit* oder allgemein *telemetry gateway*)
die nicht-permanente Limitierung seiner Ausgangsleistung zu regeln.
Hierbei ist es wichtig, nicht die permanente Limitierung zu verwenden, weil das
mit der Zeit den dafür intern verwendenten Flash-Speicher schädigen würde.

[![Bild: DTUs im Weckglas](
DTUs_im_Weckglas.jpg){:.right width="330"}](
https://blog.helmutkarger.de/balkonkraftwerk-teil-8-opendtu-und-ahoydtu-fuer-hoymiles-wechselrichter/)
An einem Netzwechselrichter der Hoymiles HM-Serie und für manche TSUN-Geräte
kann man anstelle der teuren proprietären DTU die offene
Bastel-Lösung [OpenDTU](https://github.com/roastedelectrons/HoymilesOpenDTU)
bzw. [AhoyDTU](https://ahoydtu.de/) verwenden. Für beide Varianten gibt es
schöne Anleitungen wie [diese](
https://blog.helmutkarger.de/balkonkraftwerk-teil-8-opendtu-und-ahoydtu-fuer-hoymiles-wechselrichter/)
und hilfreiche Videos auf YouTube wie [dieses](https://youtu.be/YJM913e0tiQ).
Wer nicht selbst die Elektronik zusammenlöten kann oder will, findet z.B. auf
[eBay-Kleinanzeigen](https://www.ebay-kleinanzeigen.de/s-hoymiles-dtu-ahoy/k0)
[![Bild: Hardware für OpenDTU](
OpenDTU_wiring_ESP32.png){:.left width="230"; margin-right: 20px"}](
https://github.com/tbnobody/OpenDTU)
auch betriebsfertige Geräte ab 30€, Bausätze ab 20€. Man kann sie sowohl zum
[Auslesen](https://www.heise.de/select/ct/2022/24/2224315343257577596)
der PV-Ertrags- und Geräte- Daten als auch zum [Steuern](
https://community.symcon.de/t/modul-beta-hoymiles-modulwechselrichter-mit-opendtu/130965)
des Wechselrichters verwenden.

Leider ist die Reaktionszeit eines Hoymiles-WR auf Änderungen des
(relativen oder absoluten) Limits recht lang und auch noch sehr ungleichmäßig:
er braucht meist etwa 5 bis 10, teils aber auch über 20 Sekunden,
um den eingestellten Wert (hoffentlich) zu erreichen.
Und wenn man zu schnell (z.B. nach 3 Sekunden) wieder neue Limit-Werte setzt,
verhält er sich teils chaotisch.
So ist durch seine Trägheit keine sehr flinke und exakte Regelung möglich.\
Zudem kommt es beim Betrieb an einer 24&nbsp;V Batterie bei höheren Limit-Werten
(also im oberen Leistungsbereich) teils zu [groben Abweichungen vom Sollwert](
https://www.photovoltaikforum.com/thread/221194-hm-400-an-batterie-limitierung-%C3%BCber-opendtu-eigenartig/?postID=3660691#post3660691).
Um Feedback über die tatsächliche aktuelle Ausgangsleistung des Hoymiles zu
erhalten, sollte man da auch nicht den über die DTU gelieferten Daten trauen,
weil sie besonders bei höheren Werten stark von der Realität abweichen.
Stattdessen kann man sehr gut z.B. einen Shelly Plus 1PM verwenden,
welcher verlässliche Daten im Sekundentakt bietet.

{:style="clear:both"}

[![Bild: ESP und RS485 für Soyosource](
ESP8266_Rs485_Modul2.png){:.left width="400"}](
https://github.com/KlausLi/Esp-Soyosource-Controller)
Eine [alternative Lösung](https://github.com/KlausLi/Esp-Soyosource-Controller)
mit dreiphasiger Lastmessung ermöglicht der [Soyosource 1200](
https://mona-stefan.de/index.php?option=com_content&view=article&id=765)
in der Variante mit Limiter, wobei der mitgelieferte einphasige Lastsensor hier
nicht verwendet wird. Stattdessen wird ein ESP8266 Mikrocontroller
an einem RS485-Adapter zur Steuerung mit einer fertigen Software verwendet,
wobei er die Lastinformation per WLAN von einem Shelly 3EM erhält.

{:style="clear:both"}

Ohne eigene Programmierung und Gebastel kommt man mit
dem [Tentek Tribune EMS](#Tentek) aus.

<!-- falsch:
Die Maximalleistung der bedarfsgerechten Einspeisung sollte möglichst hoch sein.
Bei einer z.B. auf 600&nbsp;W begrenzten Einspeisung beträgt für die o.g.
[Balkonanlage mit 1&nbsp;kWh Pufferspeicher und Überschussableitung](#Ladung)
die Steigerung des Eigenverbrauch durch die Speichernutzung 128&nbsp;kWh auf 588&nbsp;kWh.
Hier findet nur noch eine minimale Netzeinspeisung von 3&nbsp;kWh statt,
welche aus ungenutzter Überschussableitung resultiert.
Allerdings wird die Batterie im Schnitt pro Tag fast zweimal auf- und entladen
(655 Vollzyklen im Jahr), was neben größerer Degradation
zu erheblichen Lade- und Speicherverlusten von 39 + 31&nbsp;kWh führt.\
Eine Erhöhung der nutzbaren Speicherkapazität bringt praktisch nichts,
und eine Verringerung auf 0,5&nbsp;kWh liefert etwas weniger: 560&nbsp;kWh.
-->
<!--
TODO check/update ./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 600 -peff 92 -capacity 1250 -dc -tmy -pass spill 0 -feed lim 600

Speicherkapazität           = 1250 Wh mit max. Ladehöhe 90%, max. Entladetiefe 90%, DC-gekoppelt
Speicher-Umgehung           =    0 W und für Überschuss, max. Laderate 1 C
Maximaleinspeisung          =  600 W, max. Entladerate 1 C
Verlust durch Überlauf      =    0 kWh
Ladeverlust                 =   39 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =   31 kWh durch Speicher-Wirkungsgrad 95%
PV-Nutzung über Speicher    =  585 kWh
Zwischenspeicherung         =  655 kWh (nach Ladeverlust)
Vollzyklen pro Jahr         =  655 der effektiven Kapazität

PV-Eigenverbrauch           =  588 kWh
Netzeinspeisung             =    2 kWh
PV-Eigenverbrauchsanteil    =   89 % des Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =   20 % des Verbrauchs (Autarkiegrad)
-->
<!--
TODO check/update ./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 600 -peff 92 -capacity 2500 -dc -tmy -pass spill 0 -feed lim 600
Lastprofil-Datei            : Lastprofil_4673_kWh.csv
Grundlast                   =  184 W
Maximallast                 =13795 W am 2010-02-26 um 06:55 h

PV-Daten-Datei              : Timeseries_48.215_11.727_SA2_1kWp_crystSi_0_38deg_0deg_2005_2020.csv, enthaltene System-Effizienz 100% wurde übersteuert
Neigungswinkel, Azimut      = 38°, 0°
Breitengrad, Längengrad     = 48.215, 11.727
Simuliertes PV-Jahr         = TMY (2008..2020)

PV-Nominalleistung          =  600 Wp
Max. PV-Bruttoleistung      =  607 W am TMY (2008..2020)-04-15 um 13:00 h
PV-Bruttoertrag             =  764 kWh, PV-System-Wirkungsgrad 92%
Max. PV-Nettoleistung       =  525 W am TMY (2008..2020)-04-15 um 13:00 h
PV-Nettoertrag              =  660 kWh bei Wechselrichter-Wirkungsgrad 94%

Verbrauch durch Haushalt    = 3000 kWh

Speicherkapazität           = 2500 Wh mit max. Ladehöhe 90%, max. Entladetiefe 90%, DC-gekoppelt
Speicher-Umgehung           =    0 W und für Überschuss, max. Laderate 1 C
Maximaleinspeisung          =  600 W, max. Entladerate 1 C
Verlust durch Überlauf      =    0 kWh
Ladeverlust                 =   40 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =   31 kWh durch Speicher-Wirkungsgrad 95%
PV-Nutzung über Speicher    =  590 kWh
Zwischenspeicherung         =  660 kWh (nach Ladeverlust)
Vollzyklen pro Jahr         =  330 der effektiven Kapazität

PV-Eigenverbrauch           =  590 kWh
Netzeinspeisung             =    0 kWh
PV-Eigenverbrauchsanteil    =   89 % des Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =   20 % des Verbrauchs (Autarkiegrad)
-->
<!--
TODO check/update ./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 600 -peff 92 -capacity 625 -dc -tmy -pass spill 0 -feed lim 600

Speicherkapazität           =  625 Wh mit max. Ladehöhe 90%, max. Entladetiefe 90%, DC-gekoppelt
Speicher-Umgehung           =    0 W und für Überschuss, max. Laderate 1 C
Maximaleinspeisung          =  600 W, max. Entladerate 1 C
Verlust durch Überlauf      =    0 kWh
Ladeverlust                 =   33 kWh durch Lade-Wirkungsgrad 94%
Speicherverlust             =   26 kWh durch Speicher-Wirkungsgrad 95%
PV-Nutzung über Speicher    =  495 kWh
Zwischenspeicherung         =  554 kWh (nach Ladeverlust)
Vollzyklen pro Jahr         =  1109 der effektiven Kapazität

PV-Eigenverbrauch           =  560 kWh
Netzeinspeisung             =   42 kWh
PV-Eigenverbrauchsanteil    =   85 % des Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =   19 % des Verbrauchs (Autarkiegrad)
-->

### Inselanlage (mit Batteriespeicherung) {#Inselanlage}

![Bild: Aufbau Inselanlage](Inselanlage.png){:.right width="400"}
Alternativ zur
Einspeisung ins Hausnetz kann man den von den Solarmodulen gelieferten
Strom auch in einer Batterie speichern und bei Bedarf darüber Geräte
unabhängig vom Hausnetz mit Strom versorgen. Diese Betriebsart wird als
[*Inselanlage*](http://www.inselanlage.info/) (engl. _off-grid_)
bezeichnet und ist für die Nutzung ohne externes Stromnetz (also z.B.
bei Stromausfall, beim Campen mit dem Wohnmobil oder Wohnwagen, auf
Booten und für abseits gelegene Häuser oder Hütten) die einzig mögliche.
Als Notstromversorgung bei Stromausfall sind Batterien allerdings nur bedingt
geeignet, weil sie bei einem längeren Stromausfall (engl. _blackout_) zu wenig
Kapazität haben (es seid denn, es scheint dann genug Sonne zum Nachladen), aber
bei kürzeren Stromausfällen (engl. _brownout_) können sie sehr hilfreich sein.

Neben der Speicherbatterie wird hier zumindest ein
[Solar-Laderegler](Komp.md#Laderegler) benötigt,
welcher die PV-Module DC-seitig koppelt.

Verbraucher werden am Effizientesten mit dem Gleichstrom der Batterie betrieben.
Sollte die Batteriespannung (z.B. 12&nbsp;V oder 24&nbsp;V) dafür nicht passen,
können [Gleichspannungswandler](Komp.md#Gleichspannungswandler) verwendet werden,
die natürlich ausreichend dimensioniert und möglichst verlustarm sein sollten.
Auch Geräte (wie z.B. Laptops und Radios), die ein externes Netzteil haben,
lassen sich relativ leicht direkt mit Gleichstrom versorgen.

Zum Anschluss sonstiger Verbraucher, welche mit dem üblichen „Steckdosenstrom“
betrieben werden, braucht man einen ausreichend leistungsstarken
[Inselwechselrichter](Komp.md#Inselwechselrichter) zur Umwandlung in 230&nbsp;V Wechselstrom.\
An diesen Wechselrichter muss man bei Stromausfall alle
dann zu verwendenden Geräte (meist über eine Mehrfachsteckdose) anschließen.
Man speist dann also nicht einfach ins stromlose Hausnetz ein,
weil dazu die von außen kommende Stromleitung umgeschaltet werden und für eine
geeignete Erdung gesorgt werden müsste, was nur ein Elektriker machen sollte.

Ähnlich wie die o.g. [Batteriepufferung](#Batteriepuffer) ist diese Nutzungsart
flexibler, aber wegen der nötigen zusätzlichen Komponenten (v.A. der Batterie)
auch deutlich teurer und auch etwas anfälliger und wartungsintensiver
als die [direkte Netzeinspeisung](SSG.md#SSG).
Wirtschaftlich rentabel für die Nutzung zu Hause kann das bei den
derzeitigen Preisen nur sein, wenn man eine geeignete Batterie schon aus
anderen Gründen (z.B. für den mobilen Einsatz in einem Fahrzeug) hat und
die zusätzliche Nutzungsart auch zeitlich alternativ dazu möglich ist.

### Kombination aus Hausnetzeinspeisung und Inselanlage {#Kombination}

Wenn man Zugang zum Stromnetz hat und die für die betreffenden Varianten nötigen
Funktionen gleichzeitig installiert sind, kann man zwischen Netz-, Puffer- und
Inselbetrieb auch bedarfsweise wechseln. Dabei wird der Ausgang
der Solarmodule zwischen dem netzgekoppelten Wechselrichter und dem
Solar-Laderegler umgeschaltet (oder ohne Schalter einfach umgestöpselt) bzw.
am Ausgang der Batterie zwischen Netz- und Insel-Wechselrichter umgeschaltet.


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
LocalWords: operating temperature Timeseries crystSi PVCalculator and NPB
LocalWords: with entnahme bend OSO SSW SSO ready anlagen plugin date int limits
LocalWords: author today abstract This the ignored extension yaml txt interface
LocalWords: metadata add Austria description bagatellgrenze Loadprofiles
LocalWords: Yong Hui Green SolarPower backup net metering MPP Tracker SusEnergy
LocalWords: created changed nbsp pvroi ac dc break even fig SoC DoD MW Premium
LocalWords: Sense is end index output md ref of pv px Eff vs discussioncomment
LocalWords: my var pl zip load capacity feed spill deg magazine OC SC
LocalWords: data transfer solar cut cells open short circuit voltage lim
LocalWords: Ruecklaufsperre mdash Ueberlastung overpaneling LocalWords OW Heat
LocalWords: Bestrahlungsstaerke curves under different levels irradiation state
LocalWords: Microinverter What are Amps Volts SMF charge discharge Un Ent shunt
LocalWords: protector Micro Eco Worthy ISolar SPH GYVRM Cocar version cron job
LocalWords: Delivered Latest Downgraded shelly emeter file status returned MYPV
LocalWords: Zweirichtungszaehler issuecomment collect Notifications height ELWA
LocalWords: Plugs comments January Settings ons configuration states excl comp
LocalWords: sensor export float uksa tamorix custom firmware en Central zell TR
LocalWords: 
-->
