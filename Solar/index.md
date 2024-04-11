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

Mit einem sog. [*Steckersolargerät*](SSG.md#SSG) kann man einfach und günstig
[Solarstrom](PV.md#Photovoltaik) gewinnen
und über eine Steckdose direkt ins Hausnetz einspeisen.
Das spart Stromkosten und rechnet sich je nach verwendeten
[Komponenten](Komp.md#Komponenten), [Aufstellung](PV.md#Ausrichtung) der Solarmodule
und [Stromverbrauch](SV.md#Stromverbrauch) schon nach wenigen Jahren Betrieb ---
allerdings nur soweit man den Strom auch gleichzeitig
[selbst verbraucht](EV.md#Eigenverbrauch).
Weil diese Betriebsart den überschüssigen Strom an die Allgemeinheit weitergibt
und keine Batterie benötigt, ist sie für die ökologische Gesamtbilanz am besten.

Für eine gewisse Unabhängigkeit von der nicht ständig kräftig vorhandenen
Sonneneinstrahlung und vom allgemeinen Stromnetz
braucht man eine aufladbare Batterie als Stromspeicher und weitere Geräte,
was das Ganze deutlich aufwendiger und teurer macht.\
Mit [*Strompufferung*](Speicher.md#Batteriespeicher)
und einer geeigneten vom aktuellen Verbrauch im Haushalt abhängigen
[Regelung](Speicher.md#Regelungsstrategien)
lässt sich überschüssige Energie zwischenspeichern
und bei Bedarf wieder abrufen und damit der Eigenverbrauchsanteil erhöhen.\
Eine [*Inselanlage*](Insel.md#Inselanlage) ist ohne Stromanschluss verwendbar,
soweit die Speicherkapazität und Sonneneinstrahlung zum Nachladen reicht.

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
        - [Details zum Shelly (Pro) 3EM](SV.md#Shelly3EM)<a name="Shelly3EM"></a>
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
    -   [Hausnetzeinspeisung mit Batteriepuffer](Speicher.md#Batteriespeicher)<a name="Batteriepuffer"></a>
        - [Regelungsstrategien für PV-Speicher](Speicher.md#Regelungsstrategien)<a name="Regelungsstrategien"></a>
        - [Dimensionierung des Stromspeichers](Speicher.md#Dimensionierung)<a name="Speicherbatterie"></a>
        - [Kommerzielle SSG-Speicherlösungen](Speicher.md#kommerziell)<a name="SSG-Speicher"></a>
          - [Zendure SolarFlow und AIO 2400](Speicher.md#SolarFlow)<a name="SolarFlow"></a>
          - [Anker Solix](Speicher.md#Solix)<a name="Solix"></a>
          - [Maxxisun Maxxicharge](Speicher.md#Maxxicharge)<a name="Maxxicharge"></a>
          - [Tentek Tribune bzw. Anfuote EMS](Speicher.md#Tentek)<a name="Tentek"></a>
          - [Weitere Produkte](Speicher.md#sonstige)<a name="SSG-Speicher-sonstige"></a>
          - [Zusammenfassung und Effizienzbetrachtung](Speicher.md#Effizienz)<a name="SSG-Speicher-Effizienz"></a>
        - [SSG-Speicherlösungen im Eigenbau](Speicher.md#Eigenbau)<a name="SSG-Speicher-Eigenbau"></a>
          - [Implementierung der Speicher-Regelung](Speicher.md#Regelungsimplementierung)<a name="Regelungsimplementierung"></a>
          - [Einfache und günstige Lösung: OpenDTU-OnBattery](Speicher.md#OpenDTU-OnBattery)<a name="OpenDTU-OnBattery"></a>
          - [Weiteres Beispiel für DC-gekoppelten Speicher](Speicher.md#SSG-DC-gekoppelt)<a name="SSG-DC-gekoppelt"></a>
          - [Ladung des Stromspeichers](Speicher.md#Ladung)<a name="Ladung"></a>
          - [Konstanteinspeisung](Speicher.md#Konstanteinspeisung)<a name="Konstanteinspeisung"></a>
          - [Lastgeregelte Einspeisung](Speicher.md#lastgeregelt)<a name="lastgeregelt"></a>
    -   [Inselanlage (mit Batteriespeicherung)](Insel.md#Inselanlage)<a name="Inselanlage"></a>
    -   [Kombination aus Hausnetzeinspeisung und Inselanlage](Insel.md#Kombination)<a name="Kombination"></a>
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

<!--
Local IspellDict: german8
LocalWords: title name description date created changed keywords Komp extension
LocalWords: This is the abstract iextension yaml metadata jpg md CC BY toc
LocalWords: markdown start refresh end pandoc index output nbsp
LocalWords: PVCalculator Regelungsimplementierung SOL
-->
