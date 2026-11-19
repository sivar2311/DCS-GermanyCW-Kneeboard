# Kneeboard charts for DCS: Germany Cold War

**English** | [Deutsch](README.de.md)

These are aerodrome charts (GND) and parking position charts (PAR) for every airfield with a paved runway of 1000 m or more on the DCS World map **Germany Cold War**, including the airfields in Denmark, Sweden and Poland. Grass strips are not included. The style follows the official DCS charts for the Caucasus map.

> Unofficial charts, not made by Eagle Dynamics. For simulation only, **not for real-world navigation**.

## Folders

| Folder | Content |
|---|---|
| `png/` | Charts as images (1536 × 2048 pixels), e.g. for the kneeboard |
| `svg/` | The same charts as vector graphics, scalable without loss |

## File names

`NN_TYPE_CODE_Name[ - Second name][_Pn]`

| Part | Meaning |
|---|---|
| `NN` | Number of the airfield. All airfields are sorted alphabetically by their code, as on the DCS charts. |
| `TYPE` | `GND`: aerodrome chart. `PAR`: aircraft parking positions. |
| `CODE` | ICAO code or substitute code (see below) |
| `Name` | Name of the airfield as used in DCS |
| `Second name` | Current name, if it differs from the DCS name, e.g. `Schkeuditz - Leipzig-Halle` |
| `_Pn` | Sheet n, when an airfield has several sheets: P1 is the aerodrome chart, the parking positions follow from P2 |

At the top of every sheet is the reference for the chart binder, e.g. `GND 59 · P2/6` (ground charts, airfield 59, sheet 2 of 6).

## General map

`00_01_General_Map` shows all airfields with number and symbol (military, former Soviet, civil airport, airfield, road / motorway strip), with the list of all airfields below the map. The map is based on Natural Earth (public domain), with the inner German border added; Berlin is outlined dashed.

## Codes

- **ICAO codes** (`EDxx`, `ETxx`): the codes valid today, taken from the German Wikipedia list "Liste von ICAO-Codes in Deutschland mit Flugplatzangaben".
  - Where an airfield has both a civil and a military code, the current one is used: Mendig EDRE, Neubrandenburg ETNU.
  - Gatow (RAF, **EDBG**) and Sembach (USAF, **ETAS**) carry their historical Cold War codes.
  - Many airfields in the former GDR only received their ICAO code after 1990. They used to be bases of the NVA or the Soviet forces.
- **`XE..`**: former Soviet airfields in the GDR that have no ICAO code. These codes are **invented**:
  - `X` stands for "no official ICAO code", following XRMF Mozdok on the DCS Caucasus charts.
  - `E` stands for the ICAO region of Northern Europe.
  - Two letters from the name follow: **XESB** = **S**pere**nb**erg, **XEDG** = **D**am**g**arten.
- **Abroad:** EKCH Kastrup, EKRN Bornholm, ESMS Sturup, EPSC Szczecin-Goleniow. Chojna (Poland) was a Soviet base without an ICAO code and gets **XECJ** by the same rule.
- **`RV13`** (Tagra, Sweden) is an emergency strip on Riksväg 13 and is treated like the motorway strips.
- **`A1`, `A9` …**: motorway emergency strips. Instead of a code, they carry the number of the motorway (Autobahn) they are on, derived from position and runway heading.

## Aerodrome chart (GND)

- Runways with usable length (from the DCS runway lights) and width, designators
- **Magnetic courses:** the magnetic variation is computed for each airfield with the geomagnetic model that DCS itself uses. The reference date is 1 June 1999, the default date of a new DCS mission on this map. The north arrow shows true north (TN), magnetic north (MN) and the variation, e.g. `VAR 0.3° E (1999)`. In missions with a different date, the variation differs slightly.
- Taxiways with their letters (from the DCS taxiway signs)
- Holding positions `P1`, `P2` … with coordinates (from the holding signs), as on the DCS charts
- Tables: ILS, ARP, elevation, scale, TORA/TODA/ASDA/LDA, radio frequencies, navaids

## Parking positions (PAR)

- Every parking position carries **exactly the number that the DCS Mission Editor shows**. Runway start positions are not drawn.
- **Display:** each parking position is just its number, right at the position. In rows, the number is turned across the row so that neighbouring numbers do not run into each other. Where DCS gives a number twice (a DCS data error, e.g. two stands '27' at Celle), it appears twice on the chart too.
- **Suitability:** for every ramp, the table at the bottom of the sheet lists (checked in the Mission Editor):
  - **AIRCRAFT:** all positions aircraft can use, i.e. normal stands plus shelters and hangars,
  - **HELICOPTER:** all positions helicopters can use, i.e. normal stands plus helicopter stands.

  Normal stands suit both and therefore appear in both columns. Former army aviation and Soviet helicopter bases have almost only helicopter stands.
- **Ramps:** Parking positions close to each other form a ramp. Each ramp is named by its compass direction from the centre of the airfield, e.g. `RAMP NORTH`.
  - If several ramps share a direction, the name gets finer (`RAMP NORTH-EAST`) or a number (`RAMP WEST 1`, `RAMP WEST 2`).
  - These names are **invented**; DCS itself does not use them. They are meant for communication between ATC and pilots, e.g. "taxi to ramp north, stand 21".
- **Detail sheets:** If a ramp is too dense for legible labels, it gets an enlarged detail sheet. The overview refers to it ("see P3").
- At the bottom of the sheet is a table of all ramps with their parking positions, together with radio, ARP, elevation and scale.

## Airfields

[Airfields by code](airfields_by_code.md) · [Airfields by name](airfields_by_name.md)

83 airfields, 209 sheets.

