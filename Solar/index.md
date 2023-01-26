---
title: "Mini-Solaranlagen für daheim und unterwegs"
lang: de
keywords:
- Photovoltaik
- Sonnenenergie
- Solarenergie
- Globalstrahlung
- Diffusstrahlung
- Solaranlage
- Steckersolaranlage
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
- Solarpanels
- Solarmodule
- Ausrichtung
- Speicherung
- Stromspeicher
- Batteriespeicher
- Pufferbatterie
- Spannungsregler
- Laderegler
- Wechselrichter
- Einspeisung
- Ertrag
- spezifisch
- PV-Jahresertrag
- Optimierung
- Nutzungsprofil
- Lastprofil
- Lastspitzen
- Abregelung
- Drosselung
- Kappungsverlust
- Eigenverbrauch
- Eigenverbrauchsanteil
- Eigendeckung
- Eigendeckungsanteil
- Autarkiegrad
- Batterieentladung
- Amortisation
- Ökologie
- Umwelt
---

# Zusammenfassung {#Zusammenfassung}

Mit einem sog. *Balkonkraftwerk* kann man sehr einfach und relativ günstig
Solarstrom gewinnen und über eine Steckdose direkt ins Hausnetz einspeisen.
Das spart Stromkosten und kann sich schon nach wenigen Jahren Betrieb rechnen,
allerdings nur soweit man den Strom auch gleichzeitig selbst verbraucht.
Weil diese Betriebsart den überschüssigen Strom an die Allgemeinheit weitergibt
und keine Batterie benötigt, ist sie für die ökologische Gesamtbilanz am besten.

Für eine gewisse Unabhängigkeit von der nicht ständig kräftig vorhandenen
Sonneneinstrahlung und vom allgemeinen Stromnetz
braucht man eine aufladbare Batterie als Stromspeicher und weitere Geräte,
was das Ganze aufwendiger und deutlich teurer macht. Damit lässt sich die
gewonnene Energie über den ganzen Tag und die Nacht verteilt einspeisen.
Eine sog. *Inselanlage* ist auch während Stromausfällen verwendbar,
soweit die Speicherkapazität und die Einstrahlung zum Nachladen reichen.

# Abgrenzung {#Abgrenzung}

