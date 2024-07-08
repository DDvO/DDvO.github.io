---
title: "Photovoltaik - Mini-Solaranlagen für daheim und unterwegs"
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
-   [Photovoltaik und ihr möglicher Ertrag](#Photovoltaik)
    -   [Sonneneinstrahlung](#Sonneneinstrahlung)
    -   [Nennleistung und Jahresertrag](#Nennleistung)
    -   [Optimale Ausrichtung von Solarmodulen](#Ausrichtung)
        - [Aufteilung in mehrere Orientierungen](#Aufteilung)
-   [Stromverbrauch und Einspeisung im Haushalt](SV.md)
-   [Eigenverbrauch und seine Berechnung](EV.md)
-   [Nutzungsvarianten](SSG.md#Nutzung)
    -   [Direkte Netzeinspeisung (Steckersolargerät SSG, „Balkonkraftwerk“)](SSG.md#SSG)
    -   [Hausnetzeinspeisung mit Speicherbatterie](Speicher.md)
    -   [Inselanlage (mit Batteriespeicherung) und Kombination](Insel.md)
-   [Auswahl und Nutzung von Komponenten](Komp.md)
-   [Beispiel-Konfigurationen](Bsp.md)

Photovoltaik und ihr möglicher Ertrag {#Photovoltaik}
-----------------------------------------------------

Mit Solarzellen kann man Sonnenlicht in elektrische Energie umwandeln,
woraus sich auch die Bezeichnung *Photovoltaik (PV)* ableitet.

Leider ist diese Art der Stromgewinnung nicht besonders effizient.
Das [erste Photovoltaikmodul](
https://www.photovoltaik4all.de/seit-wann-gibt-es-photovoltaik) wurde 1883
von Charles Fritts entwickelt und hatte einen Wirkungsgrad von 1%.
Der [Wirkungsgrad](https://de.wikipedia.org/wiki/Solarzelle#Wirkungsgrad)
der heutzutage üblichen Photovoltaik-Technologie mit Siliziumzellen liegt
bei 18 bis 20%, wobei teilweise wohl auch 22% erreicht werden.
Wenn man nicht sehr mit Platz sparen muss, lohnt es sich allerdings kaum,
für einen wenige Prozentpunkte höheren Wirkungsgrad mehr Geld auszugeben.

Abgesehen vom Wirkungsgrad gibt es in der Praxis Verluste, die davon abhängen,
wie alt die PV-Module sind, wie sehr
ihre Ausrichtung von der aktuellen Einstrahlungsrichtung der Sonne abweicht
(wobei senkrechte Einstrahlung natürlich optimal, aber selten erreichbar ist),
wie stark sie verschattet und/oder verschmutzt sind und wie warm sie sind.
Die altersbedingten Verluste (*Degradation*) steigen ziemlich linear etwa 0,5%
pro Jahr, so dass sich bei einer projektierten Gesamt-Verwendungsdauer von 20
Jahren eine durchschnittliche Degradation (also nach 10 Jahren) von 5% ergibt.
Auch der termperaturbedingte Verlust ist praktisch linear und liegt je nach
Zelltyp bei insgesamt etwa 10%, wenn die Modultemperatur beispielsweise 55°C
beträgt, also 30°C über der Temperatur bei [*Standard-Testbedingungen (STC)*](
https://photovoltaiksolarstrom.com/photovoltaiklexikon/noct/) von 25°C.
Genaueres dazu z.B. [hier](
https://joint-research-centre.ec.europa.eu/pvgis-photovoltaic-geographical-information-system/getting-started-pvgis/pvgis-data-sources-calculation-methods_en#ref-5-calculation-of-pv-power-output).

Zu berücksichtigen ist zudem der elektrische Wirkungsgrad der übrigen PV-Anlage
(also z.B. von Wechselrichter, Leitungen, ggf. Batterie) von etwa 80 bis 95%.

Das Hauptproblem der Photovoltaik ist allerdings viel grundlegender, nämlich
die am Erdboden oft nicht oder nur schwach verfügbare Sonneneinstrahlung.

### Sonneneinstrahlung {#Sonneneinstrahlung}

<!--
[![Bild: Globalstrahlung in Deutschland](
Globalstrahlung_Deutschland.jpg){:.right width="500"
style="margin-left: 10px; margin-right: 0px"}](
https://solargis.com/maps-and-gis-data/download/germany)
-->
Die von Solarzellen abgegebene Leistung hängt ziemlich linear
von der Intensität der Einstrahlung durch die Sonne ab.

Die Strahlungsleistung der Sonne auf unseren Planeten außerhalb der Atmosphäre
(also ohne Dämpfung durch Luftmoleküle, Wolken und Schmutz)
senkrecht zum Sonnenstand [berechnet sich zu 1367&nbsp;W/m²](
https://www.photovoltaik4all.de/wie-kann-man-die-solarstrahlung-berechnen)
und wird als *terrestrische Solarkonstante* bezeichnet.
Die Stärke der tatsächlich auf den Erdboden treffende Sonneneinstrahlung,
welche als [*Globalstrahlung*](https://de.wikipedia.org/wiki/Globalstrahlung)
(engl. _global horizontal irradiance_, _GHI_), bezeichnet wird, ist natürlich
viel geringer.
Der 30-Jahres-Mittelwert in Deutschland liegt bei [etwa 125&nbsp;W/m²](
https://www.solaranlage-ratgeber.de/photovoltaik/photovoltaik-leistung/photovoltaik-ertrag-in-sommer-und-winter).
Sie hängt stark vom Standort auf der Erde ab und ist je nach Bewölkung,
Tages- und Jahreszeit sehr variabel.
An einem wolkenlosen Sommertag werden maximal etwa 900&nbsp;W/m² erreicht, bei
leichter Bewölkung mit teils reflektierter Strahlung [bis über 1000&nbsp;W/m²](
https://www.photovoltaik4all.de/blog/welche-rolle-spielt-die-temperatur-einer-photovoltaikanlage).
Bei sehr schlechtem Wetter kann der Strahlungswert unter 100&nbsp;W/m² sinken.

[![Bild: Globalstrahlung in Deutschland 1991-2020](
Globalstrahlung_Deutschland_1991-2020.png){:.center}](
https://www.dwd.de/DE/leistungen/solarenergie/strahlungskarten_mvs.html#buehneTop)

Die Karten [des DWD](
https://www.dwd.de/DE/leistungen/solarenergie/strahlungskarten_mvs.html#buehneTop)
und [von Solargis](https://solargis.com/maps-and-gis-data/download)
geben einen Überblick, welche Summe an Globalstrahlung
pro Quadratmeter horizontaler Fläche durchschnittlich im Jahr zusammenkommt.
In Deutschland sind es im Schnitt der Jahre 1991 bis 2020 nach Berechnungen
des Deutschen Wetterdienstes [1086&nbsp;kWh/m²](
https://www.dwd.de/DE/leistungen/_config/leistungsteckbriefPublication.pdf?view=nasPublication&nn=16102&imageFilePath=229809516383478732006435024051472532772736564919904973098512541260476561304284049751405651717289583982040495528279338628905695385542275499557266335698545506612756450227783221602239879972072419602639476858490617241105588560029118312992778838770436569905341248614940063541966138585151325296158670892628008524799090834749&download=true).

[![Bild: Direktstrahlung und Diffusstrahlung](
Direktstrahlung-Diffusstrahlung.png){:.center width="798"}](
https://solargis.com/maps-and-gis-data/download/germany)
Das Sonneneinstrahlung erreicht uns nicht nur auf direktem Wege.
Sie wird auch durch die Erdatmosphäre gestreut und trifft
als *Diffusstrahlung* auf die Erde, selbst wenn die *Direktstrahlung*
durch Wolken oder feste Hindernisse abgeschattet wird.
Die Diffusstrahlung ist nahezu richtungsunabhängig und macht
im Jahresschnitt fast die Hälfte der Globalstrahlung auf die Horizontale aus.
Auf eine 40° nach Süden geneigte Fläche sind es gut 40% der Gesamtstrahlung.
Der Anteil der von der Erdoberfläche (z.B. durch Wolkenspiegelung oder Schnee)
auf die Fläche reflektierten Strahlung liegt dann bei knapp 2%.

### Nennleistung und Jahresertrag {#Nennleistung}

{:style="clear:both"}
Die **Nennleistung** (engl. _nominal power_, _power rating_) von Solarmodulen
wird in **Wp** ([*Watt Peak*](https://de.wikipedia.org/wiki/Watt_Peak)) angegeben.
Zu ihrer Bestimmung verwendet man eine Referenzbestrahlung mit einem normierten
Sonnenlichtspektrum einer Stärke von 1000&nbsp;W/m² bei Zelltemperatur 25°C.
Diese _standard test conditions (STC)_ sind [ziemlich praxisfern](
https://photovoltaiksolarstrom.com/photovoltaiklexikon/noct/#:~:text=STC%3A%20Idealbedingungen).
Realistischer sind die *Normalbedingungen* (engl. _nominal operating cell
temperature (NOCT)_) mit 45° Betriebstemperatur und 800&nbsp;W/m² Einstrahlung.

Bei näherer Betrachtung bedeutet die Nennleistung in kWp (also 1000&nbsp;Wp)
die *effektive Solarfläche* des Moduls, also Fläche (in m²) × Wirkungsgrad.
Daher lässt sich der Wirkungsgrad eines Solarmoduls sehr einfach nachrechnen,
indem man seine Nennleistung in kWp durch seine Fläche in m² teilt.
Für den Wirkungsgrad der verwendeten Solarzellen muss man von der Gesamtfläche
vorher die Ränder und Zwischenräume abziehen (typischerweise 5-10%).

Die Wp-Angaben für Solarmodule sind mit Vorsicht zu genießen ---
hauptsächlich weil die tatsächliche Leistung wie oben erwähnt
stark von der Situation (Ausrichtung im Vergleich zum Sonnenstand, Bewölkung,
Verschattung usw.) abhängig und meist deutlich geringer ist. Außerdem weil
besonders chinesische Händler von flexiblen Solarmodulen dazu tendieren,
[bei den Leistungsangaben deutlich zu übertreiben](
https://www.youtube.com/watch?v=JjmKgrtEMqk). Daher lohnt sich als
Plausibiltäts-Check, den Wirkungsgrad nachzurechnen.

In unseren Breitengraden ist je nach Standort bei optimaler statischer
Ausrichtung der Solarmodule ein Jahres-Ertrag von 1100&nbsp;kWh pro kWp installierter
PV-Nennleistung möglich. Manche Angaben dazu sind mit [etwa 900 bis 1000&nbsp;kWh](
https://www.energie-experten.org/erneuerbare-energien/photovoltaik/planung/ertrag)
eher zu konservativ bzw. etwas veraltet, andere sehr optimistisch mit
[bis zu 1200 bis 1300&nbsp;kWh](https://gruenes.haus/photovoltaik-pv-ertrag/).
Es kommt schlichtweg darauf an, welche Werte man bei der Globalstrahlung
ansetzt (je nach Standort, in Deutschland in Jahressumme [etwa 1090&nbsp;kWh/m²](
https://www.dwd.de/DE/leistungen/_config/leistungsteckbriefPublication.pdf?view=nasPublication&nn=16102&imageFilePath=229809516383478732006435024051472532772736564919904973098512541260476561304284049751405651717289583982040495528279338628905695385542275499557266335698545506612756450227783221602239879972072419602639476858490617241105588560029118312992778838770436569905341248614940063541966138585151325296158670892628008524799090834749&download=true))
und welche Annahmen man bzgl. Modul-Ausrichtung und Anlagen-Wirkungsgrad trifft.
<!-- bzw. bei der
rechnerischen Zahl der [Volllaststunden](https://gammel.de/de/lexikon/volllaststunden/6288) pro Jahr (nämlich [standardmäßig 1000&nbsp;h/a](
https://www.photovoltaik4all.de/wie-kann-man-die-solarstrahlung-berechnen),
aber eher 1100&nbsp;h/a) bezogen auf die Standardstrahlung von 1000&nbsp;W/m².-->

[![Bild: PV-Potential in Europa](PVOUT_Europe.png){:.center}](
https://solargis.com/maps-and-gis-data/download/europe)
Der Jahresertrag lässt sich leicht näherungsweise berechnen,
und zwar durch Multiplikation der Nennleistung der PV-Module in kWp
mit dem [*spezifischen PV-Jahresertrag*](
https://solar-direktinvest.de/photovoltaik/photovoltaik-investieren/spezifischer-jahresertrag-pv/) (engl. [_PV potential_, *PVOUT*](
https://globalsolaratlas.info/global-pv-potential-study)) in&nbsp;kWh/kWp.
Dieser ist standortspezifisch und beinhaltet Annahmen zu typischen praktisch
relevanten Faktoren wie den Verlust durch Verschmutzung und Wechselrichtung.\
Man erhält diese auch *spezifischer Ertrag* genannte Kenngröße aus den
groben [Karten von Solargis](https://solargis.com/maps-and-gis-data/download),
aus dem [Global Solar Atlas der Weltbank](
https://globalsolaratlas.info/map?c=50.10,11.05,7&s=48.1807,11.604e)
(auch von Solargis) oder am Genauesten aus der [PVGIS-Datenbank der EU](
https://re.jrc.ec.europa.eu/pvg_tools/de/)
bei der Standard-Eingabe von 1&nbsp;kWp für die installierte max. PV-Leistung.

### Optimale Ausrichtung von Solarmodulen {#Ausrichtung}

Die Leistung von Solarmodulen hängt vor Allem von der Direktstrahlung ab ---
und zwar nicht nur von ihrer Intensität, sondern auch davon, wie sehr ihre
Fläche auf den aktuellen Sonnenstand ausgerichtet ist.
Dabei geht es um die zur Modulfläche senkrechte Komponente der Direktstrahlung,
also um den Faktor Kosinus der Winkelabweichung vom Lot auf die Modulfläche.

Mit der Diffusstrahlung,
welche wie oben erwähnt von der Richtung der Direktstrahlung unabhängig ist
und einen erstaunlich großen Anteil an der Gesamtstrahlung ausmacht,
können Solarzellen leider nicht sehr viel anfangen. Für diesen also
effektiv geringen Anteil wäre eine waagerechte Anordnung optimal.

![Bild: PV-Potential nach Ausrichtung von Solarmodulen](
Ausrichtung_PV-Potential.png){:width="392" }
![Bild: Ertragsanteil nach Ausrichtung von Solarmodulen](
Ausrichtung_Ertragsanteil.png){:width="385" .right}
Den [besten Jahres-Gesamtertrag](
https://machdeinenstrom.de/optimaler-ertrag-mit-mini-solar-kraftwerken/)
bekommt man in süddeutschen Breitengraden bei Orientierung genau nach Süden
und mit ca. 38° Neigung (also Winkel relativ zur Waagerechten).
Genaueres kann man z.B. über
[PVGIS](https://re.jrc.ec.europa.eu/pvg_tools/de/) (oder einfacher über
[Solarserver](https://www.solarserver.de/pv-anlage-online-berechnen/))
standortspezifisch anhand von Geo- und Klimadaten berechnen/simulieren,
wobei **es auf ein paar Grad hin oder her nicht ankommt**.

![Bild: Jahresertrag nach Ausrichtung von Solarmodulen](
Jahresertrag_nach_Ausrichtung.png){:.center}
Diese Grafik zeigt sehr schön die relative Änderung des Jahres-Gesamtertrages
einer PV-Anlage mit zunehmender Winkel-Abweichung von Süden (*Azimut*)
abhängig vom Neigungswinkel, wenn der optimale Neigungswinkel 35° beträgt.
Sie wurde von [bonotos](https://www.bonotos.com/) erzeugt,
basierend auf [Daten von Prof. Konrad Mertens](
https://www.fh-muenster.de/eti/downloads/personen/professoren/mertens/frei/2022_05_31_FH-MS_Nachhaltigkeitstag_Vortrag_Solarenergie_Kein_Dach_ohne_Solarstrom_PDF.pdf)
von der FH Münster.

Beim PV-Ertrag und entsprechenden Simulationen ist zu beachten, dass dabei
üblicherweise **der Jahres-Gesamtertrag** betrachtet und optimiert wird.
Dieser **unterliegt der Annahme, dass man den zur jeweiligen Tageszeit
(und Jahreszeit) erzeugten Strom auch immer gleichmäßig nutzen kann**,
sei es durch direkten [Eigenverbrauch](EV.md#Eigenverbrauch),
Zwischenspeicherung (was allerdings auch Verluste mit sich bringt)
oder vergütete Einspeisung (die aber leider selten attraktiv ist).\
Wenn man --- wie mit den meisten Steckersolargeräten --- den erzeugten Strom
nur direkt im Haushalt verbrauchen kann und der Rest ins externe Netz geht,
sollte man das Nutzungsprofil berücksichtigen, welches auch auch
[*Lastprofil*](https://www.energie-lexikon.info/lastprofil.html) genannt wird.

![Bild: Ertrags-Nutzungsanteil nach Ausrichtung von Solarmodulen](
Ausrichtung_Eigennutzungsanteil.png){:width="500" .right}
Durch [genaue Simulation](EV.md#SolBatSim) für durchschnittliche
Haushalts-Tages-Nutzungsprofile zeigt sich, dass
**eine Abweichung von der optimalen Ausrichtung
deutlich weniger Einbußen beim selbst genutzten Jahres-Gesamtertrag bringt**.
So liegt bei südlicher Ausrichtung, aber senkrechter Anbringung
im Verhältnis zur optimalen Neigung 35° die Einbuße beim Eigenverbrauch
nicht bei 30% vom Optimum, sondern je nach Lastprofil bei 23%.
Die Eigenverbrauchs-Einbuße durch Anbringung auf der West- oder Ostseite
liegt mit senkrechter Anbringung bei 46% und mit 35° Neigung bei 17%.

|   Azimut  | Neigung | Nettoertrag | Einbuße | Eigenverbrauch| Einbuße |
|--------------:|:----|------------:|--------:|--------------:|--------:|
|   W/O: +/-90° | 90° |   323 kWh   |   51%   |  252 kWh      |  46%    |
|   W/O: +/-90° | 35° |   522 kWh   |   21%   |  385 kWh      |  17%    |
| SW/SO: +/-45° | 90° |   432 kWh   |   36%   |  336 kWh      |  28%    |
| SW/SO: +/-45° | 35° |   623 kWh   |    6%   |  449 kWh      |   3%    |
|       Süd: 0° | 90° |   463 kWh   |   30%   |  357 kWh      |  23%    |
|       Süd: 0° | 35° |   661 kWh   |    0%   |  464 kWh      |   0%    |
|:-------------:|:----|------------:|--------:|--------------:|--------:|

Man hat also zur Ausrichtung seiner Solarmodule
bezüglich Eigenverbrauch größere Flexibilität als allgemein angenommen.

<!--
./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 600 -peff 92

Neigungswinkel              =   35°
Azimut                      =    0°
Breitengrad                 =   48.215
Längengrad                  =   11.727

PV-Nominalleistung          =  600 Wp
Max. PV-Bruttoleistung      =  650 W am 2020-03-23 um 12:00 h
PV-Bruttoertrag             =  764 kWh
PV-Nettoertrag              =  661 kWh bei PV-System-Eff. 92%, Wechselrichter-Eff. 94%

Verbrauch durch Haushalt    = 3000 kWh
PV-Eigenverbrauch           =  464 kWh

./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_90deg_0deg_2005_2020.csv 600 -peff 92

Neigungswinkel              =   90°
Azimut                      =    0°

PV-Nominalleistung          =  600 Wp
Max. PV-Bruttoleistung      =  608 W am 2005-02-13 um 13:00 h
PV-Bruttoertrag             =  535 kWh
PV-Nettoertrag              =  463 kWh bei PV-System-Eff. 92%, Wechselrichter-Eff. 94%
PV-Eigenverbrauch           =  357 kWh
-->

<!--
./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_45deg_2005_2020.csv 600 -peff 92

Neigungswinkel              =   35°
Azimut                      =   45°
Breitengrad                 =   48.215
Längengrad                  =   11.727

PV-Nominalleistung          =  600 Wp
Max. PV-Bruttoleistung      =  623 W am 2020-03-24 um 13:00 h
PV-Bruttoertrag             =  721 kWh
PV-Nettoertrag              =  623 kWh bei PV-System-Eff. 92%, Wechselrichter-Eff. 94%

Verbrauch durch Haushalt    = 3000 kWh
PV-Eigenverbrauch           =  449 kWh

./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_90deg_45deg_2005_2020.csv 600 -peff 92

Neigungswinkel              =   90°
Azimut                      =   45°

PV-Nominalleistung          =  600 Wp
Max. PV-Bruttoleistung      =  644 W am 2005-02-14 um 15:00 h
PV-Bruttoertrag             =  499 kWh
PV-Nettoertrag              =  432 kWh bei PV-System-Eff. 92%, Wechselrichter-Eff. 94%

Verbrauch durch Haushalt    = 3000 kWh
PV-Eigenverbrauch           =  336 kWh
-->

<!--
./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_35deg_-90deg_2005_2020.csv 600 -peff 92

Neigungswinkel              =   35°
Azimut                      =  -90°
Breitengrad                 =   48.215
Längengrad                  =   11.727

PV-Nominalleistung          =  600 Wp
Max. PV-Bruttoleistung      =  556 W am 2020-05-06 um 09:00 h
PV-Bruttoertrag             =  604 kWh
PV-Nettoertrag              =  522 kWh bei PV-System-Eff. 92%, Wechselrichter-Eff. 94%
PV-Eigenverbrauch           =  385 kWh

./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_14_90deg_-90deg_2005_2020.csv 600 -peff 92

Neigungswinkel              =   90°
Azimut                      =  -90°

PV-Nominalleistung          =  600 Wp
Max. PV-Bruttoleistung      =  513 W am 2020-03-23 um 08:00 h
PV-Bruttoertrag             =  374 kWh
PV-Nettoertrag              =  323 kWh bei PV-System-Eff. 92%, Wechselrichter-Eff. 94%

Verbrauch durch Haushalt    = 3000 kWh
PV-Eigenverbrauch           =  252 kWh
-->

Wer aus irgendeinem Grund (etwa wegen der Befestigung) eine möglichst flache
Neigung der PV-Module wählt, sollte trotzdem mindestens 12° verwenden,
um eine Selbstreinigung der Moduloberflächen durch Niederschlag zu ermöglichen.

Wenn man Solarmodule (z.B. auf dem Dach eines Wohnmobils) in waagerechter Lage
anbringt, ist man von der Orientierung (Himmelsrichtung) unabhängig.
Allerdings kommen nach meiner Erfahrung
billige flexible PV-Module selbst mittags an sehr sonnigen Tagen
kaum über die Hälfte der angegebenen Spitzenleistung hinaus.

#### Aufteilung in mehrere Orientierungen {#Aufteilung}

Seit vielen Jahren hält sich in der Community hartnäckig die Legende,
eine Aufteilung in zwei Orientierungen, z.B. die klassische
Ost-West-Ausrichtung oder irgendwo dazwischen nach Südosten und Südwesten,
sei günstig, um auf die Vormittags- und Nachmittagssonne zu optimieren.
Aber dieser Mythos wurde bereits/spätestens [im Februar 2014 widerlegt](
https://www.photovoltaikforum.com/thread/97856-mythos-eigenverbrauchsoptimierung-mit-ost-west-ausrichtung/).

**Jegliche Abweichung von der Südausrichtung mindert den Jahresertrag**,
und auch **für den Jahres-Eigenverbrauch lohnt sich eine Ost-West-Aufteilung
nicht wirklich**,
selbst wenn man den Ertragsüberschuss über die Mittagszeit kaum nutzen kann.
* Das liegt vor Allem daran, dass die Menge der Direktstrahlung aus südlichen
Richtungen in Summe über den Tag und übers Jahr viel höher ist --
die Sonne scheint von dort einfach stärker und häufiger (besonders im Winter)
als von weiter östlich oder westlich.
* Außerdem ist zwar morgens der Ertrag bei östlicher Ausrichtung höher,
aber der Ertrag gleichzeitig auf westlicher Seite umso geringer,
und gegen Abend entsprechend umgekehrt.
<!--
https://www.photovoltaikforum.com/core/attachment/44638-pv-vergleich-s-vs-ow-v2-pdf/
-->
* Bei niedrigem Sonnenstand, wo die Ost-West-Aufteilung Vorteile bringen soll,
ist die Tendenz zur Verschattung und damit Minderertrag viel größer.

<!--
https://www.photovoltaikforum.com/thread/97856-mythos-eigenverbrauchsoptimierung-mit-ost-west-ausrichtung/?postID=1050024#post1050024
-->
<!--
* Nachdem bei Ost-West-Ausrichtung oft eine stärkere Neigung gewählt wird
(anscheinend, weil sie als günstiger angesehen wird, aber ist das wirklich so?
Ich sehe besonders beim Ertrag, weniger beim Eigenverbrauch, das Gegenteil),
bringen sie bei Diffuslicht weniger:
Steil geneigte Anlagen „schauen“ teilweise in den dunklen Horizont, während
flach geneigte Anlagen bei diffusem Licht mehr vom hellen Himmel „sehen“.
https://www.photovoltaikforum.com/thread/97856-mythos-eigenverbrauchsoptimierung-mit-ost-west-ausrichtung/?postID=1049926#post1049926
-->
[![Bild: Vergleich Ertrag bei Süd- und O-W-Ausrichtung bei 30° Dachneigung](
PV_Vergleich_S_vs_OW_v2.png)](
https://www.photovoltaikforum.com/core/attachment/44638-pv-vergleich-s-vs-ow-v2-pdf/)

Diese Effekte werden selbst dann nicht durch eine geringere Nutzbarkeit tagsüber
ausgeglichen, wenn der Haushalt an Arbeitstagen von 8 bis 16 Uhr nur eine
[Minimallast (Grundlast)](SV.md#Strommessung) von z.B. 100&nbsp;W hat:
Dann hat die Ost-West-Ausrichtung im Sommer einen leichten Vorteil, aber zu
allen anderen Jahreszeiten ermöglicht die Südausrichtung mehr Eigenverbrauch.\
Erst wenn täglich von 8 bis sogar 18 Uhr nur z.B. 50&nbsp;W Grundlast vorliegt,
bringt eine Ost-West-Ausrichtung einen geringen Vorteil beim Eigenverbrauch.
Allerdings bewegt sich dann der Eigenverbrauch bei nur 200&nbsp;kWh im Jahr,
weshalb sich die Amortisation deutlich länger hinzieht als im Durchschnitt.

Leider wird die falsche Vorstellung, dass durch Ost-West-Anlagen
der Eigenverbrauch „oftmals zusätzlich angehoben werden kann“,
immer noch durch diverse Publikationen gefördert --
selbst von professionellen Stellen wie
[PV Austria](https://pvaustria.at/pv-ausrichtung/),
die es eigentlich besser wissen müssten. Das hat vermutlich folgende Gründe:
* Kommerzieller und energiepolitischer Grund:
Besitzer von Häusern mit nach Ost/West geneigten Dächern,
bei denen also aus baulichen Gründen eine Südausrichtung nicht möglich ist,
sollen stärker motiviert werden, sich auch eine PV-Anlage anzuschaffen.
* Energiepolitischer Grund (Stichwort *Systemdienlichkeit*):
Durch mehr Ost-West-Ausrichtung in einer Region wird eine gleichmäßigere
Verteilung der Gesamt-PV-Leistung über den Tagesverlauf erreicht, indem eine
mittägliche Überproduktion teilweise auf morgens und abends verlagert wird.

<!--
https://www.photovoltaikforum.com/thread/97856-mythos-eigenverbrauchsoptimierung-mit-ost-west-ausrichtung/?postID=1046716#post1046716
* Unverständnis von Entscheidungsträgern über die physikalischen Gegebenheiten.
-->

Bei Verwendung vieler Module ist ein Vorteil der geteilten Ost-West-Ausrichtung,
dass man auf einer gegebenen Grundfläche mehr Modulfläche unterbringen kann --
bei 30° Neigung theoretisch 15% mehr. Allerdings zu höheren Kosten (auch pro Wp)
und mit mehr Tendenz zur Verschattung zu den Zeiten direkterer Einstrahlung.
<!--
https://www.photovoltaikforum.com/thread/97856-mythos-eigenverbrauchsoptimierung-mit-ost-west-ausrichtung/?postID=1050021#post1050021
https://www.photovoltaikforum.com/thread/97856-mythos-eigenverbrauchsoptimierung-mit-ost-west-ausrichtung/?postID=1050024#post1050024
-->
Obwohl eine geteilte Ausrichtung im Vergleich zur reinen Südausrichtung nur
in besonderen Ausnahmefällen mehr bringt, schadet sie ansonsten aber auch wenig,
wenn man sie (etwa aus baulichen Gründen) trotzdem wählt, besonders wenn man
tagsüber im Vergleich zu den Morgen- und Abendstunden eher wenig Verbrauch hat.

Die genannten Auswirkungen auf den Eigenverbrauch sind
das Ergebnis einer Reihe [genauer Simulationen](EV.md#SolBatSim)
für einen Haushalt in Süddeutschland mit 3000&nbsp;kWh Jahresverbrauch mit einem
Steckersolargerät mit 2 × 300&nbsp;Wp PV-Modulen und Gesamtsystem-Wirkungsgrad 86%.\
Für die Ausrichtungen -/+ 90° (also Ost/West), +/- 60°, +/- 30° und 0° (Süd)
zeigt die folgende Tabelle den PV-Nettoertrag und den Eigenverbrauch (EV)
in den angegebenen Situationen, wobei für jede Ausrichtung der jeweils
maximale Eigenverbrauch **fett** dargestellt ist,
womit sich auch die jeweils optimale Neigung leicht ablesen lässt.

|Azimut|Neigung|Nettoertrag|EV normal|EV Mo-Fr 8-16&nbsp;h 100&nbsp;W|EV tgl. 8-18&nbsp;h 50&nbsp;W|
|------:|:-----|----------:|-----------:|------------:|----------:|
|Ost/West:
|-/+90° |  15° |  549 kWh  | **462 kWh**|   367 kWh   |  186 kWh  |
|-/+90° |  30° |  531 kWh  |   457 kWh  | **369 kWh** |  193 kWh  |
|-/+90° |  45° |  512 kWh  |   442 kWh  |   365 kWh   |**195 kWh**|
|WSW/OSO:
|+/-60° |  15° |  585 kWh  |   480 kWh  |   374 kWh   |  185 kWh  |
|+/-60° |  30° |  592 kWh  | **487 kWh**| **380 kWh** |  190 kWh  |
|+/-60° |  45° |  575 kWh  |   480 kWh  |   378 kWh   |**191 kWh**|
|SSW/SSO:
|+/-30° |  15° |  610 kWh  |   491 kWh  |   379 kWh   |**182 kWh**|
|+/-30° |  30° |  636 kWh  | **502 kWh**| **382 kWh** |**182 kWh**|
|+/-30° |  45° |  631 kWh  |   497 kWh  |   377 kWh   |  181 kWh  |
|rein Süd:
|    0° |  15° |  620 kWh  |   495 kWh  |   380 kWh   |**181 kWh**|
|    0° |  30° |  652 kWh  | **506 kWh**| **382 kWh** |  177 kWh  |
|    0° |  45° |  647 kWh  |   499 kWh  |   373 kWh   |  172 kWh  |
|------:|-----:|----------:|-----------:|------------:|----------:|

Interessant ist in diesem Zusammenhang auch zu betrachten,
wie sich die Unterschiede über die Jahreszeiten verteilen.

* Wenn man täglich von 8 bis 18 Uhr eine Grundlast von nur 50&nbsp;W hätte,
würde sich bei 30° Neigung der Eigenverbrauch saisonal wie folgt verteilen,
wobei die Ost-/West-Aufsplittung außer im Winter etwas besser abschneidet:

|Azimut| Frühjahr |  Sommer  |  Herbst  |  Winter  | Summe   |
|-----:|---------:|---------:|---------:|---------:|--------:|
| O/W  |**49 kWh**|**70 kWh**|**48 kWh**|  26 kWh  | 193 kWh |
| Süd  |  46 kWh  |  59 kWh  |  45 kWh  |**27 kWh**| 177 kWh |
|-----:|---------:|---------:|---------:|---------:|--------:|


* Wenn man an Arbeitstagen (Mo - Fr) tagsüber von 8 bis 16 Uhr
nur eine Grundlast von 100&nbsp;W hat, verteilt sich bei optimaler Neigung von 30°
der Eigenverbrauch saisonal wie folgt:

[//]: #

|Azimut| Frühjahr |  Sommer   |  Herbst   |  Winter  | Summe   |
|-----:|---------:|----------:|----------:|---------:|--------:|
| O/W  |  94 kWh  |**141 kWh**|   96 kWh  |  38 kWh  | 369 kWh |
| Süd  |**98 kWh**|  136 kWh  |**101 kWh**|**47 kWh**| 382 kWh |
|-----:|---------:|----------:|----------:|---------:|--------:|

[//]: #
Also kann bei tagsüber nur Grundlast die Ost-/West-Ausrichtung im Sommer
für den Eigenverbrauch etwas günstiger sein, aber zu den übrigen Jahreszeiten
(Herbst, Winter und Frühjahr)
ist normalerweise die reine Südausrichtung etwas günstiger.\
Daher könnte man ein paar Euro sparen, wenn man (z.B. auf einem Flachdach)
bewegliche Module hat, indem man sie normalerweise alle nach Süden richtet
und im Sommer nach Westen und/oder Osten dreht.

* Bei normalem Lastprofil (also wenn man auch tagsüber nicht nur Grundlast hat)
lohnt sich jedoch nicht einmal eine saisonale Aufteilung,
denn dann verteilt sich bei 30° Neigung der Eigenverbrauch wie folgt:

|Azimut|  Frühjahr |  Sommer   |  Herbst   |  Winter  | Summe   |
|-----:|----------:|----------:|----------:|---------:|--------:|
| O/W  |  116 kWh  |**181 kWh**|  122 kWh  |  38 kWh  | 457 kWh |
| Süd  |**130 kWh**|  180 kWh  |**139 kWh**|**57 kWh**| 506 kWh |
|-----:|----------:|----------:|----------:|---------:|--------:|


<!--
https://www.mydealz.de/comments/permalink/39540050
https://www.mydealz.de/comments/permalink/40256532

Variante extrem (Ost-West) gespreizt

./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_45deg_90deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_45deg_-90deg_2005_2020.csv 300 -tmy # -load 130  # -load 43 7:8..18
 # -load 93 7:8..18 ergäbe 100 W

Neigungswinkel  =  45° Azimut =  90°
Neigungswinkel  =  45° Azimut = -90°
PV-Bruttoertrag =  595 kWh
PV-Nettoertrag  =  512 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  442 kWh
Eigenverbrauch  =  365 kWh wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
Eigenverbrauch  =  195 kWh (opt.) wenn täglich 8-18 Uhr 50 W Verbrauch
-->
<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_40deg_90deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_40deg_-90deg_2005_2020.csv 300 -tmy # -load 130 # -load 43 7:8..18

Neigungswinkel  =  40° Azimut =  90°
Neigungswinkel  =  40° Azimut = -90°
PV-Bruttoertrag =  595 kWh
PV-Nettoertrag  =  512 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  449 kWh
-->
<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_40deg_90deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_40deg_-90deg_2005_2020.csv 300 -tmy -bend 1,1,1,1,2,2,2,2,.5,.5,.5,.5,.5,.5,.5,.5,2,2,2,2,1,1,1,1
PV-Eigenverbrauch           =  348 kWh
-->
<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_35deg_90deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_35deg_-90deg_2005_2020.csv 300 -tmy # -load 130 # -load 43 7:8..18

Neigungswinkel  =  35° Azimut =  90°
Neigungswinkel  =  35° Azimut = -90°
PV-Bruttoertrag =  607 kWh
PV-Nettoertrag  =  522 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  448 kWh
-->

<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_30deg_90deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_30deg_-90deg_2005_2020.csv 300 -tmy # -load 130 # -load 43 7:8..18

Neigungswinkel  =  30° Azimut =  90°
Neigungswinkel  =  30° Azimut = -90°
PV-Bruttoertrag =  617 kWh
PV-Nettoertrag  =  531 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  457 kWh
                   Frühjahr 116, Sommer 181, Herbst 122, Winter 38
Eigenverbrauch  =  369 kWh (opt.) wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
                   Frühjahr 94, Sommer 141, Herbst 96, Winter 38
Eigenverbrauch  =  193 kWh wenn täglich 8-18 Uhr 50 W Verbrauch
                   Frühjahr 49, Sommer 70, Herbst 48, Winter 26
-->
<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_25deg_90deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_25deg_-90deg_2005_2020.csv 300 -tmy # -load 130 # -load 43 7:8..18

Neigungswinkel  =  25° Azimut =   90°
Neigungswinkel  =  25° Azimut =  -90°
PV-Bruttoertrag =  625 kWh
PV-Nettoertrag  =  538 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  459 kWh
-->
<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_20deg_90deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_20deg_-90deg_2005_2020.csv 300 -tmy # -load 130 # -load 43 7:8..18

Neigungswinkel  =  20° Azimut =   90°
Neigungswinkel  =  20° Azimut =  -90°
PV-Bruttoertrag =  633 kWh
PV-Nettoertrag  =  544 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  461 kWh
-->
<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_15deg_90deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_15deg_-90deg_2005_2020.csv 300 -tmy # -load 130 # -load 43 7:8..18

Neigungswinkel  =  15° Azimut =   90°
Neigungswinkel  =  15° Azimut =  -90°
PV-Bruttoertrag =  639 kWh
PV-Nettoertrag  =  549 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  462 kWh (opt.)
Eigenverbrauch  =  367 kWh wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
Eigenverbrauch  =  186 kWh wenn täglich 8-18 Uhr 50 W Verbrauch
-->

<!--
Variante stark gespreizt:

./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_45deg_60deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_45deg_-60deg_2005_2020.csv 300 -tmy # load 130 # -load 43 7:8..18

Neigungswinkel  =  45° Azimut =   60°
Neigungswinkel  =  45° Azimut =  -60°
PV-Bruttoertrag =  669 kWh
PV-Nettoertrag  =  575 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  480 kWh
Eigenverbrauch  =  378 kWh wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
Eigenverbrauch  =  191 kWh (opt. ) wenn täglich 8-18 Uhr 50 W Verbrauch
-->
<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_35deg_60deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_35deg_-60deg_2005_2020.csv 300 -tmy # load 130 # -load 43 7:8..18

Neigungswinkel  =  35° Azimut =   60°
Neigungswinkel  =  35° Azimut =  -60°
PV-Bruttoertrag =  684 kWh
PV-Nettoertrag  =  588 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  486 kWh
-->
<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_30deg_60deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_30deg_-60deg_2005_2020.csv 300 -tmy # -load 130 # -load 43 7:8..18

Neigungswinkel  =  30° Azimut =   60°
Neigungswinkel  =  30° Azimut =  -60°
PV-Bruttoertrag =  689 kWh
PV-Nettoertrag  =  592 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  487 kWh (opt.)
Eigenverbrauch  =  380 kWh (opt.) wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
Eigenverbrauch  =  190 kWh wenn täglich 8-18 Uhr 50 W Verbrauch
-->
<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_25deg_60deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_25deg_-60deg_2005_2020.csv 300 -tmy # -load 130 # -load 43 7:8..18

Neigungswinkel  =  25° Azimut =   60°
Neigungswinkel  =  25° Azimut =  -60°
PV-Bruttoertrag =  689 kWh
PV-Nettoertrag  =  592 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  486 kWh
-->
<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_15deg_60deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_15deg_-60deg_2005_2020.csv 300 -tmy # -load 130 # -load 43 7:8..18

Neigungswinkel  =  15° Azimut =   60°
Neigungswinkel  =  15° Azimut =  -60°
PV-Bruttoertrag =  680 kWh
PV-Nettoertrag  =  585 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  480 kWh
Eigenverbrauch  =  374 kWh wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
Eigenverbrauch  =  185 kWh wenn täglich 8-18 Uhr 50 W Verbrauch
-->

<!--
Variante schwach gespreizt:

./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_45deg_30deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_45deg_-30deg_2005_2020.csv 300 -tmy # -load 130 # -load 43 7:8..18

Neigungswinkel  =  45° Azimut =   30°
Neigungswinkel  =  45° Azimut =  -30°
PV-Bruttoertrag =  731 kWh
PV-Nettoertrag  =  629 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  497 kWh
Eigenverbrauch  =  377 kWh wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
Eigenverbrauch  =  181 kWh wenn täglich 8-18 Uhr 50 W Verbrauch
-->
<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_35deg_30deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_35deg_-30deg_2005_2020.csv 300 -tmy # -load 130 # -load 43 7:8..18

Neigungswinkel  =  35° Azimut =  30°
Neigungswinkel  =  35° Azimut = -30°
PV-Bruttoertrag =  739 kWh
PV-Nettoertrag  =  635 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  502 kWh
-->
<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_30deg_30deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_30deg_-30deg_2005_2020.csv 300 -tmy # -load 130 -load 43 7:8..18

Neigungswinkel  =  30° Azimut =   30°
Neigungswinkel  =  30° Azimut =  -30°
PV-Bruttoertrag =  739 kWh
PV-Nettoertrag  =  636 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  502 kWh (opt.)
Eigenverbrauch  =  382 kWh (opt.) wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
Eigenverbrauch  =  182 kWh (opt.) wenn täglich 8-18 Uhr 50 W Verbrauch
-->
<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_25deg_30deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_25deg_-30deg_2005_2020.csv 300 -tmy # -load 130 # -load 43 7:8..18

Neigungswinkel  =  25° Azimut =   30°
Neigungswinkel  =  25° Azimut =  -30°
PV-Bruttoertrag =  733 kWh
PV-Nettoertrag  =  631 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  500 kWh
-->
<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_15deg_30deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_15deg_-30deg_2005_2020.csv 300 -tmy # -load 130 # -load 43 7:8..18

Neigungswinkel  =  15° Azimut =   30°
Neigungswinkel  =  15° Azimut =  -30°
PV-Bruttoertrag =  709 kWh
PV-Nettoertrag  =  610 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  491 kWh
Eigenverbrauch  =  379 kWh wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
Eigenverbrauch  =  182 kWh wenn täglich 8-18 Uhr 50 W Verbrauch
-->

<!--
Variante nicht gespreizt:

./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_45deg_0deg_2005_2020.csv 600 -tmy # -load 130 # -load 43 7:8..18

Neigungswinkel  =  45° Azimut = 0°
PV-Bruttoertrag =  753 kWh
PV-Nettoertrag  =  647 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  499 kWh
Eigenverbrauch  =  373 kWh wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
Eigenverbrauch  =  172 kWh wenn täglich 8-18 Uhr 50 W Verbrauch
-->
<!--

./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 600 -tmy # -load 130 # -load 43 7:8..18

Neigungswinkel  =  35° Azimut = 0°
PV-Bruttoertrag =  761 kWh
PV-Nettoertrag  =  655 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  506 kWh
-->
<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_30deg_0deg_2005_2020.csv 600 -tmy # -load 130 # -load 43 7:8..18

Neigungswinkel  =  30° Azimut = 0°
PV-Bruttoertrag =  758 kWh
PV-Nettoertrag  =  652 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  506 kWh (opt.)
                   Frühjahr 130, Sommer 180, Herbst 139, Winter 57
Eigenverbrauch  =  382kWh (opt.) wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
                   Frühjahr 98, Sommer 136, Herbst 101, Winter 47
Eigenverbrauch  =  177 kWh wenn täglich 8-18 Uhr 50 W Verbrauch
                   Frühjahr 46, Sommer 59, Herbst 45, Winter 27
-->
<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_25deg_0deg_2005_2020.csv 600 -tmy # -load 130 # -load 43 7:8..18

Neigungswinkel  =  25° Azimut = 0°
PV-Bruttoertrag =  749 kWh
PV-Nettoertrag  =  645 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  504 kWh
-->
<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_30deg_0deg_2005_2020.csv 600 -tmy -bend 1,1,1,1,2,2,2,2,.5,.5,.5,.5,.5,.5,.5,.5,2,2,2,2,1,1,1,1
-Eigenverbrauch =  357 kWh
-->
<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_20deg_0deg_2005_2020.csv 600 -tmy # -load 130 # -load 43 7:8..18

Neigungswinkel  =  20° Azimut = 0°
PV-Bruttoertrag =  737 kWh
PV-Nettoertrag  =  634 kWh bei PV-System-Eff. 91%, Wechselrichter-Eff. 94%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  501 kWh
-->
<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_15deg_0deg_2005_2020.csv 600 -tmy # -load 130 # -load 43 7:8..18

Neigungswinkel  =  15° Azimut = 0°
PV-Bruttoertrag =  721 kWh
PV-Nettoertrag  =  620 kWh bei PV-System-Eff. 91%, Wechselrichter-Eff. 94%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  495 kWh
Eigenverbrauch  =  380 kWh wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
Eigenverbrauch  =  181 kWh (opt.) wenn täglich 8-18 Uhr 50 W Verbrauch
-->

<!--
Variante Nord-Süd 50° Süd 20° Nord o.ä. bringt nichts
https://www.photovoltaikforum.com/thread/122364-ost-west-oder-besser-optimal-s%C3%BCd/?postID=1871373#post1871373 Favorit

./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_30deg_0deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_15deg_180deg_2005_2020.csv 300 -tmy # -load 130 # -load 43 7:8..18
Neigungswinkel  =  15° Azimut =  180°
Neigungswinkel  =  30° Azimut =    0°
PV-Bruttoertrag =  652 kWh
PV-Nettoertrag  =  561 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  467 kWh
Eigenverbrauch  =  366 kWh wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
Eigenverbrauch  =  181 kWh wenn täglich 8-18 Uhr 50 W Verbrauch
-->

**Also auch bei einem Verbrauchsprofil, das stark auf die Morgen- und
Abendstunden konzentriert ist, bringt eine Aufteilung der Modul-Ausrichtung
keinen Vorteil für den Eigenverbrauch.**
Dagegen spricht zusätzlich die Tendenz zu stärkerer Verschattung bei flacherem
Sonnenstand, etwa durch Gebäude und Bäume in der Umgebung
und auch durch die PV-Module gegenseitig (*Selbstverschattung*).
Außerdem ist die geteilte Montage meist aufwendiger.
Unterschiedliche Ausrichtungen erfordern zur Optimierung nur dann eine getrennte
[MPPT-Regelung](Komp.md#MPPT), wenn sich bei unterschiedlich starker Bestrahlung
die Modulspannung verschiebt, bei der die maximale Modulleistung erreicht wird.

[![Bild: Selbstverschattung gleichartiger Modulreihen](
PV_Vergleich_S_vs_OW_add_v1.png)](
https://www.photovoltaikforum.com/core/attachment/44467-pv-vergleich-s-vs-ow-add-v1-pdf/)

Was die für den Eigenverbrauch optimale Neigung der PV-Module
bei einer Anlage mit 600&nbsp;Wp betrifft, ergeben die Simulationen folgendes:
Bei reiner Südausrichtung (0° Azimut), ebenso bei einer Orientierung von +/- 30°
oder +/- 60° abweichend von Süden, ist eine Neigung von ungefähr 30° optimal.
Bei einer Orientierung von +/- 90° abweichend von Süden (also rein Ost-West)
ist bei einem normalen Lastprofil eine Neigung von ungefähr 15° am günstigen,
bei tagsüber nur Grundlast wieder 30° optimal.
Wobei eine Winkelabweichung von +/- 10° sehr wenig ausmacht.

Bei Verwendung von 4 PV-Modulen kann man im Sinne der Eigenverbrauchsoptimierung
und gleichmäßigeren Ertragsverteilung über den Tagesverlauf in Betracht ziehen,
eines nach Osten, zwei nach Süden und eines nach Westen auszurichten.
Bei 400&nbsp;Wp Modulen ergibt die [Eigenverbrauchssimulation](EV.md#SolBatSim), wieder
für ein typisches Lastprofil und 3000&nbsp;kWh Jahresverbrauch in Süddeutschland,
für alle drei Himmelsrichtungen eine optimale Neigung von um die 30°
mit wieder sehr geringer Empfindlichkeit auf Abweichungen davon.\
Die Verteilung 1 × Ost, 2 × Süd und 1 x West resultiert in einem Nettoertrag
von 1576&nbsp;kWh und einem Eigenverbrauch von 831&nbsp;kWh bei optimalen 30°.\
Hingegen bringt die gemeinsame Ausrichtung der 4 Module nach Süden
erwartungsgemäß einen deutlich höheren Gesamt-Nettoertrag von 1715&nbsp;kWh,
während der Eigenverbrauch von 838&nbsp;kWh nur noch minimal höher ist,
und zwar bei optimaler Neigung von 25°.
Wenn der Haushalt an Arbeitstagen von 8 bis 16 Uhr allerdings
nur eine Grundlast von z.B. 100&nbsp;W hat, hat die Aufteilung
auf drei Himmelsrichtungen beim Eigenverbrauch einen hauchdünnen Vorteil
von 3&nbsp;kWh (nämlich 629&nbsp;kWh gegenüber 626&nbsp;kWh bei reiner Südausrichtung),
und zwar bei optimaler Neigung von 25 bis 30° der südlichen Module
und 35 bis 40° der östlichen und westlichen Module.\
Also lohnt sich auch die weitere Aufteilung auf drei Himmelsrichtungen nicht
wirklich, zumal eine gemeinsame Montage meist einfacher und günstiger ist
(und auch weniger störend aussehen sollte).

<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_40deg_90deg_2005_2020.csv 400 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_40deg_-90deg_2005_2020.csv 400 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_25deg_0deg_2005_2020.csv 800 -curb 1200 # -load 130
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_35deg_90deg_2005_2020.csv 400 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_35deg_-90deg_2005_2020.csv 400 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_30deg_0deg_2005_2020.csv 800 -curb 1200 # -load 130
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_30deg_90deg_2005_2020.csv 400 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_30deg_-90deg_2005_2020.csv 400 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_30deg_0deg_2005_2020.csv 800 -curb 1200 # load 130
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_25deg_90deg_2005_2020.csv 400 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_25deg_-90deg_2005_2020.csv 400 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_25deg_0deg_2005_2020.csv 800 -curb 1200 # -load 130

40°+25°
PV-Nominalleistung = 1600 Wp = 400+400+800 Wp
PV-Bruttoertrag    = 1793 kWh
PV-Nettoertrag     = 1542 kWh bei PV-System-Eff. 91%, Wechselrichter-Eff. 94%
PV-Ertragsverlust  =    0 kWh während 0 h durch Drosselung auf 1200 W
Verbrauch Haushalt = 3000 kWh
Eigenverbrauch mit =  829 kWh
Eigenverbrauch mit =  630 kWh wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
Eigenverbrauchsv.  =    0 kWh netto während 0 h durch Drosselung auf 1200 W

35°+30° opt. für tagsüber Grundlast
PV-Nominalleistung = 1600 Wp = 400+400+800 Wp
PV-Bruttoertrag    = 1820 kWh
PV-Nettoertrag     = 1566 kWh bei PV-System-Eff. 91%, Wechselrichter-Eff. 94%
PV-Ertragsverlust  =    0 kWh während 0 h durch Drosselung auf 1200 W
Verbrauch Haushalt = 3000 kWh
Eigenverbrauch mit =  831 kWh
Eigenverbrauch mit =  629 kWh wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
Eigenverbrauchsv.  =    0 kWh netto während 0 h durch Drosselung auf 1200 W

30°
PV-Nominalleistung = 1600 Wp = 400+400+800 Wp
PV-Bruttoertrag    = 1833 kWh
PV-Nettoertrag     = 1576 kWh bei PV-System-Eff. 91%, Wechselrichter-Eff. 94%
PV-Ertragsverlust  =    0 kWh während 2 h durch Drosselung auf 1200 W
Verbrauch Haushalt = 3000 kWh
Eigenverbrauch mit =  831 kWh
Eigenverbrauch mit =  628 kWh wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
Eigenverbrauchsv.  =    0 kWh während 0 h durch Drosselung auf 1200 W

25°
PV-Nominalleistung = 1600 Wp = 400+400+800 Wp
PV-Bruttoertrag    = 1833 kWh
PV-Nettoertrag     = 1576 kWh bei PV-System-Eff. 91%, Wechselrichter-Eff. 94%
PV-Ertragsverlust  =    0 kWh während 3 h durch Drosselung auf 1200 W
Verbrauch Haushalt = 3000 kWh
Eigenverbrauch mit =  829 kWh
Eigenverbrauch mit =  627 kWh wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
Eigenverbrauchsv,  =    0 kWh netto während 0 h durch Drosselung auf 1200 W
-->

<!--
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_35deg_0deg_2005_2020.csv 1600 -curb 1200 # -load 130
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_30deg_0deg_2005_2020.csv 1600 -curb 1200 # -load 130
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_25deg_0deg_2005_2020.csv 1600 -curb 1200 # -load 130
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_20deg_0deg_2005_2020.csv 1600 -curb 1200 # -load 130
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_15deg_0deg_2005_2020.csv 1600 -curb 1200 # -load 130

35°
PV-Nominalleistung = 1600 Wp
PV-Bruttoertrag    = 2030 kWh
PV-Nettoertrag     = 1739 kWh bei PV-System-Eff. 91%, Wechselrichter-Eff. 94%
PV-Ertragsverlust  =    0 kWh während 5 h durch Drosselung auf 1200 W
Last Haushalt      = 3000 kWh
Eigenverbrauch mit =  835 kWh
Eigenverbrauch mit =  621 kWh wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
Eigenverbrauchsv.  =    0 kWh während 5 h durch Drosselung auf 1200 W

30°
PV-Nominalleistung = 1600 Wp
PV-Bruttoertrag    = 2023 kWh
PV-Nettoertrag     = 1734 kWh bei PV-System-Eff. 91%, Wechselrichter-Eff. 94%
PV-Ertragsverlust  =    6 kWh während 106 h durch Drosselung auf 1200 W
Last Haushalt      = 3000 kWh
Eigenverbrauch mit =  837 kWh
Eigenverbrauch mit =  624 kWh wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
Eigenverbrauchsv.  =    0 kWh während 5 h durch Drosselung auf 1200 W

25°
PV-Nominalleistung = 1600 Wp
PV-Bruttoertrag    = 1999 kWh
PV-Nettoertrag     = 1715 kWh bei PV-System-Eff. 91%, Wechselrichter-Eff. 94%
PV-Ertragsverlust  =    4 kWh während 84 h durch Drosselung auf 1200 W
Verbrauch Haushalt = 3000 kWh
Eigenverbrauch mit =  838 kWh
Eigenverbrauch mit =  626 kWh wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
Eigenverbrauchsv.  =    0 kWh netto während 3 h durch Drosselung auf 1200 W

20°
PV-Nominalleistung = 1600 Wp
PV-Bruttoertrag    = 1966 kWh
PV-Nettoertrag     = 1688 kWh bei PV-System-Eff. 91%, Wechselrichter-Eff. 94%
PV-Ertragsverlust  =    3 kWh während 62 h durch Drosselung auf 1200 W
Verbrauch Haushalt = 3000 kWh
Eigenverbrauch mit =  853 kWh
Eigenverbrauch mit =  625 kWh wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
Eigenverbrauchsv.  =    0 kWh netto während 2 h durch Drosselung auf 1200 W

15°
PV-Nominalleistung = 1600 Wp
PV-Bruttoertrag    = 1923 kWh
PV-Nettoertrag     = 1652 kWh bei PV-System-Eff. 91%, Wechselrichter-Eff. 94%
PV-Ertragsverlust  =    0 kWh während 38 h durch Drosselung auf 1200 W
Verbrauch Haushalt = 3000 kWh
Eigenverbrauch mit =  821 kWh
Eigenverbrauch mit =  624 kWh wenn Mo-Fr 8-16 Uhr 100 W Verbrauch
Eigenverbrauchsv.  =    0 kWh netto während 2 h durch Drosselung auf 1200 W
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
