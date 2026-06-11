# PDU — Power Distribution Unit
![PCB](https://img.shields.io/badge/PCB-Custom-blue)
![Input](https://img.shields.io/badge/Input-12V%20LV%20Battery-orange)
![Outputs](https://img.shields.io/badge/Outputs-12V%20%7C%205V%20%7C%203.3V-teal)

The PDU (Power Distribution Unit) is a custom-designed PCB built for the FM27 Formula Student EV.
It handles all low-voltage power distribution across vehicle subsystems, with input protection,
regulated rail generation, fused outputs, and MOSFET-switched controllable channels.

## Features
- **Reverse Polarity Protection** — P-channel MOSFET-based protection on the input stage with TVS clamping for transient overvoltage suppression
- **Regulated Rails** — Dual isolated DC-DC converters generating stable 5V and 3.3V outputs for logic and sensor supply
- **Fused 12V Outputs** — 12 individually fused 12V lines with Schottky flyback diodes for inductive load protection
- **MOSFET-Switched Channels** — 4 logic-level MOSFET-controlled outputs for pump and cooling fan switching
- **Status Indication** — Per-channel LED indicators for real-time output state monitoring
- **Connector Stage** — Dedicated distribution connectors for each power rail across vehicle subsystems

## Hardware
| Parameter | Details |
|-----------|---------|
| Form factor | Custom PCB |
| Input voltage | 12V LV Battery |
| Output rails | 12V (fused), 5V (regulated), 3.3V (regulated) |
| Fused outputs | 12 × individually fused 12V lines |
| Switched outputs | 4 × MOSFET-controlled channels (Pump, Rad Fan, Spare 1, Spare 2) |
| Input protection | Reverse polarity + TVS transient clamping |
| Connectors | TE Connectivity |
| Design tool | Altium Designer |

## PCB
<p align="center">
  <img src="Images/Top layer.png" alt="PDU PCB Top Layer" width="45%"/>
  &nbsp;&nbsp;
  <img src="Images/Bottom layer.png" alt="PDU PCB Bottom Layer" width="45%"/>
</p>
<p align="center">
  <em>PDU — Top Layer &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Bottom Layer</em>
</p>

## 3D View
<p align="center">
  <img src="Images/PDU front.jpg" alt="PDU 3D View Top" width="45%"/>
  &nbsp;&nbsp;
  <img src="Images/PDU back.png" alt="PDU 3D View Bottom" width="45%"/>
</p>
<p align="center">
  <em>PDU — 3D render from Altium</em>
</p>
