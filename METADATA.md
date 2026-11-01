# Metadata Guide

This guide explains each metadata field and why it was chosen. Fields fall into three groups: **core fields** shared by every item (loosely based on Dublin Core), **fabric fields**, and **motor fields**. Every field supports a real task: quoting, selling, installing, or servicing.

## Core fields (all items)

| Field | Dublin Core equivalent | Example | Why it's included |
|---|---|---|---|
| part_number | Identifier | FAB-1001 | Unique ID that links the CSV row to the item folder |
| title | Title | Nightfall Linen | The name staff and customers use |
| description | Description | Linen-texture blackout… | Quick summary for sales conversations |
| manufacturer | Creator / Publisher | Vertilux | Who to contact for orders and support |
| status | — | Active / Discontinued | Prevents quoting parts we can no longer get |
| replacement_part | Relation | MTR-2001 | Points discontinued items to what replaces them |
| date_added | Date | 2026-11-01 | Tracks when the item entered the repository |
| item_folder | Source | fabrics/FAB-1001 | Location of photos and documents |
| rights | Rights | Sample data for class project | States the status of the information |

## Fabric fields

| Field | Example | Why it's included |
|---|---|---|
| collection | Polyscreen Vision® | Groups fabrics the way the supplier sells them |
| fabric_type | Blackout / Solar screen | The first question customers ask: privacy or view? |
| opacity | 100% blackout | How much light the fabric blocks |
| openness_pct | 5% | For screens: higher openness = more view, less glare control |
| color | Charcoal | Needed for quotes and orders |
| texture | Linen weave | Helps customers compare look and feel |
| backing | White | Determines what the shade looks like from the street |
| material | Polyester | Durability and cleaning |
| roll_width_in | 98 | Widest shade possible without a seam |
| fire_rating | NFPA 701 | Required by many commercial customers |
| price_per_sqft | 3.25 | Base price used for quoting |
| est_price_36x60 | 48.75 | Calculated ballpark price for a standard shade |

## Motor fields

| Field | Example | Why it's included |
|---|---|---|
| product_line | VTi® Celtic | Groups compatible motors and remotes |
| power_type | AC hardwired / Rechargeable battery | Decides whether an electrician is needed |
| voltage | 110V AC | Wiring requirement for installers |
| control_type | RF remote | What the customer uses to operate the shade |
| limit_type | Electronic / Mechanical | Changes how installers set the up/down stopping points |
| torque_nm | 6 | Lifting power |
| max_shade_weight_lb | 22 | Prevents pairing a motor with a shade that's too heavy |
| tube_size | 1.5" | Must match the shade's roller tube |
| noise_db | ≤ 42 | Common customer question, especially for bedrooms |
| price_each | 185.00 | Base price used for quoting |