Hier geht es nicht um *Solarthermie*, also die direkte Gewinnung von Wärme
durch Sonneneinstrahlung, sondern um die Erzeugung von elektrischem Strom.
Es geht hier auch nicht um "große" Photovoltaik-Anlagen z.B. auf Hausdächern
(dazu [hier ein fundierter Leitfaden](
https://solar.htw-berlin.de/wp-content/uploads/HTW-PV-Wegweiser.pdf)),
wobei die physikalischen und technischen Grundlagen natürlich die gleichen sind.

Außerdem kann ich als Privatperson und auch als naturwissenschaftlich-technisch
versierter Nichtprofi natürlich keine offiziellen Informationen bzw. absolut
verlässliche Hinweise geben und für die Inhalte keine Gewähr oder Haftung
übernehmen. Wer bezüglich steckerfertigen PV-Anlagen etwas Offizielleres sucht,
der sei z.B. auf den schönen [Leitfaden von SmartGridsBW](
https://smartgrids-bw.net/public/uploads/2020/04/IBZ-Leitfaden_Balkon-PV-Online.pdf)
und die ["Fachinformation" des DKE](https://www.dke.de/de/arbeitsfelder/energy/mini-pv-anlage-solar-strom-balkon-nachhaltig-erzeugen)
verwiesen.

<!-- markdown-toc start - Run M-x markdown-toc-refresh-toc -->
<!--
**Inhaltsverzeichnis**

- [Zusammenfassung {#Zusammenfassung}](#zusammenfassung-zusammenfassung)
- [Abgrenzung {#Abgrenzung}](#abgrenzung-abgrenzung)
    - [Inhaltsverzeichnis](#inhaltsverzeichnis)
    - [Photovoltaik und ihr möglicher Ertrag {#Photovoltaik}](#photovoltaik-und-ihr-möglicher-ertrag-photovoltaik)
        - [Sonneneinstrahlung {#Sonneneinstrahlung}](#sonneneinstrahlung-sonneneinstrahlung)
        - [Nennleistung und Jahresertrag {#Nennleistung}](#nennleistung-und-jahresertrag-nennleistung)
        - [Optimale Ausrichtung von Solarmodulen {#Ausrichtung}](#optimale-ausrichtung-von-solarmodulen-ausrichtung)
    - [Nutzungsmöglichkeiten {#Nutzung}](#nutzungsmöglichkeiten-nutzung)
        - [Direkte Netzeinspeisung (Stecker-Solaranlage, "Balkonkraftwerk") {#Balkonkraftwerk}](#direkte-netzeinspeisung-stecker-solaranlage-balkonkraftwerk-balkonkraftwerk)
            - [Beschränkung auf 600 bzw. 800 W und ihre Gründe {#Kappung}](#beschränkung-auf-600-w-und-ihre-gründe-kappung)
            - [Kappungsverlust durch Drosselung auf 600 W {#Kappungsverlust}](#kappungsverlust-durch-drosselung-auf-600-w-kappungsverlust)
            - [Stromzähler und Rücklaufsperre {#Stromzähler}](#stromzähler-und-rücklaufsperre-stromzähler)
        - [Stromverbrauch im Haushalt {#Stromverbrauch}](#stromverbrauch-im-haushalt-stromverbrauch)
            - [Verbrauchsmessung {#Verbrauchsmessung}](#verbrauchsmessung-verbrauchsmessung)
        - [Eigenverbrauch und Eigendeckung {#Eigenverbrauch}](#eigenverbrauch-und-eigendeckung)
        - [Ertragsberechnung und Amortisation {#Ertragsberechnung}](#ertragsberechnung-ertragsberechnung)
            - [Monatsbasierte Berechnung von Ertrag und Amortisation {#PV-Rechner}](#monatsbasierte-berechnung-von-ertrag-und-amortisation-pv-rechner)
            - [Speichersimulation {#Speichersimulation}](#speichersimulation-speichersimulation)
            - [Simulation auf Minutenbasis {#Minutenbasis}](#simulation-auf-minutenbasis-minutenbasis)
        - [Hausnetzeinspeisung mit Batteriepuffer {#Batteriepuffer}](#hausnetzeinspeisung-mit-batteriepuffer-batteriepuffer)
            - [Regelungsstrategien für Stromspeicher {#Regelungsstrategien}](#regelungsstrategien-fuer-stromspeicher)
            - [Speicherbatterie {#Speicherbatterie}](#speicherbatterie-speicherbatterie)
            - [Ladung der Batterie {#Batterieladung}](#batterieladung-batterieladung)
            - [Einspeisung aus der Batterie {#Einspeisung}](#einspeisung-aus-der-batterie-einspeisung)
        - [Inselanlage (mit Batteriespeicherung) {#Inselanlage}](#inselanlage-mit-batteriespeicherung-inselanlage)
        - [Kombination aus Hausnetzeinspeisung und Inselanlage {#Kombination}](#kombination-aus-hausnetzeinspeisung-und-inselanlage-kombination)
    - [Auswahl und Nutzung von Komponenten {#Komponenten}](#hinweise-für-die-auswahl-und-nutzung-von-komponenten-komponenten)
        - [Solarmodule {#Solarmodule}](#solarmodule-solarmodule)
            - [Elektrischer Anschluss {#Anschluss}](#anschluss-von-solarmodulen-anschluss)
            - [Montage {#Montage}](#montage-montage)
        - [Solar-Regler und Wechselrichter {#Wechselrichter}](#solar-regler-und-wechselrichter-wechselrichter)
            - [Netzwechselrichter {#Netzwechselrichter}](#netzwechselrichter-netzwechselrichter)
            - [Gleichspannungswandler {#Gleichspannungswandler}](#gleichspannungswandler-gleichspannungswandler)
            - [Inselwechselrichter {#Inselwechselrichter}](#inselwechselrichter-inselwechselrichter)
        - [Solar-Laderegler {#Laderegler}](#solar-laderegler-laderegler)
        - [Hybridgeräte: Solar-Laderegler mit Wechselrichter {#Hybrid}](#hybridgeräte-solar-laderegler-mit-wechselrichter-hybrid)
        - [Speicherbatterien {#Speicher}](#speicherbatterien-speicher)
            - [Batterie-Dimensionierung {#Dimensionierung}](#batterie-dimensionierung-dimensionierung)
            - [Batterie-Strukturierung {#Strukturierung}](#batterie-strukturierung-strukturierung)
            - [Kombination aus Batterie und Wechselrichter {#Kaskadierte}](#kombination-aus-batterie-und-wechselrichter-kaskadierte)
            - [Tiefsetzsteller {#Tiefsetzsteller}](#tiefsetzsteller-tiefsetzsteller)
            - [Spannungswächter {#Spannungswächter}](#spannungswächter-spannungswächter)
    - [Beispiel-Konfigurationen {#Konfigurationen}](#beispiel-konfigurationen-konfigurationen)
        - [Mobile Inselanlage {#Mobilanlage}](#mobile-inselanlage-mobilanlage)
        - [Stecker-Solaranlage {#Steckeranlage}](#stecker-solaranlage-steckeranlage)
        - [Kombi-Anlage {#Kombianlage}](#kombi-anlage-kombianlage)
-->
<!-- markdown-toc end -->

<!-- pandoc -s - -toc index.md -o output.md -->

# Inhaltsverzeichnis

-   [Zusammenfassung](#Zusammenfassung)
-   [Abgrenzung](#Abgrenzung)
-   [Inhaltsverzeichnis](#inhaltsverzeichnis)
-   [Photovoltaik und ihr möglicher Ertrag](#Photovoltaik)
    -   [Sonneneinstrahlung](#Sonneneinstrahlung)
    -   [Nennleistung und Jahresertrag](#Nennleistung)
    -   [Optimale Ausrichtung von Solarmodulen](#Ausrichtung)
-   [Nutzungsmöglichkeiten](#Nutzung)
    -   [Direkte Netzeinspeisung (Stecker-Solaranlage, "Balkonkraftwerk")](#Balkonkraftwerk)
        - [Beschränkung auf 600 bzw. 800 W und ihre Gründe](#Kappung)
        - [Kappungsverlust durch Drosselung auf 600 W](#Kappungsverlust)
        - [Stromzähler und Rücklaufsperre](#Stromzähler)
    -   [Stromverbrauch im Haushalt](#Stromverbrauch)
        - [Verbrauchsmessung](#Verbrauchsmessung)
    -   [Eigenverbrauch und Eigendeckung](Eigenverbrauch)
    -   [Ertragsberechnung und Amortisation](#Ertragsberechnung)
        - [Monatsbasierte Berechnung von Ertrag und Amortisation](#PV-Rechner)
        - [Speichersimulation](Speichersimulation)
        - [Simulation auf Minutenbasis](#Minutenbasis)
    -   [Hausnetzeinspeisung mit Batteriepuffer](#Batteriepuffer)
        - [Regelungsstrategien für Stromspeicher](#Regelungsstrategien)
        - [Speicherbatterie](#Speicherbatterie)
        - [Ladung der Batterie](#Batterieladung)
        - [Einspeisung aus der Batterie](#Einspeisung)
    -   [Inselanlage (mit Batteriespeicherung)](#Inselanlage)
    -   [Kombination aus Hausnetzeinspeisung und
        Inselanlage](#Kombination)
-   [Auswahl und Nutzung von Komponenten](#Komponenten)
    -   [Solarmodule](#Solarmodule)
        - [Elektrischer Anschluss](#Anschluss)
        - [Montage](#Montage)
    -   [Solar-Regler und Wechselrichter](#Wechselrichter)
        - [Netzwechselrichter](#Netzwechselrichter)
        - [Gleichspannungswandler](#Gleichspannungswandler)
        - [Inselwechselrichter](#Inselwechselrichter)
    -   [Solar-Laderegler](#Laderegler)
    -   [Hybridgeräte: Solar-Laderegler mit Wechselrichter](#Hybrid)
    -   [Speicherbatterien](#Speicher)
        - [Batterie-Dimensionierung}](#Dimensionierung)
        - [Batterie-Strukturierung](#Strukturierung)
        - [Kombination aus Batterie und Wechselrichter](#Kaskadierte)
        - [Tiefsetzsteller](#Tiefsetzsteller)
        - [Spannungswächter](#Spannungswächter)
-   [Beispiel-Konfigurationen](#Konfigurationen)
    -   [Mobile Inselanlage](#Mobilanlage)
    -   [Stecker-Solaranlage](#Steckeranlage)
    -   [Kombi-Anlage](#Kombianlage)

Photovoltaik und ihr möglicher Ertrag {#Photovoltaik}
--------------------------------------------------

Mit Solarzellen kann man Sonnenlicht in elektrischen Strom umwandeln,
woraus sich auch die Bezeichnung *Photovoltaik (PV)* ableitet.

Leider ist diese Art der Stromgewinnung nicht besonders effizient.
Das [erste Photovoltaikmodul](
https://www.photovoltaik4all.de/seit-wann-gibt-es-photovoltaik) wurde 1883
von Charles Fritts entwickelt und hatte einen Wirkungsgrad von 1%.
Der [Wirkungsgrad](https://de.wikipedia.org/wiki/Solarzelle#Wirkungsgrad)
der heutzutage üblichen Photovoltaik-Technologie mit Siliziumzellen liegt
bei 18 bis 20%, wobei besonders hochwertige Zellen etwa 22% erreichen.

Abgesehen vom Wirkungsgrad gibt es in der Praxis Verluste, die davon abhängen,
wie alt die PV-Module sind, wie sehr
ihre Ausrichtung von der aktuellen Einstrahlungsrichtung der Sonne abweicht
(wobei senkrechte Einstrahlung natürlich optimal, aber selten erreichbar ist),
wie stark sie verschattet und/oder verschmutzt sind und wie warm sie sind.
Die altersbedingte Degradation ist ziemlich linear und liegt bei etwa 0,5%
pro Jahr, so dass sich bei projektierten 20 Jahren Gesamt-Verwendungsdauer
nach 10 Jahren ein durchschnittlicher Verlust durch die Alterung von 5% ergibt.
Auch der termperaturbedingte Verlust ist praktisch linear und liegt je nach
Zelltyp bei etwa 10%, wenn die Modultemperatur beispielsweise 55°C beträgt,
also 30°C über der Standard-Temperatur von 25°C. Genaueres dazu z.B. [hier](
https://joint-research-centre.ec.europa.eu/pvgis-photovoltaic-geographical-information-system/getting-started-pvgis/pvgis-data-sources-calculation-methods_en#ref-5-calculation-of-pv-power-output).

Zu berücksichtigen ist zudem der elektrische Wirkungsgrad der übrigen PV-Anlage
(also z.B. von Wechselrichter, Kabeln, ggf. Batterie) von etwa 80 bis 95%.

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
senkrecht zum Sonnenstand [berechnet sich zu 1367 W/m²](
https://www.photovoltaik4all.de/wie-kann-man-die-solarstrahlung-berechnen)
und wird als *terrestrische Solarkonstante* bezeichnet.
Die Stärke der tatsächlich auf den Erdboden treffende Sonneneinstrahlung,
welche als [*Globalstrahlung*](https://de.wikipedia.org/wiki/Globalstrahlung)
(engl. _global horizontal irradiance_, _GHI_), bezeichnet wird, ist natürlich
viel geringer.
Der 30-Jahres-Mittelwert in Deutschland liegt bei [etwa 125 W/m²](
https://www.solaranlage-ratgeber.de/photovoltaik/photovoltaik-leistung/photovoltaik-ertrag-in-sommer-und-winter).
Sie hängt stark vom Standort auf der Erde ab und ist je nach Bewölkung,
Tages- und Jahreszeit sehr variabel.
An einem wolkenlosen Sommertag werden maximal etwa 900 W/m² erreicht, bei
leichter Bewölkung mit teils reflektierter Strahlung [bis über 1000 W/m²](
https://www.photovoltaik4all.de/blog/welche-rolle-spielt-die-temperatur-einer-photovoltaikanlage).
Bei sehr schlechtem Wetter kann der Strahlungswert unter 100 W/m² sinken.

[![Bild: Globalstrahlung in Deutschland 1991-2020](
Globalstrahlung_Deutschland_1991-2020.png){:.center}](
https://www.dwd.de/DE/leistungen/solarenergie/strahlungskarten_mvs.html#buehneTop)

Die Karten [des DWD](
https://www.dwd.de/DE/leistungen/solarenergie/strahlungskarten_mvs.html#buehneTop)
und [von Solargis](https://solargis.com/maps-and-gis-data/download)
geben einen Überblick, welche Summe an Globalstrahlung
pro Quadratmeter horizontaler Fläche durchschnittlich im Jahr zusammenkommt.
In Deutschland sind es im Schnitt der Jahre 1991 bis 2020 nach Berechnungen
des Deutschen Wetterdienstes [1086 kWh/m²](
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
Die **Nennleistung** von Solarmodulen wird in **Wp** ([*Watt Peak*](
https://de.wikipedia.org/wiki/Watt_Peak)) angegeben. Zu ihrer
Bestimmung verwendet man eine Referenzbestrahlung mit einem normierten
Sonnenlichtspektrum einer Stärke von 1000 W/m² bei Zelltemperatur 25°C.\
Bei näherer Betrachtung bedeutet die Nennleistung in kWp (also 1000 Wp)
die *effektive Solarfläche* des Moduls, also Fläche (in m²) ×
max. Wirkungsgrad.
Daher kann man auch den maximalen Wirkungsgrad eines Solarmoduls sehr
einfach nachrechnen, indem man seine Nennleistung in kWp durch seine
Fläche in m² teilt.

Die Wp-Angaben von Herstellern und Händlern für Solarmodule sind mit Vorsicht
zu genießen --- hauptsächlich weil die tatsächliche Leistung wie oben erwähnt
stark von der Situation (Ausrichtung im Vergleich zum Sonnenstand, Bewölkung,
Verschattung usw.) abhängig und meist deutlich geringer ist. Außerdem weil
besonders chinesische Händler von flexiblen Solarmodulen dazu tendieren,
bei den Leistungsangaben deutlich zu übertreiben. Daher lohnt sich als
Plausibiltäts-Check, den Wirkungsgrad nachzurechnen.

In unseren Breitengraden ist je nach Standort bei optimaler statischer
Ausrichtung der Solarmodule ein Jahres-Ertrag von 1100 kWh pro kWp installierter
PV-Nennleistung möglich. Manche Angaben dazu sind mit [etwa 900 bis 1000 kWh](
https://www.energie-experten.org/erneuerbare-energien/photovoltaik/planung/ertrag)
eher zu konservativ bzw. etwas veraltet, andere sehr optimistisch mit
[bis zu 1200 bis 1300 kWh](https://gruenes.haus/photovoltaik-pv-ertrag/).
Es kommt schlichtweg darauf an, welche Werte man bei der Globalstrahlung
ansetzt (je nach Standort, in Deutschland in Jahressumme [etwa 1090 kWh/m²](
https://www.dwd.de/DE/leistungen/_config/leistungsteckbriefPublication.pdf?view=nasPublication&nn=16102&imageFilePath=229809516383478732006435024051472532772736564919904973098512541260476561304284049751405651717289583982040495528279338628905695385542275499557266335698545506612756450227783221602239879972072419602639476858490617241105588560029118312992778838770436569905341248614940063541966138585151325296158670892628008524799090834749&download=true))
und welche Annahmen man bzgl. Modul-Ausrichtung und Anlagen-Wirkungsgrad trifft.
<!-- bzw. bei der
rechnerischen Zahl der [Volllaststunden](https://gammel.de/de/lexikon/volllaststunden/6288) pro Jahr (nämlich [standardmäßig 1000 h/a](
https://www.photovoltaik4all.de/wie-kann-man-die-solarstrahlung-berechnen),
aber eher 1100 h/a) bezogen auf die Standardstrahlung von 1000 W/m².-->

[![Bild: PV-Potential in Europa](PVOUT_Europe.png){:.center}](
https://solargis.com/maps-and-gis-data/download/europe)
Der Jahresertrag lässt sich leicht näherungsweise berechnen,
und zwar durch Multiplikation der Nennleistung der PV-Module in kWp
mit dem [*spezifischen PV-Jahresertrag*](
https://solar-direktinvest.de/photovoltaik/photovoltaik-investieren/spezifischer-jahresertrag-pv/) (engl. [_PV potential_, *PVOUT*](
https://globalsolaratlas.info/global-pv-potential-study)) in kWh/kWp.
Dieser ist standortspezifisch und beinhaltet Annahmen zu typischen praktisch
relevanten Faktoren wie den Verlust durch Verschmutzung und Wechselrichtung.\
Man erhält diese auch *spezifischer Ertrag* genannte Kenngröße aus den
groben [Karten von Solargis](https://solargis.com/maps-and-gis-data/download),
aus dem [Global Solar Atlas der Weltbank](
https://globalsolaratlas.info/map?c=50.10,11.05,7&s=48.1807,11.604e)
(auch von Solargis) oder am Genauesten aus der [PVGIS-Datenbank der EU](
https://re.jrc.ec.europa.eu/pvg_tools/de/)
bei der Standard-Eingabe von 1 kWp für die installierte max. PV-Leistung.

### Optimale Ausrichtung von Solarmodulen {#Ausrichtung}

Die Leistung von Solarmodulen hängt vor Allem von der Direktstrahlung ab ---
und zwar nicht nur von ihrer Intensität, sondern auch davon, wie sehr ihre
Fläche auf den aktuellen Sonnenstand ausgerichtet ist.
Dabei geht es um die zur Modulfläche senkrechte Komponente der Direktstrahlung,
also um den Faktor Kosinus der Winkelabweichung vom Lot auf die Modulfläche.

Mit der Diffusstrahlung, welche
wie oben erwähnt einen sehr großen Anteil an der Gesamtstrahlung ausmacht,
können Solarzellen leider nicht sehr viel anfangen.
Für diesen effektiv geringen Anteil wäre eine waagerechte Anordnung optimal.

![Bild: PV-Potential nach Ausrichtung von Solarmodulen](
Solarmodule_Ausrichtung_PV-Potential.png){:width="392" }
![Bild: Ertragsanteil nach Ausrichtung von Solarmodulen](
Solarmodule_Ausrichtung_Ertragsanteil.png){:width="385" .right}
Den [besten Jahres-Gesamtertrag](
https://machdeinenstrom.de/optimaler-ertrag-mit-mini-solar-kraftwerken/)
bekommt man in süddeutschen Breitengraden bei Orientierung nach Süden
und mit ca. 38° Neigung (also Winkel relativ zur Waagerechten).
Genaueres kann man z.B. über
[PVGIS](https://re.jrc.ec.europa.eu/pvg_tools/de/) (oder einfacher über
[Solarserver](https://www.solarserver.de/pv-anlage-online-berechnen/))
standortspezifisch anhand von Geo- und Klimadaten berechnen/simulieren,
wobei es auf ein paar Grad hin oder her nicht ankommt.

![Bild: Jahresertrag nach Ausrichtung von Solarmodulen](
Jahresertrag_nach_Ausrichtung.png){:.center}
Diese Grafik zeigt sehr schön die relative Änderung des Jahres-Gesamtertrages
einer PV-Anlage mit zunehmender Winkel-Abweichung von Süden (*Azimut*)
abhängig vom Neigungswinkel, wenn der optimale Neigungswinkel 35° beträgt.
Sie wurde von [bonotos](https://www.bonotos.com/) erzeugt,
basierend auf [Daten von Prof. Konrad Mertens](
https://www.fh-muenster.de/eti/downloads/personen/professoren/mertens/frei/2022_05_31_FH-MS_Nachhaltigkeitstag_Vortrag_Solarenergie_Kein_Dach_ohne_Solarstrom_PDF.pdf)
von der FH Münster.

Bei PV-Ertrags-Simulationen ist zu beachten, dass dabei üblicherweise
**der Jahres-Gesamtertrag** betrachtet und optimiert wird.
Dieser **unterliegt der Annahme, dass man den zur jeweiligen Tageszeit
(und Jahreszeit) erzeugten Strom auch immer gleichmäßig nutzen kann**,
sei es durch direkten Eigenverbrauch,
Zwischenspeicherung (was allerdings auch Verluste mit sich bringt)
oder vergütete Einspeisung (die aber leider selten attraktiv ist).\
Wenn man --- wie mit den meisten Stecker-Solaranlagen --- den erzeugten Strom
nur direkt im Haushalt verbrauchen kann und der Rest ins externe Netz geht,
sollte man das Nutzungsprofil berücksichtigen, welches auch auch
[*Lastprofil*](https://www.energie-lexikon.info/lastprofil.html) genannt wird.

![Bild: Ertrags-Nutzungsanteil nach Ausrichtung von Solarmodulen](
Solarmodule_Ausrichtung_Ertragsnutzungsanteil.png){:width="385" .right}
Durch genaue Simulation für durchschnittliche Haushalts-Tages-Nutzungsprofile
zeigt sich, dass **eine Abweichung von der optimalen Ausrichtung
deutlich weniger Einbußen beim selbst genutzten Jahres-Gesamtertrag bringt**.
So liegt bei senkrechter Anbringung im Verhältnis zur optimalen Neigung
die Einbuße nicht bei 30% vom Optimum, sondern je nach Lastprofil bei 23%.
Man hat also zur günstigen Ausrichtung seiner Solarmodule
meist größere Flexibilität als allgemein angenommen.

Eine Aufteilung in zwei Orientierungen, z.B. die klassische Ost-West-Ausrichtung
oder irgendwo dazwischen nach Südosten und Südwesten,
um **zu versuchen, auf die Vormittags- und Nachmittagssonne zu optimieren,
lohnt sich nicht**, selbst
wenn man den Ertragsüberschuss über die Mittagszeit kaum nutzen kann.
Das liegt daran, dass die Stahlungsintensität aus südlichen Richtungen
in der Tages- und Jahressumme viel höher ist -- die Sonne scheint dort einfach
viel stärker und viel häufiger (besonders im Winter) als im Osten oder Westen.
Dieser Effekt wird selbst dann nicht durch eine geringere Nutzbarkeit tagsüber
ausgeglichen, wenn man im Haushalt an Arbeitstagen von 8 bis 18 Uhr
nur Grundlast von z.B. 100 W hat.\
Eine Ost-West-Ausrichtung (etwa aus baulichen Gründen) schadet der Eigennutzung
allerdings auch nicht sehr, besonders wenn man tagsüber
im Vergleich zu den Morgen- und Abendstunden wenig Verbrauch hat.

Eine Reihe [genauer Simulationen](#Minutenbasis) für einen Haushalt
in Süddeutschland mit 3000 kWh Jahresverbrauch mit einer Stecker-PV-Anlage
mit zwei 300 Wp PV-Modulen und Gesamtsystem-Wirkungsgrad 86%
liefert für den Eigenverbrauch (EV) folgende Ergebnisse:

|Azimut |(opt.) Neigungswinkel|Nettoertrag|EV normales Profil|EV tagsüber nur Grundlast|
|------:|----------------:|----------:|-------------:|-----------------:|
|+/-90° |      15°        |  549 kWh  |  456 kWh     |  356 kWh         |
|+/-90° |      20°        |  544 kWh  |  455 kWh     |  357 kWh         |
|+/-60° |      30°        |  590 kWh  |  481 kWh     |  369 kWh         |
|+/-30° |      30°        |  637 kWh  |  496 kWh     |  372 kWh         |
|   0°  |      30°        |  652 kWh  |  500 kWh     |  372 kWh         |

<!-- https://www.mydealz.de/comments/permalink/39540050

./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_34deg_90deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_33deg_-90deg_2005_2020.csv 300
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_25deg_90deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_25deg_-90deg_2005_2020.csv 300
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_20deg_90deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_20deg_-90deg_2005_2020.csv 300
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_15deg_90deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_15deg_-90deg_2005_2020.csv 300

/Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_35deg_60deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_35deg_-60deg_2005_2020.csv 300
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_30deg_60deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_30deg_-60deg_2005_2020.csv 300
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_25deg_60deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_25deg_-60deg_2005_2020.csv 300
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_15deg_60deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_15deg_-60deg_2005_2020.csv 300
       ./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_30deg_53deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_33deg_-54deg_2005_2020.csv 300 

./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_45deg_30deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_45deg_-30deg_2005_2020.csv 300
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_36deg_30deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_35deg_-30deg_2005_2020.csv 300
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_30deg_30deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_30deg_-30deg_2005_2020.csv 300
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_25deg_30deg_2005_2020.csv 300 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_25deg_-30deg_2005_2020.csv 300

./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_37deg_2deg_2005_2020.csv 600
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_31deg_0deg_2005_2020.csv 600
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_28deg_0deg_2005_2020.csv 600
./Solar.pl Lastprofil_17_teils_64.csv 3000 Timeseries_48.269_10.408_SA2_1kWp_crystSi_14_25deg_0deg_2005_2020.csv 600

Variante extrem (Ost-West) gespreizt

Neigungswinkel  =  34° Azimut =  90°
Neigungswinkel  =  33° Azimut = -90°
PV-Bruttoertrag = 610 kWh
PV-Nettoertrag  = 525 kWh bei System-Wirkungsgrad 86%
Last Haushalt  = 3000 kWh
Eigenverbrauch  = 449 kWh
Eigenverbrauch  = 357 kWh wenn Mo-Fr 8-18 Uhr nur 100 W Verbrauch (Grundlast)

Neigungswinkel  =  25° Azimut =   90°
Neigungswinkel  =  25° Azimut =  -90°
PV-Bruttoertrag = 625 kWh
PV-Nettoertrag  = 538 kWh bei System-Wirkungsgrad 86%
Last Haushalt  = 3000 kWh
Eigenverbrauch  = 453 kWh
Eigenverbrauch  = 358 kWh wenn Mo-Fr 8-18 Uhr nur 100 W Verbrauch (Grundlast)

Neigungswinkel  =  20° (opt.) Azimut =   90°
Neigungswinkel  =  20° (opt.) Azimut =  -90°
PV-Bruttoertrag =  633 kWh
PV-Nettoertrag  =  544 kWh bei System-Wirkungsgrad 86%
Last Haushalt  = 3000 kWh
Eigenverbrauch  =  455 kWh
Eigenverbrauch  =  357 kWh wenn Mo-Fr 8-18 Uhr nur 100 W Verbrauch (Grundlast)

Neigungswinkel  =  15° Azimut =   90°
Neigungswinkel  =  15° Azimut =  -90°
PV-Bruttoertrag = 639 kWh
PV-Nettoertrag  = 549 kWh bei System-Wirkungsgrad 86%
Last Haushalt  = 3000 kWh
Eigenverbrauch  =  456 kWh
Eigenverbrauch  =  356 kWh wenn Mo-Fr 8-18 Uhr nur 100 W Verbrauch (Grundlast)

Variante stark gespreizt:

Neigungswinkel  =  35° Azimut =   60°
Neigungswinkel  =  35° Azimut =  -60°
PV-Bruttoertrag =  686 kWh
PV-Nettoertrag  =  590 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  481 kWh
Eigenverbrauch  =  369 kWh wenn Mo-Fr 8-18 Uhr nur 100 W Verbrauch (Grundlast)

Neigungswinkel  =  30° (opt.) Azimut =   60°
Neigungswinkel  =  30° (opt.) Azimut =  -60°
PV-Bruttoertrag =  689 kWh
PV-Nettoertrag  =  592 kWh bei System-Wirkungsgrad 86%
Last Haushalt  = 3000 kWh
Eigenverbrauch  =  481 kWh
Eigenverbrauch  =  369 kWh wenn Mo-Fr 8-18 Uhr nur 100 W Verbrauch (Grundlast)

Neigungswinkel  =  25° Azimut =   60°
Neigungswinkel  =  25° Azimut =  -60°
PV-Bruttoertrag =  689 kWh
PV-Nettoertrag  =  592 kWh bei System-Wirkungsgrad 86%
Last Haushalt  = 3000 kWh
Eigenverbrauch  =  480 kWh
Eigenverbrauch  =  368 kWh wenn Mo-Fr 8-18 Uhr nur 100 W Verbrauch (Grundlast)

Neigungswinkel  =  15° Azimut =   60°
Neigungswinkel  =  15° Azimut =  -60°
PV-Bruttoertrag =  680 kWh
PV-Nettoertrag  =  585 kWh bei System-Wirkungsgrad 86%
Last Haushalt  = 3000 kWh
Eigenverbrauch  =  474 kWh
Eigenverbrauch  =  364 kWh wenn Mo-Fr 8-18 Uhr nur 100 W Verbrauch (Grundlast)

  Neigungswinkel  =  30° (opt.?) Azimut =  53°
  Neigungswinkel  =  33° (opt.?) Azimut = -54°
  PV-Bruttoertrag = 702 kWh
  PV-Nettoertrag  = 604 kWh bei System-Wirkungsgrad 86%
  Last Haushalt  = 3000 kWh
  Eigenverbrauch  = 485 kWh
  Eigenverbrauch  = 371 kWh wenn Mo-Fr 8-18 Uhr nur 100 W Verbrauch (Grundlast)

Variante schwach gespreizt:

Neigungswinkel  =  45° Azimut =   30°
Neigungswinkel  =  45° Azimut =  -30°
PV-Bruttoertrag =  734 kWh
PV-Nettoertrag  =  631 kWh bei System-Wirkungsgrad 86%
Last Haushalt  = 3000 kWh
Eigenverbrauch  =  492 kWh
Eigenverbrauch  =  369 kWh wenn Mo-Fr 8-18 Uhr nur 100 W Verbrauch (Grundlast)

Neigungswinkel  =  36° Azimut =  30°
Neigungswinkel  =  35° Azimut = -30°
PV-Bruttoertrag = 741 kWh
PV-Nettoertrag  = 637 kWh bei System-Wirkungsgrad 86%
Last Haushalt  = 3000 kWh
Eigenverbrauch  = 496 kWh
Eigenverbrauch  = 372 kWh wenn Mo-Fr 8-18 Uhr nur 100 W Verbrauch (Grundlast)

Neigungswinkel  =  30° (opt.) Azimut =   30°
Neigungswinkel  =  30° (opt.) Azimut =  -30°
PV-Bruttoertrag =  739 kWh
PV-Nettoertrag  =  636 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  496 kWh
Eigenverbrauch  =  372 kWh wenn Mo-Fr 8-18 Uhr nur 100 W Verbrauch (Grundlast)

Neigungswinkel  =  25° Azimut =   30°
Neigungswinkel  =  25° Azimut =  -30°
PV-Bruttoertrag =  733 kWh
PV-Nettoertrag  =  631 kWh bei System-Wirkungsgrad 86%
Last Haushalt   = 3000 kWh
Eigenverbrauch  =  494 kWh
Eigenverbrauch  = 372 kWh wenn Mo-Fr 8-18 Uhr nur 100 W Verbrauch (Grundlast)

Variante nicht gespreizt:

Neigungswinkel  =  37° (opt.?) Azimut = 2° (opt.?)
PV-Bruttoertrag = 762 kWh
PV-Nettoertrag  = 655 kWh bei System-Wirkungsgrad 86%
Last Haushalt  = 3000 kWh
Eigenverbrauch  = 500 kWh
Eigenverbrauch  = 369 kWh wenn Mo-Fr 8-18 Uhr nur 100 W Verbrauch (Grundlast)

Neigungswinkel  =  31° (opt.) Azimut = 0°
PV-Bruttoertrag =  758 kWh
PV-Nettoertrag  =  652 kWh bei System-Wirkungsgrad 86%
Last Haushalt  = 3000 kWh
Eigenverbrauch  = 500 kWh
Eigenverbrauch  = 372 kWh wenn Mo-Fr 8-18 Uhr nur 100 W Verbrauch (Grundlast)

Neigungswinkel  =  25° (opt.) Azimut = 0°
PV-Bruttoertrag =  755 kWh
PV-Nettoertrag  =  649 kWh bei System-Wirkungsgrad 86%
Last Haushalt  = 3000 kWh
Eigenverbrauch  = 500 kWh
Eigenverbrauch  = 372 kWh wenn Mo-Fr 8-18 Uhr nur 100 W Verbrauch (Grundlast)

Neigungswinkel  =  25° Azimut = 0°
PV-Bruttoertrag =  749 kWh
PV-Nettoertrag  =  645 kWh bei System-Wirkungsgrad 86%
Last Haushalt  = 3000 kWh
Eigenverbrauch  =  498 kWh
Eigenverbrauch  = 372 kWh wenn Mo-Fr 8-18 Uhr nur 100 W Verbrauch (Grundlast)
-->

Also selbst bei einem Verbrauchsprofil, das sehr stark auf die Morgen- und
Abendstunden gespreizt ist, bringt eine Aufteilung der Modul-Ausrichtung
keinen Vorteil für den Eigenverbrauch. Dagegen spricht zusätzlich 
die Tendenz zu stärkerer Verschattung durch den flacheren Sonnenstand.
Außerdem ist die geteilte Montage meist aufwendiger, und die beiden Richtungen
verlangen zur Optimierung eine getrennte [MPPT-Regelung](#Wechselrichter).

Bei reiner Südausrichtung (0° Azimut), ebenso bei einer Orientierung von +/- 30°
oder +/- 60° abweichend von Süden, ist für den Eigenverbrauch eine Neigung von
ungefähr 30° optimal, wobei +/- 10° Winkeldifferenz sehr wenig ausmacht.
Bei einer Orientierung von +/-90° abweichend von Süden (also rein Ost-West) 
ist eine Neigung von ungefähr 15° bis 20° am günstigen,
aber bei 25 bis 30° fast gleich gut (besser gesagt: gleich schlecht).

Wer aus irgendeinem Grund (etwa wegen der Befestigung)
eine möglichst flache Neigung wählt, sollte trotzdem mindestens 12° verwenden,
um eine Selbstreinigung der Moduloberflächen durch Niederschlag zu ermöglichen.

Wenn man Solarmodule (z.B. auf dem Dach eines Wohnmobils) in waagerechter Lage
anbringt, ist man von der Orientierung (Himmelsrichtung) unabhängig.
Allerdings kommt nach meiner Erfahrung mit billigen flexiblen
Modulen selbst mittags an sehr sonnigen Tagen kaum über die Hälfte der
angegebenen Spitzenleistung hinaus.

Nutzungsmöglichkeiten {#Nutzung}
---------------------

Solarmodule liefern in direkter Abhängigkeit von der Einstrahlungsstärke
sehr variablen Gleichstrom (je nach Nennleistung maximal z.B. 11 A)
mit einer Spannung je nach Modultyp von üblicherweise 22 bis 44 V.
Dieser "rohe" Strom ist direkt erst mal kaum verwendbar,
außer z.B. zum Aufheizen eines Warmwasserspeichers mit einem [DC-Heizstab](
https://www.net4energy.com/de-de/energie/pv-heizstab#unterschiedliche).

Zum Thema *Stromspeicher* in verschiedensten Formen
und Nutzungsmöglichkeiten im Zusammenhang mit Photovoltaik
[hier ein ausführlicher Artikel](https://www.net4energy.com/de-de/stromspeicher)
und [hier](
https://www.wegatech.de/ratgeber/photovoltaik/stromspeicher/speicher-kennzahlen/)
eine gute Erklärung der wichtigsten Begriffe in diesem Zusammenhang,
z.B. der *Entladetiefe* und der *Zyklenanzahl*.

### Direkte Netzeinspeisung (Stecker-Solaranlage, "Balkonkraftwerk") {#Balkonkraftwerk}

![Bild: Solaranlage am Balkon](Balkonsolaranlage.jpg){:.left width="400"}
![Bild: Aufbau Balkonkraftwerk](Balkonkraftwerk.jpg){:.right width="378"}

{:style="clear:both"}

Typischerweise speisen Solaranlagen den erzeugten Strom
nach Umwandlung durch einen netzgekoppelten Wechselrichter
([Solarwechselrichter](https://de.wikipedia.org/wiki/Solarwechselrichter),
engl. _grid-tie inverter_) direkt ins Hausnetz oder öffentliche Stromnetz ein,
wo er sofort in irgendeiner Form verbraucht wird (bzw. der Rest verlorengeht).

Wichtig zu beachten ist, dass diese Nutzungsart abseits eines bestehenden
Wechselstrom-Netzes und während eines Stromausfalls nicht funktioniert,
weil sich der verwendete Wechselrichter mit dem Stromnetz synchronisieren muss.

Wie schon der Name *Stecker-Solaranlage* ausdrückt, werden solche kleinen
Anlagen meist einfach über einen (Schuko-)Stecker mit dem Hausnetz verbunden,
z.B. an einer Außensteckdose auf dem Balkon oder der Terrasse. Das ist sehr
flexibel und ermöglicht, sehr einfach ein Energiemessgerät dazwischenzustecken,
wie es unten zur [Verbrauchsmessung](#Verbrauchsmessung) gezeigt ist.
Diese Lösung ist m.E. schon sicher genug,
weil der Wechselrichter die Stromzufuhr sofort unterbricht, wenn man den
Stecker aus der Dose zieht und seine blanken Kontakte berühren kann.
Anfang 2023 [sprach sich der VDE dafür aus](
https://www.vde.com/de/presse/pressemitteilungen/2023-01-11-mini-pv),
"den Schuko-Stecker für die Einspeisung
bis zu einer Systemgesamtleistungsgrenze von 800 W zu dulden".

![Bild: Wieland-Unterputz-Dose](Wieland-Unterputz-Dose.png){:.right width="450"}
Man kann aber auch, wie vom VDE bislang empfohlen, eine spezielle
*Energiesteckdose* verwenden. Diese wird auch [*Einspeisesteckdose*](
https://www.solarenergie-info.de/wieland-einspeisesteckdose/) genannt
und ist meist von der Firma Wieland. Sie gilt als besonders sicher,
ist aber auch recht teuer und muss von einem Elektriker installiert werden.
[Hier](https://priwatt.de/blog/wieland-vs-schuko-stecker-was-eignet-sich-am-besten-fur-mein-balkonkraftwerk/)
ein ausführlicher Vergleich.
Eine weitere Möglichkeit ist, den Wechselrichter direkt fest mit dem Hausnetz
zu verdrahten, was den Betrieb sogar noch sicherer macht.

Die auch [*Balkonkraftwerk*](https://www.steckdosensolar.de/) genannten Anlagen
haben meist eine recht geringe PV-Nennleistung von etwa 600 bis 800 Wp.
Das hat neben der geringen Größe und sehr überschaubaren Kosten auch damit zu
tun, dass sie selbst installiert werden dürfen und genehmigungsfrei (jedoch
anmeldepflichtig) sind, wenn sie [maximal 600 W in die Steckdose einspeisen](
https://solarblitz.blogspot.com/2019/08/zulassigkeit-von-balkonkraftwerken-plug.html).
Dies gilt bislang für Deutschland und die Schweiz; in Österreich gilt nach einer
allgemeineren EU-Regel für die vereinfachte Nutzung eine Obergrenze von 800 W.
Seit Anfang 2023 [empfiehlt selbst der VDE](
https://www.vde.com/de/presse/pressemitteilungen/2023-01-11-mini-pv), sich
künftig auch in Deutschland an der "Bagatellgrenze bis 800 W" zu orientieren.

#### Beschränkung auf 600 bzw. 800 W und ihre Gründe {#Kappung}

Hintergründe dieser Beschränkung sind nicht in erster Linie, wie meist
angenommen wird, Sicherheitsbedenken bzgl. der Stromleitungen im Haushalt.

Der wesentliche technische Grund sind mögliche nicht immer gut kalkulierbare
Rückwirkungen auf das allgemeine Stromnetz.
Bei massenhafter nicht angemeldeter Einspeisung und kräftigem Sonnenschein
kann der Strom im Verteilnetz durch ziehende Wolken sehr stark schwanken,
was seine Stabilität beeinträchtigen könnte.
Auch könnten z.B. Mittelspannungs-Stromleitungen, die schon am Limit sind,
sich durch ungewöhnlich hohen Stromfluss stärker ausdehnen als normal
und daher teils die Mindest-Durchfahrtshöhe unterschritten werden.
Wenn jedoch durch sog.
[*Nulleinspeisung*](https://www.energie-experten.org/erneuerbare-energien/photovoltaik/eigenverbrauch/nulleinspeisung)
sichergestellt ist, dass kein überflüssiger Strom ins externe Netz fließt,
können Steckdosen-Anlagen [auch z.B. mit 1800 W Leistung](
https://www.pv-magazine.de/2022/07/04/indielux-startet-crowdfunding-fuer-serienproduktion-seines-einspeisewaechters-fuer-stecker-solar-geraete/)
normgerecht betrieben werden.

Man kann durchaus annehmen,
dass die Beschränkung auch nichttechnisch motiviert ist, etwa
weil die Energieversorgungsunternehmen möglichst wenig Konkurrenz haben wollen.

Die Beschränkung leistet auch in gewisser Hinsicht einen Beitrag zum Schutz
der Stromleitungen im Haus in folgendem sehr selten auftretenden Fall:

[![Bild: Mögliche Überlastung einer Wohnungs-Stromleitung durch lokale
Solarstrom-Einspeisung](
Stromleitung_Ueberlastung_Solareinspeisung.jpg){:.right width="380"}](
https://www.sonnenenergie.de/index.php?id=30&tx_ttnews%5Btt_news%5D=254)
Wenn über die Wohnungs-Stromleitung, an der die Einspeisung
stattfindet, gleichzeitig sehr kräftig Strom verbraucht wird, kann es
unter sehr ungünstigen Umständen passieren, dass auf Teilen der Leitung mehr
Strom fließt als die Sicherung eigentlich erlauben würde, was dann zu
einer mehr oder weniger übermäßigen Erwärmung der Leitung führt.\
Wenn L der momentane Gesamt-Verbrauch auf der Leitung ist und P die momentane
Erzeugung auf derselben Leitung, kommt bei der Sicherung die Leistung L - P an.
Wenn die Sicherung auf 16 A ausgelegt ist und die dort ankommende Leistung
vom Betrag her, also | L - P |, kleiner als 3680 W (= 230 V × 16 A) ist,
löst die Sicherung nicht aus. Falls dabei L oder P größer als 3680 W ist,
fließen auf einem Teilabschnitt der Leitung mehr als 16 A Strom.\
Das kann beispielsweise passieren, wenn gerade die Erzeugung 6 A Strom liefert
und der Stromverbrauch zwischen 16 A und 22 A liegt.\
Das ist allerdings insgesamt in der Praxis höchst unwahrscheinlich,
denn fast niemand betreibt an derselben Leitung gleichzeitig Geräte, die in
Summe einen Verbrauch L von über 3680 W haben, und dass z.B. durch einen
Kurzschluss extrem viel Strom fließt, ist möglich, aber kommt selten vor.
Und selbst wenn das der Fall ist und die Solaranlage in dieser Zeit auch nur
mal kurz weniger Leistung als L - 3680 W liefert,
löst die Sicherung wie üblich aus und die Überlast ist beendet.\
Von der ESTI (Schweiz) wird aus diesem Grund
die Leitungsüberlastung durch Stecker-Solaranlagen
[nicht normativ betrachtet](https://www.pvplug.de/positionspapier/).


#### Kappungsverlust durch Drosselung auf 600 W {#Kappungsverlust}

Die nominelle Leistung der verwendeten Solarmodule kann und sollte durchaus
größer sein aus 600 Wp (also eher 800 bis 1000 Wp), denn
in der Praxis werden sonst 600 W PV-Ausgangsleistung ohnehin nicht oft erreicht,
gerade in sonnenarmen Zeiten.
Man hat durch einen gewisse Überdimensionierung der PV-Module
(auch "Überbelegung" des Wechselrichters genannt)
auch zu ungünstigen Tages- und Jahreszeiten entsprechend mehr Ausbeute
(eigentlich sogar überproportional mehr,weil die Schwellspannung schneller
erreicht wird), allerdings auf eher niedrigem absoluten Niveau.

Die typischerweise auf 600 W gedrosselten Wechselrichter realisieren
die Leistungsbegrenzung aus energetischen Gründen schon auf ihrer Eingangsseite.
Leider verwenden einige Modelle (zumindest die von Deye/Bosswerk/revolt),
wie man in [Diagrammen](
https://www.photovoltaikforum.com/thread/180129-deye-sun600-und-sun2000-erfahrungen/)
sehen kann, dabei direkt den Ziel-Grenzwert, statt zu berücksichtigen,
dass aufgrund des Wirkungsgrades auf der Ausgangsseite ca. 10% weniger ankommen.
Zudem wird der Grenzwert oft auch noch einfach gleichmäßig auf die Eingänge
aufgeteilt. So können bei 90% Wirkungsgrad höchstens 540 W geliefert werden.
Obwohl der Netto-Ertrag durch diese ungeschickte Form der Abregelung also oft
sogar unnötig stark verringert wird, ist der Effekt auf den nutzbaren Ertrag
längst nicht so groß wie man meinen könnte.

Nehmen wir beispielsweise eine PV-Anlage mit 1000 Wp, die je nach Standort
und Ausrichtung zu einem Ertrag von etwa 1215 kWh brutto pro Jahr führen kann,
also bei einem PV-System-Wirkungsgrad von 92%
und einem Wechselrichter-Wirkungsgrad von 94% etwa 1050 kWh Netto-Ertrag.
Dann **macht der effektive Verlust durch Drosselung auf 600 W** Eingangsleistung
des Wechselrichters (also 564 W Ausgangsleistung bei den 94% Wirkungsgrad)
**nur ungefähr 10 kWh aus**. Dies erklärt sich durch zwei Effekte:
* Die Abregelung findet zwar während etwa 650 Sonnenstunden im Jahr statt, aber
die Differenz auf den sonst möglichen Netto-Ertrag ist moderat: etwa 80 kWh.
Diese Zahl ist schon relativ klein, und sie wird durch folgenden Effekt nochmal
deutlich kleiner:
* Nur während in Summe etwa 90 Stunden wird zeitgleich zu dieser Abregelung
typischerweise überhaupt so viel Strom verbraucht, dass sich die Drosselung beim
Eigenverbrauch bemerkbar macht, und die Menge dieses Verbrauchs, bei dem also
mehr als 528 W Leistung beansprucht werden, ist typischerweise ziemlich gering.

[//]: #
<!--
./Solar.pl Lastprofil_4673_kWh.csv 3000 Solardaten_1215_kWh.csv 1000 -tmy -peff 92 -ieff 94 -curb 564
88%: -peff 93.617

PV-Nominalleistung          = 1000 Wp
Bruttoleistung max.         =  994 W am TMY-04-30 um 11:00 h
PV-Bruttoertrag             = 1216 kWh
PV-Nettoertrag              =  973 kWh bei PV-System-Wirkungsgrad 92%, Wechselrichter-Wirkungsgrad 94%
PV-Ertragsverlust           =   78 kWh während 653 h durch Drosselung auf 564 W
Ertragsanteil 9-15 Uhr MEZ  =   70 %

Last durch Haushalt         = 3000 kWh
Eigenverbrauch mit Drossel  =  577 kWh
Eigenverbrauchsverlust      =    6 kWh während 93 h durch Drosselung auf 564 W
Netzeinspeisung             =  396 kWh
Eigenverbrauchsanteil       =   59 % des Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =   19 % des Verbrauchs (Autarkiegrad)
-->

Hingegen bieten 1000 statt 600 Wp PV-Nennleistung bei mäßigen Zusatzkosten eine
sinnvolle Reserve für schwächere Sonnenstunden, wodurch der Netto-Ertrag (trotz
Kappung) ca. 340 kWh höher liegt, der Eigenverbrauch ca. 135 kWh höher im Jahr.
Die Amortisationszeit der Gesamt-Anlage bleibt dabei ziemlich gleich, und auf
lange Sicht ergibt sich eine entsprechend höhere Kostenersparnis als mit 600 Wp.

<!--
./Solar.pl Lastprofil_4673_kWh.csv 3000 Solardaten_1215_kWh.csv 600 -curb 564 -tmy -peff 92 -ieff 94

PV-Nominalleistung          =  600 Wp
Bruttoleistung max.         =  597 W am TMY-04-30 um 11:00 h
PV-Bruttoertrag             =  729 kWh
PV-Nettoertrag              =  631 kWh bei PV-System-Wirkungsgrad 92%, Wechselrichter-Wirkungsgrad 94%
PV-Ertragsverlust           =    0 kWh während 0 h durch Drosselung auf 564 W
Ertragsanteil 9-15 Uhr MEZ  =   72 %

Last durch Haushalt         = 3000 kWh
Eigenverbrauch mit Drossel  =  444 kWh
Eigenverbrauchsverlust      =    0 kWh während 0 h durch Drosselung auf 564 W
Netzeinspeisung             =  187 kWh
Eigenverbrauchsanteil       =   70 % des Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =   15 % des Verbrauchs (Autarkiegrad)
-->

#### Stromzähler und Rücklaufsperre {#Stromzähler}

Für den selbst erzeugten und gleichzeitig verbrauchten Strom spart man sich
die Verbrauchskosten, weil der *Stromzähler* nur die Differenz berücksichtigt
und entsprechend langsamer läuft.
Es wird also nur der vom Stromanbieter bezogene Anteil des Verbrauchs berechnet.

Übrigens ist es normalerweise egal, auf welcher Drehstrom-Phase (L1, L2 oder L3)
die Stecker-Solaranlage angeschlossen wird und auf welcher Phase
die gleichzeitig verwendeten Verbraucher angeschlossen sind ---
die Stromzähler arbeiten *phasensaldierend*, d.h. sie bilden die Gesamtsumme
von Verbrauch und Erzeugung, welche dabei negatives Vorzeichen hat.

![Bild: Ferrariszähler](Ferrariszaehler.jpg){:.left width="400"}
![Bild: Symbol für Rücklaufsperre im Stromzähler](
Ruecklaufsperre.png){:.right width="370"}
Von gewonnenen Strom fließt der Anteil, der nicht aktuell im Haushalt
verbraucht (oder gespeichert) wird, automatisch ins allgemeine Stromnetz.
Moderne Stromzähler haben eine *Rücklaufsperre*, was man an dem entsprechenden
Symbol auf dem Gehäuse erkennen kann. Das führt dazu, dass der überflüssige
Strom praktisch ins externe Netz verschenkt wird.
Die klassischen *Ferrariszähler* mit mechanischer Drehscheibe
laufen dagegen rückwärts, wenn mehr Strom erzeugt als verbraucht wird.
Damit kann man "unter der Hand Strom verkaufen", was aber in Deutschland bislang
nicht erlaubt ist. Anfang 2023 [sprach sich der VDE jedoch dafür aus](
https://www.vde.com/de/presse/pressemitteilungen/2023-01-11-mini-pv), dass
bei PV-Anlagen bis 800 W die Zähler künftig "auch rückwärtslaufen dürfen".

Ein *Zweirichtungszähler* kann die Menge des eingespeisten Stroms unabhängig
vom Verbrauch messen, was die Möglichkeit der Vergütung eröffnet.
Eine offiziell angemeldete und vergütete Einspeisung ist mit einiger Bürokratie
verbunden und bringt wenig --- die Vergütung sank in Deutschland gemäß eEG
[bis 2022 auf ca. 6 ct/kWh](
https://www.zolar.de/blog/entwicklung-der-eeg-einspeiseverguetung)
und steigt [ab 2023 auf etwa 8 ct/kWh](
https://www.aroundhome.de/solaranlage/einspeiseverguetung/),
--- immer noch sehr mager, besonders im Vergleich zum Verbrauchspreis.

### Stromverbrauch im Haushalt {#Stromverbrauch}

Eigentlich ist es im Vergleich zum Betrieb einer (möglicherweise
recht groß dimensionierten) Solaranlage immer noch günstiger und
umweltfreundlicher, von vornherein den Stromverbrauch zu senken.
Stromfressende Geräte sollte man möglichst meiden und Geräte, die einen hohen
Verbrauch im Bereitschaftsmodus haben, bei längerem Nichtgebrauch ausschalten.
Man kann damit in einem 3-Personen-Haushalt auf unter 1500 kWh im Jahr kommen.

Je stromhungriger ein Haushalt tagsüber ist, desto größer der zu erwartende
Einsparungseffekt durch eine Steckdosen-Anlage ohne Stromspeicher.
Denn diese Nutzungsart lohnt sich also nur insoweit, wie man während der
Sonnenscheindauer den erzeugten Strom direkt sinnvoll verbrauchen kann.
Am einfachsten und am besten planbar geschieht das über die sog. *Grundlast*,
also ständig und mehr oder weniger gleichmäßig laufende Verbraucher
wie Kühlschränke, Internetanschluss, Computerserver
und Geräte, die im Bereitschaftsmodus (engl. _standby_) sind.
Darüber hinaus kann man gezielt diverse Haushaltsgeräte und Ladegeräte
vorzugsweise dann betreiben, wenn hohe Sonneneinstrahlung vorhanden ist.
Dazu bieten sich insbesondere Waschmaschinen und das Laden von Batterien an,
wobei die Akkus von E-Bikes oder E-Rollern von der Größenordnung
und ihrem zeitlichen Nutzungsprofil besonders geeignet sind.

Eine ziemlich clevere Nutzung von überschüssigem Strom finde ich die verstärkte
Nutzung einer Wärmepumpe oder das zusätzliche Aufheizen des Warmwasserbehälters
über einen [Heizstab](https://www.net4energy.com/de-de/energie/pv-heizstab),
so dass man weniger fossile Brennstoffe verbraucht.

#### Verbrauchsmessung {#Verbrauchsmessung}

![Bild: Energiekosten-Messgerät in Steckdosenform](
Energiekosten-Messgeraet.png){:.right width="300"
style="margin-left: 70px; margin-right: 70px"}
Den Stromverbrauch von Elektrogeräten im Haushalt kann man recht einfach
mit Energiekosten-Messgeräten in Steckdosenform bestimmen. Diese messen
nicht nur den momentanen Stromverbrauch in Watt, sondern bei längerer
Verwendung auch die über die Zeit verbrauchte Strommenge in kWh.

Die Grundlast eines Haushalts kann man über den Haushalts-Stromzähler
noch einfacher bestimmen, indem man die Differenz der Zählerstände
über einen Zeitraum von mehreren Stunden, zu dem sonst keine Verbraucher
eingeschaltet sind (z.B. nachts), durch die Zahl der Stunden teilt.

Eine schöne Übersicht von Geräten zur Messung auch der eingespeisten Strommenge
z.B. [hier](https://greenergains.de/balkonkraftwerk-einspeisung-messen/).

### Eigenverbrauch und Eigendeckung {#Eigenverbrauch}

Wer privat eine PV-Anlage betreibt, möchte möglichst viel von ihrem Ertrag
auch selbst verbrauchen, und zwar am besten direkt. Überschüssigen Strom in
einer Batterie für spätere Nutzung zwischenzuspeichern ist aufwendig und teuer.
Der nicht selbst genutzte Anteil wird meist ins externe Netz eingespeist.
Bei Balkonkraftwerken geschieht dies ohne Vergütung, aber auch wenn man seinen
Strom als Kleinunternehmer verscherbelt, hat man einige Bürokratie und bekommt
ziemlich wenig heraus.

Also geht es ökonomisch darum, den Eigenverbrauchsanteil zu maximieren. Der
*Eigenverbrauchsanteil* (*Nutzungsgrad*) ist der Anteil der Netto-Stromerzeugung,
der direkt verbraucht (oder ggf. mit Batterie-Ladeverlusten gespeichert wird).
Je höher er ist, desto weniger Energie wird ins externe Stromnetz eingespeist.
Je kleiner die Anlage ist, umso leichter kann man eine hohe Eigenverbrauchsquote
erreichen, allerdings dann bei entsprechend kleinerem Stromvolumen.

Damit verwandt ist der *Eigendeckungsanteil* (*Selbstversorgungsgrad*), also der
Anteil des Eigenverbrauchs (ggf. mit Batterieentladung abzüglich Ladeverlusten)
am Gesamtverbrauch.
Je höher er ist, desto weniger Energie muss von extern bezogen werden.
Er wird oft auch als
[*Autarkiegrad*](https://klarsolar.de/unterschied-eigenverbrauch-autarkie/)
bezeichnet, was etwas irreführend ist, denn typischerweise arbeitet
der Wechselrichter der PV-Anlage auch dann nicht ohne Verbindung zum Netzstrom,
wenn gerade kein *Netzbezug* (also Stromfluss von außen) stattfindet.
Je größer die Anlage ist, umso höher fällt der Autarkiegrad aus,
allerdings oft zu Lasten des Eigendeckungsanteils.
Eine Quasi-Autarkie (Eigendeckungsanteil 100%)
kann man aber nur mit enormer Stromspeicher-Kapazität erreichen.

[![Bild: Eigenverbrauch einer 7kWp-Anlage mit 5kWh-Speicher über den Tag](
Eigenverbrauch-7kWp-5kWh-Speicher.png){:.center}](
https://klarsolar.de/wp-content/uploads/2022/10/Eigenverbrauchsanteil-bei-einer-7kWp-Anlage-mit-5kW-Speicher.pnghttps://klarsolar.de/unterschied-eigenverbrauch-autarkie/)
Das Bild veranschaulicht den typischen Stromverlauf bei einer Hausdach-PV-Anlage
mit 7kWp Nennleistung und 5kWh Stromspeicher an einem ziemlich sonnigen Tag mit
mittags etwas Wolken. Weitere schöne Erklärungen mit Grafiken gibt es
[hier](https://brodsoft.de/stromverlauf/pages/simulation).

Der Eigendeckungsanteil und Eigenverbrauchsanteil lässt sich sehr einfach
näherungsweise mit dem ["Stecker-Solar-Simulator"](
https://solar.htw-berlin.de/rechner/stecker-solar-simulator/)
für Balkonkraftwerke bzw. dem ["Unabhängigkeitsrechner"](
https://solar.htw-berlin.de/rechner/unabhaengigkeitsrechner/)
für Hausdach-PV-Anlagen der HTW Berlin berechnen.
[![Bild: Stecker-Solar-Simulator](Stecker-Solar-Simulator.png)](
https://solar.htw-berlin.de/rechner/stecker-solar-simulator/)
Beide Simulationen erfolgen mit Daten der Wetterstation Lindenberg bei Berlin
aus dem Jahr 2017 (für Süddeutschland kann man 10-15% mehr PV-Leistung ansetzen)
für einen gegebenen Jahresstromverbrauch (mit einer typischen Lastverteilung),
gegebene PV-Nennleistung (mit einem hohen spezifischen PV-Jahresertrag)
und optional gegebene nutzbare Speicherkapazität (mit typischem Wirkungsgrad
für LFP-Batterien und typischen Wandlungsverlusten).
[![Bild: Unabhängigkeitsrechner](Unabhängigkeitsrechner.png)](
https://solar.htw-berlin.de/rechner/unabhaengigkeitsrechner/)
Der Unabhängigkeitsrechner liefert auch den Anteil der Batterieentladung an der
Stromversorgung, den man zur Ertrags- und [Wirtschaftlichkeitsberechnung von
PV-Speichern](https://www.youtube.com/watch?v=bE5fLy0w3MM&t=674s)
verwenden kann (und zwar durch Multiplikation mit dem Stromverbrauch).
<!--
Für Anlagen ohne Stromspeicher sind die Ergebnisse sehr realistisch.
Für Stromspeicher scheinen sie allerdings recht optimistisch.
-->

Eine sehr einfache Möglichkeit, online die Amortisation zu berechnen, bietet
auch das [PVTool von Andreas Schmitz ("AkkuDoktor")](https://www.akkudoktor.net/pvtool-rechner/).
Als Besonderheit kann man hier schön sehen, wie sich Eigenverbrauchsquote,
Autarkiegrad und Amortisation in Abhängigkeit von der Anwesenheit und Kapazität
eines Stromspeichers ändern.\
Allerdings sind die Ergebnisse deutlich zu optimistisch. Das liegt vermutlich
am verwendeten Lastprofil und unrealistisch hoch angenommenen Wirkungsgraden.
Er macht zu diesen wichtigen Punkten und sonstigen Grundlagen seiner Berechnung
auf seinen beiden PVTool-Seiten keinerlei Angaben.

### Ertragsberechnung und Amortisation {#Ertragsberechnung}

Wie eingangs geschrieben kann man bei optimaler Platzierung von Solarmodulen
pro Jahr etwa 1,1 kWh Strommenge pro Wp installierter Solarleistung gewinnen.
Rechnet man beispielsweise mit einer Investition von 1,10€/Wp
(inklusive anteiliger Kosten für Wechselrichter, Installation etc.),
ergeben sich Kosten von 1€/kWh erzeugtem Solarstrom pro Jahr.

* Falls der damit erzeugte Strom komplett selbst verbraucht wird,
was aber praktisch kaum der Fall ist,
und man einen dadurch eingesparten Arbeitspreis von 40 ct/kWh ansetzt,
ergibt sich eine Amortisation der Anschaffungskosten in nur 2,5 Jahren.
* Eine typische Balkonanlage mit 600 Wp Nennleistung erreicht einen
Jahres-Bruttoertrag von etwa 765 kWh, was bei 86% Gesamtsystem-Wirkungsgrad
ca. 660 kWh Netto-Einspeisung des Wechselrichters an der Steckdose bedeutet.
Bei einem durchschnittlichen Haushalts-Tages-Nutzungsprofil und einem typischen
Jahresverbrauch von 3000 kWh liegt der selbst genutzte Ertrag bei etwa 460 kWh.
Der Eigendeckungsanteil liegt damit bei 15% des Verbrauchs,
der Eigenverbrauchsanteil bei 70% des Ertrags.

[//]: #
<!-- ./Solar.pl Lastprofil_4673_kWh.csv 3000 Timeseries_48.215_11.727_SA2_1kWp_crystSi_0_38deg_0deg_2005_2020.csv 600 -peff 92
ergibt 457 kWh, aber noch etwas Lastspitzen-Abzug
88%: -peff 93.617

PV-Nominalleistung          =  600 Wp
Bruttoleistung max.         =  656 W am 2020-03-23 um 11:00 h
PV-Bruttoertrag             =  765 kWh
PV-Nettoertrag              =  662 kWh bei PV-System-Wirkungsgrad 92%, Wechselrichter-Wirkungsgrad 94%
Ertragsanteil 9-15 Uhr MEZ  =   73 %

Last durch Haushalt         = 3000 kWh
Eigenverbrauch              =  460 kWh
Netzeinspeisung             =  201 kWh
Eigenverbrauchsanteil       =   70 % des Nettoertrags (Nutzungsgrad)
Eigendeckungsanteil         =   15 % des Verbrauchs (Autarkiegrad)

Bei Lastprofil_4685_kWh.csv Eigenverbrauch 502 kWh -->
Damit kann man bei 40 Ct/kWh jährlich ungefähr 180€ Stromkosten einsparen.
Bei einer Investition von 660€ ergibt sich (ohne Berücksichtigung
von Kapitalkosten u.ä.) eine Amortisationszeit von 3,7 Jahren.\
Bei 1500 kWh Jahresverbrauch können immerhin etwa 320 kWh selbst genutzt werden,
was eine Amortisation in gut 5 Jahren ergibt.

Für die Amortisation des energetischen Aufwands
zur Herstellung einer Mini-PV-Anlage muss man nach [Angaben des DKE](
https://www.dke.de/de/arbeitsfelder/energy/mini-pv-anlage-solar-strom-balkon-nachhaltig-erzeugen)
allerdings noch 2-3 Jahre länger rechnen.
In die Gesamt-Ökobilanz einer PV-Anlage und ihrer Nutzung gehen natürlich
noch weitere Effekte ein, die sich aber kaum quantifizieren lassen.

#### Monatsbasierte Berechnung von Ertrag und Amortisation {#PV-Rechner}

[![Bild: Ertragsrechnung Balkonanlage](
PV-Rechner_v6+_Balkonanlage_600Wp.png){:.center}](PV-Rechner_v6+.xls)
Beispielsweise mit
dem [PV-Rechner](PV-Rechner_v6+.xls) (der eigentlich für "große"
PV-Anlagen auf Hausdächern konzipiert ist) kann man die Rechnung
deutlich genauer machen. Er berücksichtigt u.A. die Ausrichtung der
Solarmodule, die jährliche Abschreibung, Reparatur- und Kapitalkosten,
den Anteil des während der Sonnenscheindauer im Haushalt nutzbaren
Ertrages, sowie optional Effekte durch das Laden eines E-Fahrzeugs (was
normalerweise öfter zu Sonnenscheinzeiten erfolgen kann), den Betrieb
einer Wärmepumpe und die Nutzung eines Stromspeichers. Dabei werden die
Energieflüsse der Einfachheit halber nur auf Monatsbasis gerechnet, so dass
selbst tageszeitliche Effekte nur näherungsweise berücksichtigt werden können.

Bei der o.g. typischen Balkonanlage für 660€ mit 600 Wp und 660 kWh Jahresertrag
ergibt sich mit dem PV-Rechner für einen Haushalt mit 3000 kWh Jahresverbrauch,
der zu 28% während der Haupt-Sonnenscheinzeiten erfolgt,
ein etwas zu optimistischer Solarstrom-Eigenverbrauch von etwa 530 kWh pro Jahr.
Damit könnte man bei 40 Ct/kWh jährlich ca. 205€ Stromkosten einsparen, was eine
Amortisationszeit von 3,2 Jahren und eine satte (Anfangs-)Rendite von 26% ergäbe.

Hinweis: Der PV-Rechner stammt von [Falko (bonotos)](https://www.bonotos.com/)
Der originale beinhaltet auch seiner letzten Version 22-06 einen groben Fehler
in der Rendite-Formel, der zu (fast) doppelt überhöhten Rendite-Zahlen führt.
Ich habe mich mit Falko zu diesen und anderen Punkten ausgetauscht.
Er möchte an dem Tool nichts mehr machen.
So stelle ich hier eine verbesserte und etwas erweiterte Version zur Verfügung.

#### Speichersimulation {#Speichersimulation}

[![Bild: Speichersimulation InGe16 1.-6. April, 1000kWh, PV 660 kWh, 2,4 kWh
Speicher](Speichersimulation_InGe16_April_1-6.png){:.center}](
https://brodsoft.de/stromverlauf/profiles/simulation)
Eine genauere Simulation des Eigenverbrauchs für einen gegebenen PV-Nettoertrag,
ohne oder mit Stromspeicher (mit Angabe von genutzter Kapazität und Wirkungsgrad),
gibt es von [brodsoft](https://brodsoft.de/stromverlauf/profiles/simulation).
Diese basiert auf realen Profildaten für PV-Erzeugung und Stromverbrauch,
mit denen die Berechnung immerhin auf Stundenbasis erfolgt.
Man kann sich in der Ausgabe auch für jeden Monat Grafiken ausgeben lassen,
auf denen man sich sehr schön den Verlauf der elektrischen Größen ansehen kann.
Außerdem gibt es gute Info-Seite mit guten Erklärungen zu Eigenverbrauchsanteil
und Eigendeckungsanteil zu Strategien zu ihrer Optimierung.
Diese Simulation berechnet für die o.g. 600 Wp Beispiel-Anlage je nach Auswahl
des Profils einen Eigenverbrauch von teils 601 kWh (Profil "allgemein 13/14")
und mehr, aber typischerweise eher 514 kWh (Profil "InGe 16") pro Jahr.

#### Simulation auf Minutenbasis {#Minutenbasis}

Eine eigene Simulation auf Minutenbasis
basierend auf den PV-Profildaten für ein [*typisches meteorologisches Jahr*](
https://help.valentin-software.com/pvsol/de/berechnungsgrundlagen/einstrahlung/klimadaten/)
von [PVGIS](https://re.jrc.ec.europa.eu/pvg_tools/de/)
und auf 74 minütlichen Haushaltsverbrauchs-Profilen,
die von der Forschungsgruppe Solarspeichersysteme HTW Berlin [veröffentlicht](
https://solar.htw-berlin.de/elektrische-lastprofile-fuer-wohngebaeude/)
wurden, kommt auf realistischere Ergebnisse.
Mit einem [Lastprofil-Skript](Lastprofil.pl) können aus den genannten Rohdaten
Lastprofil-Dateien wie [diese](Lastprofil_4673_kWh.csv) synthetisiert werden.
So eine Datei wird dann zusammen mit von PVGIS heruntergeladenen Solardaten
wie [diesen](Solardaten_1215_kWh.csv) als Eingabe für ein
[Solarertrag-Skript](Solar.pl) verwendet. Weitere Parameter sind die
Nennleistung und der Wirkungsgrad der Anlage sowie der Jahresverbrauch
und optional eine Limitierung des PV-Ertrags durch den Wechselrichter.
Auch die Kombination von PV-Modulgruppen verschiedener Leistung und Ausrichtung
wird unterstützt.

Für die o.g. Beispiel-Anlage für den Raum München mit 600 Wp
und einem  PV-Nettoertrag (nach Wechselrichter-Verlusten) von etwa 730 kWh
ergibt sich mit dieser Simulation unter Verwendung minutengenauer Lastprofile
je nach Profil eine Eigennutzung von ca. 450 bis 560 kWh.

Das Ergebnis fällt nicht ganz so günstig wie bei den anderen beiden Simulationen
aus, v.A. weil hier die in der Praxis relativ häufigen Lastspitzen immerhin im
Minutenbereich berücksichtigt werden, die von einer Mini-Solaranlage praktisch
kaum abgefangen werden können, so dass der Eigenverbrauchsanteil geringer ist
als bei einer über Stunden oder gar Monate gemittelten Betrachtung.

Vergleichsrechnungen auf Grundlage eines Lastprofils mit (annähernd)
sekündlicher Auflösung haben ergeben, dass die Lastspitzen nur teilweise einen
spürbaren Einfluss auf die Nutzbarkeit des PV-Ertrags von kleinen Anlagen haben.
Bei 600 Wp sind die Eigennutzungs-Ergebnisse bei Lastdaten auf Stundenbasis
etwa 3 bis 6% zu optimistisch, auf Minutenbasis nur bis etwa 1%.
<!-- bei 3000 kWh: 593 562 557  6%   bei 6000 kWh: 630 623 622  1% -->

### Hausnetzeinspeisung mit Batteriepuffer {#Batteriepuffer}

![Bild: Balkonkraftwerk mit Pufferbatterie und Inselwechselrichter](
Pufferbatterie_und_Inselwechselrichter.png){:.right width="400"
style="margin-left: 40px}
Statt den Solarstrom direkt einzuspeisen, kann man in auch in einer aufladbaren
Batterie zwischenspeichern und von dort nach Bedarf zeitlich versetzt über einen
[netzgekoppelten Wechselrichter](#Netzwechselrichter) ins Hausnetz einspeisen.
Diese Betriebsart kann man allgemein als *Strompufferung* bezeichnen.
Ihre einfachsten Ausprägungen sind die [*Konstanteinspeisung*](#Einspeisung),
wobei eine etwas optimierte Variante *Nachteinspeisung* genannt wird.

Die Strompufferung maximiert den Nutzen der PV-Anlage für den eigenen
Stromverbrauch, lohnt sich finanziell aber kaum, außer wenn man die Batterie
sehr günstig bekommt oder schon aus anderen Gründen hat, z.B. für eine
Notstromversorgung (mit Inselwechselrichter) oder als Fahrzeugbatterie.
Außerdem ist es für die ökologische Gesamtbilanz eigentlich besser, den
überschüssigen Strom an die Allgemeinheit (auch ohne Vergütung) abzugeben.

#### Regelungsstrategien für Stromspeicher {#Regelungsstrategien}

Für die Einsparung von Stromkosten wäre folgende Lade- und Entladeregelung
ideal:
* Solange der Speicher nicht voll ist, erfolgt die Ladung
immer genau so stark wie gerade an PV-Leistung übrig ist,
also aktuell nicht anderweitig verbraucht wird.
Damit kann man die sogenannte *Nulleinspeisung* realisieren,
also dass kein überschüssiger Strom ins externe Netz fließt.
* Solange der Speicher nicht leer ist, erfolgt die Entladung
immer genau so stark wie gerade an Last nicht von der PV-Leistung abdeckt wird.

[//]: #
Zur Schonung der Batterie solle dabei
* ein gewisser Ladestrom und ein gewisser Entladestrom nicht überschritten
werden, wobei die verwendeten Komponenten da ohnehin Grenzen setzen, und
* die Regelung zeitlich geglättet werden, so dass bei sich schnell ändernder
Erzeugung und Last nicht ständig zwischen Auf- und Entladung umgeschaltet wird,

[//]: #
wobei diese Zusatzbedingungen allerdings gewisse Verluste mit sich bringen.

Das alles ist reglungstechnisch ziemlich aufwendig und benötigt jedenfalls
einen Sensor zur Erfassung des momentanen Haushalts-Stromverbrauchs.
Es lohnt sich eher nur für größere PV-Anlagen.

Für Stecker-Solaranlagen ist es viel einfacher
und für die meisten Anwendungsfälle ausreichend,
die (gedrosselte) Ausgangsleistung des Wechselrichters und die Batteriekapazität
so abzustimmen, dass lediglich ein Großteil der Grundlast des Haushalts,
z.B. 50 bis 100 W, für eine Dauer von etwa 1-2 Tagen abgedeckt wird.
Wenn man diese *Konstanteinspeisung* noch mit einer Zeitschaltuhr (oder einem
Helligkeitssensor) zur Beschränkung zwischen Sonnenunter- und Aufgang
kombiniert, bekommt man eine *Nachteinspeisung*.\
Ziel der Konstanteinspeisung ist, die über die sonnenreiche Tageszeit
gesammelte Solarenergie auch über sonnenarme Zeiten  gleichmäßig abgegeben
(solange die Ladung reicht, zumindest bis zum nächsten Vormittag),
und dabei möglichst wenig Strom nach extern zu verschenken.

![Bild: Wasserspeicher als Analogie](Wasserspeicher.jpg){:.right width="400"
style="margin-left: 50px; margin-right: 50px"}
Hier als Analogie eine Skizze eines automatischen Wasserspeichers,
der z.B. über die Dachrinne eines Hauses gespeist wird. Wenn er voll genug ist,
läuft das Wasser über die rechte innere Trennwand und lässt die Kugel
aufschwimmen, die bis dahin den Auslass blockiert hat. Dann fließt das
Wasser aus dem Speicher langsam und gleichmäßig nach unten aus. Wenn der
Speicher fast leer ist, verschließt die Kugel den Auslass wieder. Der
Speicher füllt sich (auch schon zwischendurch) bei Wasserzufuhr wieder
auf. Zusätzlich ist der Speicher am Einlass mit einem Überlaufschutz
ausgestattet, der die Wasserzufuhr stoppt, wenn der Speicher sehr voll
ist und das Wasser durch den kleinen Auslass nicht schnell genug
abfließt.

Diese einfache Regelung hat allerdings verschiedene Schwächen,
vor Allem dass damit nur die Grundlast effizient abdeckbar ist.
Außerdem geht Sonnenenergie verloren, wenn die Batterie voll ist,
z.B. an sonnenreichen Tagen am Nachmittag, wenn die Solarleistung relativ groß
ist im Vergleich zur Batteriekapazität bzw. dem Verbrauch durch die Grundlast.
Mit einer Zusatzschaltung könnte man dafür sorgen, dass in dieser Zeit der
Solarstrom direkt über einen Netzwechselrichter (idealerweise über den bereits
vorhandenen) eingespeist wird.
Das Umschaltsignal für den Überlaufmodus sollte wohl am besten vom Laderegler
kommen (z.B. optisch über die Ladekontrollleuchte). Es kann aber auch von der
Batteriespannung abhängig gemacht werden, wobei es dann auch vorkommen wird,
dass Laderegler und Wechselrichter gleichzeitig aktiv sind. Ob das eher stört
oder sogar vorteilhaft wäre, dürfte von den verwendeten Geräten abhängig sein.

#### Speicherbatterie {#Speicherbatterie}

Zu berücksichtigen ist, dass die Zwischenspeicherung des Stroms je nach Art der
[Batterie](#Speicher) Verluste von etwa 5 bis 20% mit sich bringt -- bei LiFePO4
unter 10%. Auch kann man nicht die volle Nennkapazität entnehmen,
ohne dass die Akkuzellen stark leiden (d.h. schnell an Kapazität verlieren).
Bei LiFePO4 sind immerhin 90% Entladetiefe problemlos möglich.

Als Faustformel für die Dimensionierung [empfiehlt die Verbraucherzentrale NRW](
https://www.verbraucherzentrale.nrw/wissen/energie/lohnen-sich-batteriespeicher-fuer-photovoltaikanlagen-24589)
etwa 1 kWh pro 1000 kWh Jahresstromverbrauch, also gut 1/3 des Tagesverbrauchs.
Wer mit der Speicherbatterie zusätzlich eine Notstromversorgung über eine
[Inselanlage](#Inselanlage) realisieren möchte, wird die Kapazität je nach
Anwendungsszenario eher größer wählen.

Die Forschungsgruppe Solarspeichersysteme der HTW Berlin
gibt [genauere Empfehlungen und Begründungen](
https://solar.htw-berlin.de/publikationen/auslegung-von-solarstromspeichern/).
Kurz zusammengefasst:
Ein Batteriespeicher ist nur sinnvoll, wenn die PV-Leistung mind. 0,5 kWp
je 1000 kWh Jahresstromverbrauch beträgt. Als Kapazität empfiehlt sie
maximal 1,5 kWh je 1000 kWh Jahresverbrauch und
maximal 1,5 kWh je kWp PV-Nominalleistung.

#### Ladung der Batterie {#Batterieladung}

Das Laden der Batterie erfolgt am besten möglichst direkt aus der PV-Anlage
über einen [Solar-Laderegler](#Laderegler). Dies nennt man [*DC-Kopplung*](
https://www.photovoltaikforum.com/core/article/7-pv-und-batteriespeicher-besser-ac-oder-dc-gekoppelt/),
weil der Gleichstrom der PV-Module nicht umständlich und verlustreich
zwischendurch in Wechselstrom hin- und her-gewandelt wird.
Ein weiterer Vorteil ist (mit einem Inselwechselrichter) die Notstromfähigkeit.
Hingegen ist der einzige Vorteil der *AC-Kopplung* übers Haus-Wechselstromnetz
und ein 230 V-Ladegerät eine große Flexibilität bei der Wahl der Komponenten,
auch bzgl. eines späteren Ausbaus und der Betriebsspannung der Komponenten.

#### Einspeisung aus der Batterie {#Einspeisung}

Wenn man schon einen Solar-Wechselrichter hat und diesen für eine ganz einfache
Netzeinspeisung verwenden möchte, könnte es schon genügen, ihn (über eine
Sicherung und soweit nötig eine automatische Unterspannungsabschaltung)
mit der Batterie zu verbinden und nach Bedarf über einen Schalter zu steuern ---
allerdings nur, wenn die Batteriespannung gut im Eingangsspannungsbereich des
Wechselrichters liegt und dieser mit seiner vollen oder limitierten Leistung
betrieben werden kann. Dazu kann man beispielsweise einen auf 300 W begrenzten
PV-Eingang nutzen oder die Drosselung in die Firmware programmieren (lassen),
wie es z.B. der Kundendienst von Deye (Mail an service@deye.com.cn) anbietet.\
Wenn der Wechselrichter mehrere Eingänge hat, kann man an die übrigen Eingänge
auch noch direkt PV-Module anschließen,
deren Ertrag dann nicht über die Batterie gepuffert wird.

Wer zudem bereits eine Powerstation hat,
kann zwischen ihren Wechselstrom-Ausgang und den Netzwechselrichter ein
regelbares Netzteil hängen, wie [von Andreas Schmitz vorgeschlagen](
https://www.youtube.com/watch?v=ZXHAXrJS9CU),
was allerdings zu Zusatz-Verlusten durch Hin- und Her-Wandlung des Stroms führt.

![Bild: Netzwechselrichter aus Batterie gespeist](
Netzwechselrichter-aus-Batterie-gespeist.jpg){:width="600" .right}
Besser ist allerdings, die Einspeisung regelbar zu gestalten.
Dazu bietet sich ein Netzwechselrichter wie von
[Soyosource](https://de.aliexpress.com/item/1005001445871590.html) bzw.
[PMSUN](https://www.amazon.de/PMSUN-netzgekoppelter-Wechselrichter-einstellbare-Batterieentladung/dp/B0B4RZNHF3)
an, der für die Verwendung an einer Batterie als Quelle ausgelegt ist
und dessen Ausgangsleistung innerhalb gewisser Grenzen manuell regelbar ist.

Um die Stromstärke regelbar zu drosseln, kann man dem Solar-Wechselrichter
auch ein einen günstigen [Gleichspannungswandler](#Gleichspannungswandler)
mit regelbarer Strombegrenzung (engl. _limiter_) vorschalten.

{:style="clear:both"}

[![Bild: Balkonsolar mit Akku - AkkuDoktor](
Balkonsolar_AkkuDoktor.png){:.center}](
https://www.youtube.com/watch?v=yOcoux9IbzM)
Noch eleganter und flexibler, aber deutlich aufwendiger ist die Verwendung eines
elektronisch steuerbaren DC-DC-Wandlers, z.B. des [Joy-IT DPM8624](
https://www.idealo.de/preisvergleich/OffersOfProduct/202115817),
wie in einem [Video von Andreas Schmitz](
https://www.youtube.com/watch?v=yOcoux9IbzM) vorgeführt.
Dann lässt sich die Einspeisung sogar abhängig vom realen Stromverbrauch regeln
(allerdings mit einer gewissen Verzögerung), und etwa über einen entsprechend
programmiert Raspberry Pi, der die Verbrauchsdaten über den sog.
[„Volkszähler“](https://hessburg.de/tasmota-wifi-smartmeter-konfigurieren/)
oder [„Powerfox“](https://hessburg.de/tasmota-wifi-smartmeter-konfigurieren/)
aus dem Haushalts-Stromzähler übermittelt bekommt -- sofern ein smarter
Stromzähler verbaut ist und man Zugang zu diesem hat.

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
hat, wie z.B. beim Victron BlueSolar, kann man diesen so verwenden, wie in
[diesem schönen Video von PV&E](https://www.youtube.com/watch?v=N6NqMXQHP2I)
gezeigt. Zudem kann dessen Straßenlichtfunktion für die zeitliche Steuerung
genutzt werden.

{:style="clear:both"}

[![Bild: Balkonkraftwerk mit Speicher - Solaranlage](
Balkonkraftwerk_mit_Speicher.jpg){:.right width="350"}](
https://www.youtube.com/watch?v=f-iz6WE8GD8)
Um die Einspeisung automatisch in Abhängigkeit vom Ladezustand der Batterie
ein- und auszuschalten, kann man auch einen recht simplen
[programmierbaren Batteriespannungswächter](#Spannungswächter) verwenden, wie im
[Video von Dimitri](https://www.youtube.com/watch?v=f-iz6WE8GD8) vorgeführt.

Der Spannungswächter wird so eingestellt,
dass er beim Erreichen einer Batteriespannung, die
z.B. annähernd einer Vollladung entspricht, den Wechselrichter einschaltet und
z.B. in der Nähe der Batterie-Entladeschlussspannung diesen wieder ausschaltet.

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
[Solar-Laderegler](#Laderegler) benötigt, und sofern die Verbraucher
nicht direkt mit der Batteriespannung (z.B. 12 V oder 24 V Gleichstrom)
betrieben werden können, zusätzlich ein ausreichend leistungsstarker
[Inselwechselrichter](#Inselwechselrichter) zur Umwandlung
in den üblichen "Steckdosenstrom" (also Wechselstrom mit 230 V).\
An diesen Wechselrichter muss man bei Stromausfall alle
dann zu verwendenden Geräte (meist über eine Mehrfachsteckdose) anschließen.
Man speist dann also nicht einfach ins stromlose Hausnetz ein,
weil dazu die von außen kommende Stromleitung umgeschaltet werden und für eine
geeignete Erdung gesorgt werden müsste, was nur ein Elektriker machen kann/darf.

Ähnlich wie die o.g. [Batteriepufferung](#Batteriepuffer) ist diese Nutzungsart
flexibler aber wegen der nötigen zusätzlichen Komponenten (v.A. der Batterie)
auch deutlich teurer und auch etwas anfälliger und wartungsintensiver
als die [direkte Netzeinspeisung](#Balkonkraftwerk).
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


Auswahl und Nutzung von Komponenten {#Komponenten}
--------------------------------------------------

### Solarmodule {#Solarmodule}

Solarmodule (engl. _solar panels_) werden intern aus vielen in Reihe
geschalteten Solarzellen zusammengesetzt, die Sonnenlicht in Gleichstrom
umwandeln.

![Bild: Spannung und Strom abhängig von der Bestrahlungsstärke](
Kennlinie_Bestrahlungsstaerke_Spannung-Strom.jpg){:.right width="550"}
Bei den üblichen Silizium-Solarzellen steigt der entnehmbare Strom
(Kurzschlussstrom) linear mit der Bestrahlungsstärke. Ihre
Leerlaufspannung hingegen steigt schon bei geringer Helligkeit stark an
und nähert sich dann nur noch langsam steigend dem Wert 0,63 V.

Generell sind *monokristalline* Zellen zu bevorzugen, auch wenn sie ein wenig
teurer sind als *polykristalline* oder *amorphe*, weil sie einen höheren
Wirkungsgrad haben.

![Bild: Bypass-Dioden bei der Arbeit](
Bypass-Dioden-bei-der-Arbeit.jpg){:.center}
Leider bricht die
Leistung von in Reihe geschalteten Zellen ein, sobald auch nur eine
davon verschattet ist. Daher werden in den üblichen größeren Modulen
sog. *Bypass-Dioden* eingesetzt, die bei Teilverschattung immerhin einen
Teil der Leistung fließen lassen.

![Bild: Starre Solarpanels](Starre_Solarpanels.png){:width="392"}
![Bild: Flexible Solarpanels](Flexible_Solarpanels.png){:.right width="392"}
[Klassische Solarmodule](https://gruenes.haus/pv-modul-groesse-gewicht/)
haben einen
Aluminiumrahmen und eine Größe von typischerweise ca. 1,7 m × 1 m × 3
cm, was eine Nennleistung von etwa 350 Wp ergibt, und eine Masse von ca.
20 kg. (Semi-)Flexible Module sind teurer als starre und weniger
langlebig, dafür aber viel leichter und nur wenige Millimeter dick. Sie
sind meist auch deutlich kleiner --- typischerweise 1,2 m × 0,5 m bei
einer Nennleistung von 100 Wp und einer Masse von 1 bis 2 kg.
[Hier](https://solar-generatoren.de/die-richtigen-solarmodule-fuers-wohnmobil/)
ein Vergleich verschiedener Solarmodul-Typen in Hinblick auf die
Verwendung für Wohnmobile.

![Bild: starres Schindel-Solarmodul](Schindel-Solarmodul.png){:width="392"}
![Bild:
flexibles Schindel-Solarmodul](Schindel-Solarmodul2.png){:.right width="392"}
Technisch besonders interessant finde ich die überlappende Anordnung und direkte
Verschaltung von Solarzellen ohne Stromschienen (engl. _busbars_) in
[*Schindel-Modulen*](https://www.strom-forschung.de/aktuelles/news/2022/schindel-solarmodule-innovativ-verschaltet-und-industriell-herstellbar)
(engl. _SSP_ = _shingle solar panel_). Dadurch steigt der Wirkungsgrad, weil
die Fläche besser genutzt wird und bei Teilverschattung und Wärme die
Verluste verringert werden. Allerdings ist diese Bauart selten zu finden
und verhältnismäßig teuer, so dass sie nur dann sinnvoll ist, wenn man
Platz sparen will/muss.

#### Elektrischer Anschluss {#Anschluss}

Solarmodule haben als Stromanschluss meist die praktischen MC4-Steckverbinder.
Generell sollten die Solarkabel, also die Verbindungen der Module
(untereinander und zum [Solar-Regler](#Wechselrichter)),
möglichst kurz sein, weil da relativ hohe Ströme fließen,
was proportional zur Länge zu spürbaren Verlusten führt.
Aus dem selben Grund sollte der Querschnitt nicht zu klein sein --- mind. 4mm²,
bei längeren Kabeln und höheren Strömen mind. 6mm² (was allerdings teurer ist).

Solarmodule kann man wie Batteriezellen seriell und/oder parallel verbinden,
um mehr Leistung zu erhalten, ohne für jedes Modul einen eigenen Regler
(bzw. Regler-Eingang) verwenden zu müssen.
Dabei sollten die Module alle gleichartig sein, weil es sonst Verluste gibt.\
Wenige große Solarmodule sind technisch und wirtschaftlich typischerweise
etwas günstiger als entsprechend viele kleine.

-   Bei [*Reihenschaltung*](https://de.wikipedia.org/wiki/Reihenschaltung) (oft
    auch *Serienschaltung* genannt) hängt man die Module einfach hintereinander,
    wobei sich die Spannungen der einzelnen Module addieren.

    Ein Nachteil der Reihenschaltung ist,
    dass es dabei viel leichter zu [Verlusten durch Teilverschattung](
    https://photovoltaikbuero.de/pv-know-how-blog/teilverschattung-bei-solarmodulen-messungen/)
    kommt, weil die Gesamtleistung einbricht, sobald auch nur eines der Module
    verschattet wird.
    Man sollte aus diesem Grund nur Module in Reihe schalten, die
    die gleiche Ausrichtung haben und relativ gleich(zeitig) verschattet werden.

-   Bei [*Parallelschaltung*](https://de.wikipedia.org/wiki/Parallelschaltung)
    addieren sich die Ströme der einzelnen Module. Natürlich sollte die
    (Gesamt-)Spannung auf den parallel geschalteten Strängen gleich sein.

    Der elektrische Verlust ist größer als bei Reihenschaltung,
    andererseits hat man weniger Verluste auf Modulebene bei Teilverschattung.

    Für die parallele Verschaltung bieten sich Y-Kabel mit MC4-Anschlüssen an.
    Die Kabellänge auf parallelen Zweigen sollten ungefähr gleich sein.

    [Hier](
    https://www.photovoltaikforum.com/core/article/49-ost-west-anlage-mit-einem-wechselrichter/)
    ein schöner Artikel für eine klassische Anwendung der Parallelschaltung:
    geteilte Ost-West-Ausrichtung von PV-Modulen auf einem Hausdach
    oder um den Ertrag über den Tag möglichst gleichmäßig zu verteilen,
    ohne dafür unbedingt mehr als einen MPPT-Eingang zu benötigen.

Generell muss man unbedingt darauf achten, dass die maximale Eingangsspannung,
die ein Regler-Eingang verkraftet, nicht überschritten wird --- und
zwar nicht nur bei Normbedingungen (25°C), sondern auch bei sehr niedrigen
Temperaturen, wo die (Leerlauf-)Spannung etwa 10 - 20% höher sein kann.
Der wesentliche Vorteil gegenüber der Parallelschaltung ist, dass
der Strom in den Kabeln und der damit verbundene Verlust nicht steigt.

Im Gegensatz dazu darf der (je nach Einstrahlung und Temperatur) mögliche
(Gesamt-)Strom den spezifizierten Maximalstrom eines Regler-Eingangs durchaus
überschreiten.
Allerdings wird dann PV-Leistung verschenkt, weil der Wechselrichter
im Prinzip nicht mehr Leistung aufnimmt als worauf er ausgelegt wurde.
Auch kann es bei stark wechselnden Lichtverhältnissen und starkem
Strom-Überangebot zu Überlastungen kommen.

![Bild: Strom-Spannungs-Kennlinien abhängig von der Bestrahlungsstärke](
I-V-curves-of-the-solar-panel-under-different-irradiation-levels-and-the-Voltage.png){:.right width="530"}
Zu beachten ist noch, dass die Regler-Eingangsspannung je nach Modell
bis zu 5 V über der gewünschten Ausgangsspannung des Reglers (z.B. der
Speicherbatterie) liegen muss, damit der Regler effektiv Strom liefern
kann. Wenn man z.B. kleine Solarmodule mit 100 Wp und 22,6 V
Leerlaufspannung hat, wird es ohne Reihenschaltung bei einer
Ladeschlussspannung von ca. 14,5 V einer LiFePO4-Batterie bei wolkigem
Wetter (mit vielleicht nur 100 - 200 W/m²) ziemlich eng.

#### Montage {#Montage}

![Bild: Garten-Solaranlage an Hauswand](Garten-Anlage.jpg){:.left width="386"}
![Bild: Solaranlage auf Pergola](Pergola-Anlage.jpg){:.right width="386"}

{:style="clear:both"}
Zur Montage bzw.
Aufständerung von Solarmodulen auf einem Hausdach oder an einem Balkon
[hier](https://www.youtube.com/watch?v=TKeu6YGVuus) ein Überblick-Video.
[Hier](https://machdeinenstrom.de/balkonkraftwerk-montageloesungen-fuer-die-balkonbruestung/)
ein Artikel mit speziellen Tipps zur Installation an einer Balkonbrüstung.
Es gibt aber auch andere Möglichkeiten, wie z.B. auf einer Garage, einem
Gartenhaus, einer Gartenfläche, an der Hauswand oder als Teil einer Pergola.

Wichtig ist, dass die Module sicher angebracht werden, besonders bzgl. Sturm.
Bei über 4 m Montagehöhe gelten besondere Verordnungen für Glasoberflächen,
wenn sich direkt darunter den Menschen bewegen oder aufhalten können.

Bei Anbringung außen am Haus kann es auch Probleme mit dem optischen
Erscheinungsbild geben (daher soweit erforderlich, eine Genehmigung einholen)
und bei spiegelnden Oberflächen eventuell auch mit Blendeffekten.

### Solar-Regler und Wechselrichter {#Wechselrichter}

![Bild: Strom-/Leistungs-Spannungskennlinien einer Solarzelle](
I-U-Kennlinie_MPP_Silizium-Solarzelle.png){:.right width="450"}
Für die Umwandlung des recht volatilen "rohen" Solarstroms auf die gewünschte
(nahezu) konstante Zielspannung benötigt man regelbare *Gleichspannungswandler*,
kurz *Regler* genannt.
Sehr einfache und billige Regler verwenden dazu *Pulsweitenmodulation* (*PWM*).
Wesentlich besser sind aber Regler mit Leistungsoptimierung durch
[*MPPT* (Maximal-Leistungspunkt-Suche, engl. _maximum power point tracking_)](
https://de.wikipedia.org/wiki/Maximum_Power_Point_Tracking), weil sie
auch unter stark schwankenden Bedingungen optimale Energieausbeute bringen.

![Bild: Solar-Microinverter](Solar-Microinverter.png){:.right width="500"}
Für die Umwandlung von Gleichstrom in Wechselstrom (bei uns meist mit
230 V) benötigt man einen
[*Wechselrichter*](https://de.wikipedia.org/wiki/Wechselrichter)
(manchmal auch *Spannungswandler* genannt, engl. _inverter_).
Bei jedem Wechselrichter sollte man darauf achten, dass er ordentlichen
Wechselstrom liefert (sog. *reine Sinuswelle*, engl. _pure sine wave_)
und einen hohen
[Wirkungsgrad](https://www.energie-experten.org/erneuerbare-energien/photovoltaik/wechselrichter/wirkungsgrad)
(engl. _efficiency_) hat.
Außerdem ist empfehlenswert, ihn mit etwas Leistungsreserve zu dimensionieren,
weil seine Lebensdauer sonst leiden und er je nach Bauart
unangenehm lautes Lüftergeräusch verbreiten kann.
Der kritischste Punkt ist, das seine maximale Eingangsspannung nicht
überschritten werden darf, weil er sonst zerstört wird.

#### Netzwechselrichter {#Netzwechselrichter}

Für die Einspeisung ins Stromnetz wird ein *netzgekoppelter Wechselrichter*
verwendet. Dieser wird auch *Netzwechselrichter*, *Einspeisewechselrichter*
oder *fremd geführter Wechselrichter* genannt, weil er sich automatisch
an die Frequenz und Phase des anliegenden Wechselstroms anpasst und bei
fehlendem Stromanschluss den Ausgang abschaltet --- auch aus
Sicherheitsgründen für den Fall, dass ein blanker Stecker berührt werden kann.
Bei Stecker-Solaranlagen wird meist ein *Solar-Mikrowechselrichter* verwendet,
der einen Spannungsregler mit einem Netzwechselrichter integriert.
Im Zusammenhang von Solaranlagen wird meist vereinfacht nur von einem
'*Wechselrichter*' (*WR*) gesprochen.
Zur Dimensionierung von Solar-Wechselrichtern gibt es
z.B. [hier und auf den Folgeseiten](
https://photovoltaikbuero.de/pv-know-how-blog/ist-bei-der-wechselrichterauslegung-zu-beachten-kriterium-1/)
ausführliche Hinweise.

Im Gegensatz zu Solarkabeln (s.o.) können 230 V-Kabel
zwischen Netzwechselrichter und Steckdose durchaus länger sein (z.B. 5 - 10 m).
Allerdings kann es dort je nach Kabellänge und -Querschnitt bei größeren Strömen
zu einem höheren Spannungsabfall kommen, der die Netzkoppelung des WR stört.

#### Gleichspannungswandler {#Gleichspannungswandler}

![Bild: Gleichspannungswandler mit regelbarer Strombegrenzung](
DC-DC-converter.png){:.right width="400"
style="margin-left: 40px; margin-right: 40px"}
Für die Nutzung zur [regelbaren Einspeisung](#Batteriepuffer) aus einem
Strompuffer ins Hausnetz braucht man eine einstellbaren Strombegrenzer,
wie er in manchen *Gleichspannungswandler* (engl. _DC-to-DC-converter_)
enthalten ist. Er sollte möglichst wenig Verluste haben. Wenn er einen
[Aufwärtswandler](https://de.wikipedia.org/wiki/Aufw%C3%A4rtswandler)
(engl. _boost converter_ oder _step-up converter_) enthält,
kann er zudem dazu benutzt werden,
die Spannung der Pufferbatterie (z.B. 12 V) auf eine für den Eingang
des Netzwechselrichters passende Spannung (z.B. mindestens 20 V) zu bringen.

#### Inselwechselrichter {#Inselwechselrichter}

![Bild: Wechselrichter](Wechselrichter.png){:.right width="500"}
*Inselwechselrichter*, auch *selbst geführte Wechselrichter* genannt,
werden vom Stromnetz unabhängig betrieben. Mit ihnen kann man die üblichen
Haushaltsgeräte auch im Falle eines Stromausfalls mit einer Batterie versorgen,
natürlich nur im Rahmen der Belastbarkeit und Kapazität der Batterie.
Auch bei dieser Art von Wechselrichter ist darauf zu achten,
dass er eine reine Sinusspannung liefert und sein Wirkungsgrad hoch ist.
Hinzukommt, dass sein Leerlauf-/Ruhestromverbrauch
(engl. _standby power consumption_) gering sein sollte,
seine Dauerleistung groß genug für die daran betriebenen Geräte sein muss
und dass seine Spitzenleistung auch deren Anlaufstrom abdecken muss.
Die benötigte Anlaufleistung eines Kühl- oder Gefrierschrankes kann das
[Fünffache der Scheinleistung](
http://www.off-grid-systems.de/mediafiles/Sonstiges/bedienungsanleitung/Wechselrichter/Handbuch-LMP3000W.pdf)
(angegeben in Volt × Ampere = VA, nicht nur [Wirkleistung](
https://www.energie-experten.org/energie-sparen/strom-sparen/elektrischer-strom/schein-wirk-blindleistung),
angegeben in Watt) im laufenden Betrieb betragen.
Da können schon mal 1000 VA zusammenkommen (wenn auch nur für 1-2 Sekunden).

### Solar-Laderegler {#Laderegler}

![Bild: Solar-Laderegler](Solar-Laderegler.png){:.right width="400"
style="margin-left: 70px; margin-right: 70px"}
Wenn man über Solarmodule eine Batterie laden möchte, benötigt man einen
*Solar-Laderegler*, der einen Spannungsregler mit einem Batterieladegerät
verbindet. Mit billigen chinesischen (angeblich) MPPT-Reglern habe ich
keine guten Erfahrungen gemacht, wohl aber mit den europäischen Marken
Victron und Votronic.

### Hybridgeräte: Solar-Laderegler mit Wechselrichter {#Hybrid}

![Bild: Hybrides Solar-Ladegerät mit Wechselrichter](
Solar-off-grid-inverter.png){:.right width="450"}
Es gibt auch
[Kombigeräte](https://www.solarserver.de/2021/07/26/green-cell-bietet-neuen-solarwechselrichter-an/), welche
die Funktionen Solar-Laderegler, Batterie-Netzladegerät und
Inselwechselrichter in sich vereinen. Damit können Elektrogeräte
vorzugsweise direkt mit Solarstrom versorgt werden, wobei die
überschüssige Energie in einer Batterie gespeichert wird. Bei
unzureichender Stromversorgung aus den Solarmodulen ergänzt das Gerät
die benötigte Energie automatisch aus der Batterie und schaltet bei
leerer Batterie (oder je nach konfigurierter Präferenz auch schon bei
fehlendem Solarstrom) auf eine externe Stromquelle (Stromnetz oder
Generator) um, worüber auch die Batterie geladen wird.
Solch ein Kombigerät ist in seiner Funktionsweise sehr praktisch, braucht
weniger Platz, ist im Einkauf günstiger und zudem einfacher zu installieren
und zu verwenden als entsprechende Einzelkomponenten. Es hat aber [auch
Nachteile](https://www.oeko-energie.de/shop1/de/Solarstrom/Insel-WR/Kombigeraet-Laderegler-MPPT-Wechselrichter-Batterieladegeraet/)
wie geringe Flexibilität bei der Komponentenwahl
und größere Wahrscheinlichkeit für einen Ausfall und dann höhere Kosten.

Offenbar gibt es auf dem Markt kein Gerät, das neben der Nutzungsart
für eine Inselanlage (also netzunabhängige Stromversorgung) auch
die einer Stecker-Solaranlage (also Netzeinspeisung des Solarstroms,
idealerweise mit Nachteinspeisung aus der Batterie) ermöglicht.

### Speicherbatterien {#Speicher}

![Bild: LiFePO4-Batterie mit 4 prismatischen Zellen](
LiFePO4-Batterie.png){:.right width="450"}
Für die Stromspeicherung bieten sich heutzutage
[*Lithium-Eisenphosphat*-Batterien](
https://de.wikipedia.org/wiki/Lithium-Eisenphosphat-Akkumulator)
(*LiFePO<sub>4</sub>* oder noch kürzer *LFP*) an.
Diese sind zwar erheblich teurer als *Blei-Säure-Batterien* (inkl. Varianten wie
AGM), wie man sie vom Auto kennt, aber sind wartungsfrei, nicht so groß und
schwer, sowie viel spannungsstabiler und langlebiger. Sie haben weniger
Selbstentladung, einen deutlich höheren Wirkungsgrad (über 90%) und vertragen
ein Vielfaches an Lade-/Entladezyklen sowie recht hohe Lade-/Entladeströme,
so dass sie in weniger als einer Stunde geladen bzw. entladen werden können.
Im Vergleich zu anderen Lithium-Ionen-Akkutypen wie Lithium-Polymer (LiPo),
welche eine noch höhere Energiedichte und keinerlei "Memory-Effekt" haben,
sind sie recht robust und sicher und sind weniger umweltschädlich.\
Alle Lithium-basierten Batterien benötigen, anders als Blei-Batterien, für die
Reihenschaltung der internen Akkuzellen ein sog. *Batteriemanagementsystem*
(*BMS*), das für eine gleichmäßige Spannungsverteilung der Zellen sorgt.\
Eine typische 100 Ah Autobatterie wiegt etwa 26 kg und kostet nur etwa 100€.
Aus ihrer Nennkapazität von 12 V × 100 Ah = 1200 Wh sollte man aber höchstens
50% entnehmen, damit die Batterie nicht durch Tiefentladung Schaden nimmt,
also maximal 600 Wh.
Selbst dann hält ein Bleiakku nur etwa 500 bis 1000 Lade-/Entladezyklen.\
Die Zahl der Lade-/Entladezyklen eines LiFePO4-Akkus, bis die Kapazität merklich
nachgelassen hat, wird mit etwa 5000 angegeben, die Zahl der Jahre mit 15 - 20.
Eine 12,8 V 100 Ah LiFePO4-Batterie wiegt etwa 11 kg und kann problemlos zu 90%
entladen werden, so dass sich eine effektive Kapazität von 1150 Wh ergibt.
Unter Berücksichtigung von Speicherungsverlusten und des Wandlungsverlustes
eines Wechselrichters lässt sich damit ein Gerät mit 1000 W Verbrauch
(z.B. Staubsauger, Kaffeemaschine oder Fön) etwa eine Stunde lang betreiben.

#### Batterie-Dimensionierung {#Dimensionierung}

Um den Wandlungsverlust von ca. 10% eines Wechselrichters zu vermeiden,
sollte man bei einer Inselanlage die Verbraucher möglichst direkt an der
Batterie anschließen, was z.B. bei LED-Lampen, Radios und
USB-Ladebuchsen gut machbar ist --- aber auch bei Laptops,
wenn man für sie ein Netzteil mit 12 V (statt 230 V) Eingang verwendet.
Bei mittlerer Last von 25 W ergeben sich mit einer voll geladenen 12,8 V 100 Ah
LiFePO4-Batterie gut 50 Stunden Betriebszeit. Ein durchschnittlicher 3,6 V
Smartphone-Akku mit 2500 mAh hat 9 Wh Kapazität.
Wenn er jeweils zu 80% entladen ist, lässt er sich damit etwa 160 mal aufladen.\
Zum Vergleich: Eine Powerbank mit nominell 20.000 mAh Kapazität hat
(aufgrund oft stark überzogener Hersteller-Angaben und Verlusten bei der
Wandlung von 3,6 V auf die 5 V eines USB-Anschlusses) effektiv eher die
Hälfte dieser Kapazität. Ein durchschnittlicher Smartphone-Akku lässt
sich über die Powerbank in der Praxis nur etwa 10 mal aufladen.

Der Preis einer Batterie pro kWh sinkt mit steigender Größe/Gesamtkapazität.

#### Batterie-Strukturierung {#Strukturierung}

![Bild: Spannung](What-are-Ohm-Amps-and-Volts.jpg){:.right width="400"}
Wenn man die Wahl
hat zwischen höherer Spannung (d.h. mehr Akkuzellen in Reihe) oder
größere bzw. mehr Zellen parallel, dann besser die höhere Spannung nehmen.
Also ist z.B. eine 24 V 100 Ah Batterie einer mit 12 V und 200 Ah vorzuziehen,
aus folgenden Gründen:

-   Hohe Ströme belasten elektronische Bauteile besonders stark, bringen
    mehr Verluste und verlangen größere Kabelquerschnitte, die schnell
    unhandlich werden.

-   Ein Solar-Laderegler ist vor Allem durch seinen Ausgangsstrom
    begrenzt. So verkraftet ein [Victron BlueSolar MPPT
    100/30](Datenblatt_BlueSolar-MPPT-100-30-100-50.pdf) eine
    PV-Leerspannung von max. 100 V (was die Reihenschaltung von
    mindestens 2 Solarmodulen erlaubt). Er liefert einen max. Ladestrom
    von 30 A, woraus sich bei Betrieb an einer 12 V Batterie eine
    maximale Leistung von 360 W ergibt, bzw. unter Berücksichtigung von
    PV-Verlusten eine sinnvolle maximale Leistung der Solarmodule von
    440 Wp. Bei 24 V Batteriespannung ist hingegen die doppelte Leistung
    (880 Wp) möglich. Wenn man anders herum für die doppele PV-Leistung
    bei 12 V Batteriespannung bleiben will bzw. muss, braucht man einen
    Laderegler mit doppelter Strom-Belastbarkeit, und der kostet ca. 50
    bis 80% mehr.

-   Vermutlich arbeiten Wechselrichter mit 24 V Eingangsspannung etwas
    effizienter als solche mit 12 V, zumal Strom und Spannungsspreizung
    geringer sind.

Man kann auch mehrere Batterien in Reihe (also hintereinander) schalten, um
z.B. auf 2 × 12 V = 24 V zu kommen,
muss dann aber für eine dauerhafte *Balancierung* (gleichmäßige Spannungslage)
der Einzelbatterien sorgen, wie es auch das BMS innerhalb einer Batterie
für die Einzelzellen tut. Dafür gibt es
spezielle *Batterie-Balancierer* (engl. _balancer_ oder _equalizer_),
wie im [Video von Dimitri](https://youtu.be/BcWKrPj6-qs) schön vorgeführt.

#### Kombination aus Batterie und Wechselrichter {#Kaskadierte}

Ganz anders als herkömmliche Batterien und Wechselrichter funktioniert
die patentierte sog. [*Kaskadierte H-Brücken*-Technologie](
https://www.finepower.com/fachartikel-hocheffizienter-umrichter-fuer-batteriespeichersysteme/),
der [Firma SAX](https://sax-power.net/).
Dabei schaltet eine komplexe Software-Regelung, die gleichzeitig als BMS dient,
einzelne LiFePO4-Batteriezellen zur Einspeisung zyklisch so zusammen, dass
darüber sehr direkt die nötige Wechselstrom-Sinuskurve synthetisiert wird.
Daraus ergeben sich einige Vorteile, insbesondere ein Wirkungsgrad von über 99%,
besonders platzsparende und langlebige Batterien ohne externen Wechselrichter,
sowie die Nutzbarkeit zur Einspeisung und als Notstromanlage mit USV-Funktion.
Leider sind die Produkte sehr teuer: 5700€ für eine Anlage mit 5,2 kWh.

#### Tiefsetzsteller {#Tiefsetzsteller}

![Bild: Tiefsetzsteller](Tiefsetzsteller.png){:.right width="300"
style="margin-left: 70px; margin-right: 70px"}
Ein Problem bei einer
Batteriespannung von 24 V (oder 48 V) ist, dass Niederspannungs-Geräte
typischerweise eher mit 12 V zu betreiben sind. Aber dafür gibt es für
Geräte mit mäßigem Verbrauch (bis etwa 5 A, also 60 W) eine recht
effiziente und kostengünstige Lösung, nämlich sog. *Tiefsetzsteller*
(auch *Abwärtswandler*, engl. _DC-DC buck converter oder _step-down converter_).

#### Spannungswächter {#Spannungswächter}

{:style="clear:both"}
![Bild: Programmierbarer Batteriespannungswächter](
Battery_voltage_protector.png){:.right width="500"
style="margin-left: 50px; margin-right: 50px"}
Für die Nutzung als [automatischen Strompuffer](#Batteriepuffer) zur
zeitversetzten Einspeisung ins Hausnetz braucht man einen *Spannungswächter*,
der die Einspeisung bei nahezu voller Batterie einschaltet und bei nahezu
leerer Batterie wieder ausschaltet. Dazu gibt es einfache fertige Module,
die man nur noch geeignet anschließen und einstellen muss.

Beispiel-Konfigurationen {#Konfigurationen}
------------------------

### Mobile Inselanlage {#Mobilanlage}

Für unser Wohnmobil verwende ich seit Sommer 2019 folgende relativ günstige
Komponenten zu meiner vollen Zufriedenheit:

-   2 × 100 Wp flexible Solarpanels [Dokio
    DFSP-100M](https://www.amazon.de/DOKIO-Batterie-wasserdicht-Wohnmobil-Oberfl%C3%A4che/dp/B07FYW3C6W),
    ca. 180€\
    Diese habe ich einfach auf das Blechdach unseres Wohnmobils geklebt.
    Etwas lästig war die Kabelführung ins Innere.

-   15 A Solar-Laderegler [Victron BlueSolar MPPT
    75/15](https://www.ebay.de/itm/142083505206), ca. 90€\
    Dieser Regler unterstützt Batterien mit 12 oder 24 V und Ladeströme
    bis 15 A (wobei für die o.g. Solarzellen bei Dachmontage in der
    Praxis auch 10 A genügt hätten).\
    Sehr praktisch finde ich bei den BlueSolar-Modellen die
    Status-Abfrage auf dem Smartphone.\
    Leider unterbinden die Victron-Regler ohne Zusatzgerät nicht das Laden
    bei unter 0°C, was bei LiFePO4-Akkus zu Schäden führen kann,
    wenn man sie im Winter nicht abklemmt.

-   12,8 V 100 Ah 4S1P LiFePO4-Batterie inkl. 100 A BMS [Delong
    DL-12100](https://www.alibaba.com/product-detail/Delong-Factory-Rechargeable-12-8V-100Ah_62388029440.html),
    inkl. DDP-Versand direkt aus China ca. 400€\
    In Deutschland werden solche Batterien hingegen für ungefähr 1000€
    verkauft. Siehe auch [meinen
    myDealz-Beitrag](https://www.mydealz.de/deals/12v-100ah-lifepo4-akku-mit-bms-ab-400-zb-fur-solaranlage-oder-wohnmobilbatterie-ersatz-1350559)
    dazu mit interessanter Diskussion.

-   [2000 Wp
    Wechselrichter](https://de.aliexpress.com/wholesale?SearchText=pure+sine+wave+inverter+2000w),
    ebenfalls direkt aus China, ca. 70€

### Stecker-Solaranlage {#Steckeranlage}

Für eine sehr einfache, aber effiziente Anlage zur Netzeinspeisung finde
ich folgende Komponenten besonders interessant:

-   2 × 400 Wp starre SSP [EcoDelta -
    ECO-400M-66SA](Datenblatt_ECO-380-400M-66SA.pdf) mit besonders hoher
    Effizienz: 213 Wp/m², ca. 540€\
    oder 4 × 150 Wp flexible ETFE SSP Solarmodule [Solarfam
    SZ-150-36MFE](Solarfam_SSP_SZ-150-36MFE.pdf) mit 188 Wp/m², ca.
    [664€](https://stromvoll.com/shop/#!/150W-Flexible-Solar-panel-1170-x-680-x-2-mm/p/396304457)\
    oder 2 × 310 Wp sehr langlebige flexible Solarmodule [Sunman eArc
    SMF310M-6X10DW](Datenblatt_Sunman_flexible_310W.pdf) mit 187 Wp/m²,
    ca.
    [715€](https://shop-lieckipedia.de/Ab-2-Stueck-310-Watt-Solarmodul-monokristallin-flexibel-Sunman)

-   4-in-1 Mikrowechselrichter 1200 W [Hoymiles
    HM-1200](https://www.hoymiles.com/product/microinverter/hm-1200-1500-as/),
    ca. 230€\
    oder 1000 W Micro Grid Tie Inverter Inverter
    [SG1000MQ](https://www.ebay.de/itm/124731502486), ca. 200€\
    oder 600 W WR mit 2 × 400 W MPPT-Eingang und WLAN [Deye Sun1600g3-EU-230](
    https://deye.com/de/product/sun600-800-1000g3-eu-230-600-1000w-single-phase-2-mppt-micro-inverter-rapid-shutdown/),
    ca. 215€\
    _Achtung, in älteren Softwareversionen (bis ca. Ende 2022) reißen
    die Wechselrichter von Deye, sowie baugleich Bosswerk und revolt (Pearl),
    beim WLAN-Zugang [sträfliche Sicherheitslücken](
    https://www.photovoltaikforum.com/thread/187077-achtung-wifi-sicherheit-der-deye-und-bosswerk-mi600-300-sowie-baugleiche-microwe/).
    Daher sollte ihre WLAN-Funktion höchstens in einem Gastnetz genutzt werden._

### Kombi-Anlage {#Kombianlage}

![Bild: Balkonsolaranlage mit senkrechten flexiblen Modulen
](Balkonsolaranlage_senkrecht_flexibel.jpg)

Als Balkonanlage mit wahlweise direkter oder gepufferter Netzeinspeisung,
aber auch für eine Notstromversorgung daheim und für einen längeren autarken
Aufenthalt mit dem Wohnmobil habe ich seit Sommer 2022 folgende Komponenten:

-   4 × [150 Wp flexible ETFE SSP
    Solarmodule](https://www.solarfam.nl/150w-shingle-etfe-flexible-solar-panel-solarfam.html),
    für 600€\
    _Zuvor hatte ich mir gekauft, aber nicht verwendet, weil mir ihre
    Anbringung an der Balkonbrüstung im 4. Stock zu riskant war:\
    4 × [120Wp starre Eco-Worthy
    Solarpanel](https://www.manomano.de/p/2x120watt-solarpanel-solarmodul-12v-12volt-monocrystalline-wohnwagen-wohnmobil-48845318),
    für 320€\
    Diese Eco-Worthy Module kann ich empfehlen, wenn man keine größeren
    verwenden kann. Sie bringen jedenfalls die versprochene
    Spitzenleistung, was gerade bei günstigen Modellen nicht
    selbstverständlich ist._

-   700 W Netzwechselrichter mit 2 × MPPT und WLAN [Mars Rock
    EC700MD](https://de.aliexpress.com/item/1005002469159821.html) (oder
    [ähnlich mit LCD](https://www.ebay.de/itm/165694072328)), ca. 135€
    inkl. Versand\
    _Zumindest bei meinem Gerät funktioniert das WLAN nicht._

-   24 V Hybridwechselrichter
    [EASun ISolar SPH-3K](https://de.aliexpress.com/item/1005003665568494.html)
    mit 3000 VA (6000 VA Spitzenlast) reiner-Sinus-Wechselrichter
    (mit USV-Funktion und angeblich 93% max. Wirkungsgrad),
    40-50 A PWM Solar-Laderegler und 20-30 A Batterieladegerät über Netzstrom,
    für 185€\
    _Leider hatte ich nicht aufpasst, die
    [MPPT-Version](https://de.aliexpress.com/item/1005004488463489.html)
    zu bestellen, deren Solarwandlungs-Effizienz wohl deutlich besser wäre_.

-   24 V 100 Ah LiFePO4-Batterie mit 8S1P-Konfiguration inkl. 100 A BMS
    und Display [CERRNSS LF-24100
    small](https://de.aliexpress.com/item/1005003937833782.html), ca.
    570€\
    _Diese Zellen sind [qualitativ allerdings nicht ganz so
    gut](https://www.youtube.com/watch?v=4OYlp1aMtTU) wie die von
    Delong.\
    Noch günstiger und sehr hochwertig geht es im [Eigenbau: 12 V 280 Ah
    schon ab 600€](https://www.youtube.com/watch?v=F0Ot7JOR2VM)._

-   24 V auf 12 V Tiefsetzsteller 60W [Akozon GYVRM / LY-KREE / Cocar
    K241205](https://www.amazon.de/Netzteil-Spannungswandler-Transformator-Konverter-Sonnensystem-5A/dp/B01KQWWQUI)
    mit angeblich 96% Wirkungsgrad, ca. 13€

-   Programmierbarer Batteriespannungswächter [DC 6-40V LED Battery Charger
    Discharger Board Under Over Voltage Protection Module](
    https://www.ebay.de/itm/313940626703),  ca. 6€

-   Gleichspannungswandler mit Strombegrenzung [300W 20A DC DC Wandler
    Step Down Wandler Konverter Spannungsregler, einstellbar](
    https://www.ebay.de/itm/385099914040), ca. 12€

<!--
LocalWords: title keywords toc start refresh zusammenfassung abgrenzung pv end
LocalWords:  inhaltsverzeichnis photovoltaik sonneneinstrahlung
LocalWords:  nennleistung jahresertrag ausrichtung solarmodulen
LocalWords:  nutzungsmöglichkeiten nutzung netzeinspeisung fuer
LocalWords:  stecker solaranlage balkonkraftwerk beschränkung
LocalWords:  kappung kappungsverlust drosselung stromzähler md
LocalWords:  rücklaufsperre stromverbrauch haushalt berechnung
LocalWords:  verbrauchsmessung eigenverbrauch eigendeckung ref
LocalWords:  ertragsberechnung monatsbasierte amortisation of
LocalWords:  rechner speichersimulation simulation minutenbasis
LocalWords:  hausnetzeinspeisung batteriepuffer stromspeicher
LocalWords:  regelungsstrategien speicherbatterie einspeisung
LocalWords:  batterieladung batterie inselanlage kombination px
LocalWords:  batteriespeicherung auswahl komponenten anschluss
LocalWords:  solarmodule montage solar regler wechselrichter pl
LocalWords:  netzwechselrichter gleichspannungswandler beispiel
LocalWords:  inselwechselrichter laderegler hybridgeräte kombi
LocalWords:  speicherbatterien dimensionierung strukturierung
LocalWords:  tiefsetzsteller spannungswächter konfigurationen
LocalWords:  mobilanlage steckeranlage anlage kombianlage index
LocalWords:  pandoc output calculation power width style margin
LocalWords:  left right irradiance GHI buehneTop clear both png
LocalWords:  potential csv grid tie inverter tmy peff ieff curb
LocalWords:  standby xls jpg Balkonsolar center limiter off to
LocalWords:  blackout brownout panels busbars shingle panel up
LocalWords:  maximum point tracking sine wave efficiency boost
LocalWords:  converter step consumption pdf balancer equalizer
LocalWords:  buck down SA SZ DW MQ EC LF small LY KREE Battery
LocalWords:  Charger Discharger Board Under Over Voltage Protection
-->
