---
title: "Insel- und Kombianlagen - Mini-Solaranlagen für daheim und unterwegs"
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
    -   [Hausnetzeinspeisung mit Batteriepuffer](Speicher.md)
    -   [Inselanlage (mit Batteriespeicherung)](#Inselanlage)
    -   [Kombination aus Hausnetzeinspeisung und Inselanlage](#Kombination)
-   [Auswahl und Nutzung von Komponenten](Komp.md)
-   [Beispiel-Konfigurationen](Bsp.md)

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

Ähnlich wie die [Batteriepufferung](Speicher.md) ist diese Nutzungsart
flexibler, aber wegen der nötigen zusätzlichen Komponenten (v.A. der Batterie)
auch deutlich teurer und auch etwas anfälliger und wartungsintensiver
als die [direkte Netzeinspeisung](SSG.md#SSG).
Wirtschaftlich rentabel für die Nutzung zu Hause kann das bei den
derzeitigen Preisen nur sein, wenn man eine geeignete Batterie schon aus
anderen Gründen (z.B. für den mobilen Einsatz in einem Fahrzeug) hat und
die zusätzliche Nutzungsart auch zeitlich alternativ dazu möglich ist.

### Kombination aus Hausnetzeinspeisung und Inselanlage {#Kombination}

Wenn die für die betreffenden Varianten nötigen Funktionen gleichzeitig
installiert sind, kann man zwischen Netz-, Puffer- und Inselbetrieb
auch bedarfsweise wechseln. Dabei wird der Ausgang der Solarmodule
zwischen dem netzgekoppelten Wechselrichter und dem Solar-Laderegler
umgeschaltet (oder ohne Schalter einfach umgestöpselt) bzw.
am Ausgang der Batterie zwischen Netz- und Insel-Wechselrichter umgeschaltet.


<!--
Local IspellDict: german8
LocalWords: title description created changed png right width md nbsp index Komp
LocalWords: off grid blackout brownout
-->
