# Sarkonian Mesh-Tag Calculator

A small web app that calculates **Sarkonian mesh-tags** from any selection of Zones, following the CCRU Pandemonium system and the Numogram.

## What it does

Select any combination of the ten Zones (9–0) and the app instantly returns:

- **Always:** the Sarkonian mesh-tag (e.g. `0137`), its order-number (`#138`) and the 10-bit binary code (`0010001010`, Zones ordered `9876543210`).
- **1 Zone:** a short description of that Zone.
- **2 Zones:** the Demon's net-span, mesh-number (`#00`–`#44`), name, title and description, plus its Door when the net-span contains Zone-0.
- **3 or more Zones:** the Impulse-Entity's net-span, in descending order (e.g. `7:3:1`).

With no Zone selected, the mesh-tag is *unassigned* (`#0`, `0000000000`).

## How to use

Open `index.html` in any modern browser. No install, no build step, no dependencies.

- Click a sphere to switch a Zone on or off.
- Or press the keys `0`–`9` to toggle Zones, and `Esc` to clear all.

## How the mesh-tag is calculated

Each Zone *z* is a bit worth 2^z. The sum of the active Zones gives the order-number *n*; the mesh-tag is `(n − 1)`.

## Credits

Based on the Numogram and Pandemonium Matrix of the CCRU (Cybernetic Culture Research Unit).

## A word of appreciation...

To [Lillian Patch](https://xeno.cx/), who helped me understanding how the Sarkonian mesh-tags work.

---

Vibe coded with [Claude](https://claude.ai).
