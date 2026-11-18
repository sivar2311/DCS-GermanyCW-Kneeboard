# Kneeboard-Karten für DCS: Germany Cold War

[English](README.md) | **Deutsch**

Platzkarten (GND) und Parkpositionskarten (PAR) für alle Flugplätze mit befestigter Bahn ab 1000 m der DCS-Karte **Germany Cold War**, auch für die Plätze in Dänemark, Schweden und Polen. Grasplätze sind nicht enthalten. Gestaltet sind die Karten nach dem Vorbild der offiziellen DCS-Karten für den Kaukasus.

> Inoffizielle Karten, nicht von Eagle Dynamics. Nur für die Simulation, **nicht für die reale Navigation**.

Alle Inhalte werden automatisch aus den Dateien der DCS-Installation erzeugt: Bahnen, Rollwege, Schilder, Haltepunkte, Parkpositionen, Gebäude, Frequenzen und Funkfeuer. Es wurde nichts von Hand nachgezeichnet.

## Ordner

| Ordner | Inhalt |
|---|---|
| `png/` | Karten als Bild (1536 × 2048 Pixel), z. B. für das Kneeboard |
| `svg/` | Dieselben Karten als Vektorgrafik, verlustfrei skalierbar |

## Dateinamen

`NN_TYP_KENNUNG_Name[ - Zweitname][_Pn]`

| Teil | Bedeutung |
|---|---|
| `NN` | Nummer des Flugplatzes. Alle Plätze sind alphabetisch nach ihrer Kennung sortiert, wie bei den DCS-Karten. |
| `TYP` | `GND`: Platzkarte (Aerodrome Chart). `PAR`: Parkpositionen (Aircraft Parking Positions). |
| `KENNUNG` | ICAO-Code oder Ersatzkennung (siehe unten) |
| `Name` | Name des Platzes, wie er in DCS heißt |
| `Zweitname` | heutiger Name, falls er vom DCS-Namen abweicht, z. B. `Schkeuditz - Leipzig-Halle` |
| `_Pn` | Blatt n, wenn ein Platz mehrere Blätter hat: P1 ist die Platzkarte, ab P2 kommen die Parkpositionen |

Oben auf jedem Blatt steht der Verweis für die Kartenmappe, z. B. `GND 59 · P2/6` (Bodenkarten, Platz 59, Blatt 2 von 6).

## Übersichtskarte

`00_01_General_Map` zeigt alle Flugplätze mit Nummer und Symbol (Militär, ehemals sowjetisch, ziviler Flughafen, Flugplatz, Straßen-/Autobahnabschnitt). Darunter steht die Liste aller Plätze. Kartengrundlage ist Natural Earth (Public Domain), ergänzt um die innerdeutsche Grenze; Berlin ist gestrichelt umrandet.

## Kennungen

- **ICAO-Codes** (`EDxx`, `ETxx`): die heute gültigen Codes laut der deutschen Wikipedia-Liste „Liste von ICAO-Codes in Deutschland mit Flugplatzangaben“.
  - Hat ein Platz einen zivilen und einen militärischen Code, gilt der heutige: Mendig EDRE, Neubrandenburg ETNU.
  - Gatow (RAF, **EDBG**) und Sembach (USAF, **ETAS**) tragen ihren historischen Code aus der Zeit des Kalten Kriegs.
  - Viele Plätze in der ehemaligen DDR haben ihren ICAO-Code erst nach 1990 bekommen. Sie waren früher Plätze der NVA oder der sowjetischen Streitkräfte.
- **`XE..`**: ehemalige sowjetische Flugplätze in der DDR, die keinen ICAO-Code haben. Die Kennung ist **erfunden**:
  - `X` steht für „kein offizieller ICAO-Code“, nach dem Vorbild von XRMF Mozdok auf den DCS-Kaukasus-Karten.
  - `E` steht für die ICAO-Region Nordeuropa.
  - Dazu kommen zwei Buchstaben aus dem Namen: **XESB** = **S**pere**nb**erg, **XEDG** = **D**am**g**arten.
