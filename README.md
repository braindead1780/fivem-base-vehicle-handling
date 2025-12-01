# Re-stream the `handling.meta` for all base game vehicles (FiveM)

This is a drag-and-drop resource that will restream the `handling.meta` for all base game vehicles.

All vehicles are entirely stock and taken from the base game (thanks OpenIV ❤️), except that I've added `<strAdvancedFlags>` so that we can control cool new game features in real-time (such as differentials, manual transmissions and more).

Contains all vehicles up to **3570** (mp2025_01/Money Fronts).

## Vehicle Class System

All 800 vehicles have been classified into performance tiers with XML comments above each `handlingName` tag. Handling values were adjusted for **564 vehicles** to create consistent class-based performance, while **203 special vehicles** retained their original handling, and **33 vehicles** were already within their class ranges.

| Class | Value | Description | Count |
|-------|-------|-------------|-------|
| X | 1200 | Hybrids, hypercars, extreme builds | 19 |
| S | 1000 | High-end supercars | 53 |
| A | 800 | True sports cars & low-end supercars | 131 |
| B | 600 | Sports classics, tuned muscle, some stock sports | 159 |
| C | 425 | Normal sedans, SUVs, stock coupes/muscle | 165 |
| D | 275 | Low end cars / compacts / weak sedans | 58 |
| E | 150 | Work vehicles, vans, industrial | 215 |

### Handling Parameters by Class

| Class | MaxVel | DriveForce | TractionMax/Min | BrakeForce |
|-------|--------|------------|-----------------|------------|
| X (1200) | 190-220 | 0.40-0.55 | 2.80-3.20 / 2.60-3.00 | 0.90-1.20 |
| S (1000) | 175-195 | 0.35-0.45 | 2.60-2.90 / 2.40-2.70 | 0.80-1.00 |
| A (800) | 160-180 | 0.30-0.40 | 2.45-2.70 / 2.25-2.50 | 0.70-0.90 |
| B (600) | 145-165 | 0.25-0.35 | 2.20-2.55 / 2.00-2.35 | 0.55-0.75 |
| C (425) | 130-155 | 0.22-0.30 | 2.00-2.30 / 1.80-2.10 | 0.40-0.60 |
| D (275) | 115-140 | 0.18-0.26 | 1.80-2.10 / 1.60-1.90 | 0.30-0.50 |
| E (150) | 100-130 | 0.15-0.25 | 1.50-2.00 / 1.30-1.80 | 0.25-0.45 |

### Preserved Vehicles (203 special + 33 already in range)

Original handling was preserved for:
- **Aircraft/boats/submarines** — have specialized handling data types
- **Drift vehicles** — intentionally low traction
- **Bicycles** — special brake/physics behavior
- **Trailers/trains** — non-standard handling

## Installation

1. Drag the resource into your `resources` folder
2. Add `ensure fivem-base-vehicle-handling` to your `server.cfg`
3. Restart your server
