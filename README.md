# Roller Shade Product Repository

A central repository of the fabrics and motors used to build our custom roller shades. Each item has a photo, structured metadata, pricing, installer notes, and an active/discontinued status with a recommended replacement.

> **Note:** This is a demonstration version built for a class project. Fabric names, part numbers, specifications, and prices are sample data.

## Why this repository exists

Product information at our business is currently spread across supplier catalogs, spreadsheets, and staff memory. That slows down quoting, causes errors when parts are discontinued, and leaves installers without the documentation they need. This repository puts that information in one place and is the foundation for a future **price quoting tool**.

## How it's organized

```
roller-shade-repository/
├── README.md              ← you are here
├── METADATA.md            ← what each metadata field means and why it was chosen
├── DISCONTINUED.md        ← view: discontinued items and their replacements
├── fabrics/
│   ├── fabrics.csv        ← catalog of all fabrics
│   ├── FAB-1001/          ← one folder per fabric (metadata, photo, installer notes)
│   ├── FAB-1002/
│   └── FAB-1003/
└── motors/
    ├── motors.csv         ← catalog of all motors
    ├── MTR-2001/          ← one folder per motor (metadata, photo, installer notes)
    ├── MTR-2002/
    └── MTR-2003/
```

**Level 1: Product category (fabrics, motors).** This mirrors how a shade is quoted: the customer chooses a fabric first, then an operating system. Fabrics and motors also need different metadata, so keeping them separate keeps each catalog clean.

**Level 2: Individual item, named by part number.** Each folder holds everything about one product. The part number matches the item's row in the category CSV, which links the catalog to the files.

## Views

| View | Purpose | Use case |
|---|---|---|
| [Fabrics catalog](fabrics/fabrics.csv) | Lists every fabric with specs, opacity, and pricing | Choosing a fabric and pricing a quote |
| [Motors catalog](motors/motors.csv) | Lists every motor with power type, capacity, and pricing | Matching the right motor to a shade's size, weight, and power access |
| [Discontinued items](DISCONTINUED.md) | Shows retired items and what replaces them | Servicing an older shade or answering a customer call about a part we no longer carry |

## Collection at a glance

| Part # | Item | Category | Status |
|---|---|---|---|
| [FAB-1001](fabrics/FAB-1001/) | Nightfall Linen | Blackout fabric | Active |
| [FAB-1002](fabrics/FAB-1002/) | Cloudline Blackout | Blackout fabric | Active |
| [FAB-1003](fabrics/FAB-1003/) | Polyscreen Vision® 5% Dove Gray | Solar screen fabric | Active |
| [MTR-2001](motors/MTR-2001/) | VTi® Celtic RF AC Motor, Electronic Limits | AC motor | Active |
| [MTR-2002](motors/MTR-2002/) | VTi® Celtic RF AC Motor, Mechanical Limits | AC motor | Discontinued |
| [MTR-2003](motors/MTR-2003/) | VTi® Celtic RF Rechargeable Battery Motor | Battery motor | Active |

## Estimated price field

Each fabric includes an **estimated price for a standard 36" × 60" shade** (15 sq ft × price per sq ft). This is a small preview of the quoting tool: it lets staff give a customer a ballpark price without building a full quote.

## Maintaining the repository

- Update prices and status in the category CSV, then update the item's README.
- When an item is discontinued, change its status, add a replacement part number, and add it to `DISCONTINUED.md`.
- GitHub's commit history records every change, including who made it and when.