- **Ausland:** EKCH Kastrup, EKRN Bornholm, ESMS Sturup, EPSC Szczecin-Goleniów. Chojna (Polen) war ein sowjetischer Fliegerhorst ohne ICAO-Code und bekommt nach derselben Regel **XECJ**.
- **`A1`, `A9` …**: Autobahn-Notlandeplätze. **`RV13`** (Tagra, Schweden) ist ein Notlandeabschnitt der Riksväg 13 und wird genauso behandelt. Statt eines Codes steht die Autobahn, auf der der Abschnitt liegt. Abgeleitet ist sie aus Lage und Bahnrichtung.

## Platzkarte (GND)

- Bahnen mit nutzbarer Länge (aus der Bahnbefeuerung in DCS) und Breite, Bahnbezeichnungen
- **Kurse magnetisch:** Die Missweisung ist für jeden Platz einzeln berechnet, mit dem Erdmagnetfeldmodell, das DCS selbst verwendet. Bezugsdatum ist der 1.6.1999, das Standarddatum einer neuen DCS-Mission auf dieser Karte. Der Nordpfeil zeigt rechtweisend Nord (TN), magnetisch Nord (MN) und die Missweisung, z. B. `VAR 0.3° E (1999)`. In Missionen mit anderem Datum weicht die Missweisung etwas ab.
- Rollwege mit Buchstaben (aus den Rollwegschildern in DCS)
- Haltepunkte `P1`, `P2` … mit Koordinaten (aus den Halteschildern), wie auf den DCS-Karten
- Tabellen: ILS, ARP, Platzhöhe, Maßstab, TORA/TODA/ASDA/LDA, Funkfrequenzen, Navigationsanlagen

## Parkpositionen (PAR)

- Jede Parkposition trägt **genau die Nummer, die DCS im Missionseditor anzeigt**. Startpositionen auf der Bahn sind nicht eingezeichnet.
- **Darstellung:** Jede Parkposition ist nur ihre Nummer, direkt an der Position. In Reihen steht sie quer zur Reihe, damit benachbarte Nummern nicht zusammenstoßen. Gibt DCS eine Nummer doppelt aus (ein Fehler in den DCS-Daten, z. B. zweimal „27“ in Celle), steht sie auch auf der Karte doppelt.
- **Eignung:** Die Tabelle unten auf dem Blatt nennt für jede Ramp, geprüft am Missionseditor:
  - **AIRCRAFT:** alle Positionen, die Flugzeuge nutzen können, also normale Abstellflächen sowie Shelter und Hangars,
  - **HELICOPTER:** alle Positionen, die Hubschrauber nutzen können, also normale Abstellflächen und Hubschrauberplätze.

  Normale Abstellflächen eignen sich für beide und stehen deshalb in beiden Spalten. Frühere Heeresflieger- und sowjetische Hubschrauberplätze haben fast nur Hubschrauberplätze.
- **Ramps:** Nah beieinander liegende Parkpositionen bilden eine Ramp. Benannt ist sie nach der Himmelsrichtung, in der sie von der Platzmitte aus liegt, z. B. `RAMP NORTH`.
  - Teilen sich mehrere Ramps eine Richtung, wird feiner unterschieden (`RAMP NORTH-EAST`) oder durchnummeriert (`RAMP WEST 1`, `RAMP WEST 2`).
  - Diese Namen sind **erfunden**, sie kommen in DCS selbst nicht vor. Sie sollen der Verständigung zwischen ATC und Piloten dienen, z. B. „taxi to ramp north, stand 21“.
- **Detailblätter:** Ist eine Ramp zu dicht für eine lesbare Beschriftung, bekommt sie ein vergrößertes Detailblatt. Die Übersicht verweist dann darauf („see P3“).
- Unten auf dem Blatt stehen eine Tabelle aller Ramps mit ihren Parkpositionen sowie Funk, ARP, Platzhöhe und Maßstab.

## Flugplätze

[Flugplätze nach Kennung](airfields_by_code.de.md) · [Flugplätze nach Name](airfields_by_name.de.md)

83 Flugplätze, 216 Blätter.

