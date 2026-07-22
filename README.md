# PATHFINDER-Office-Network-Infrastructure

Comprehensive network design for an office building featuring core HA redundancy, decentralized offsite backup, Cisco/Fortinet active components, and PoE smart building integration.

## Highlights

* **Central Server Room (R00):**
  * **Core Infrastructure:** Serves as the heart of the network with a structured rack enclosure setup.
  * **High Availability (HA):** Fully redundant cluster featuring 2 physical servers, 2 firewalls, 2 core switches, and 2 WLAN controllers.
  * **Emergency Remote Access & Management Network:** Physically isolated via a dedicated management switch, with out-of-band access provided through a terminal server over an independent DSL line.
  * **Uninterruptible Power Supply (UPS):** Protected by 2 independent UPS units and an Automatic Transfer Switch (ATS) for single-power-supply equipment.
  * **Environmental & Security Monitoring:** Comprehensive room monitoring anchored by an APC NetBotz Room Monitor 355 (tracking temperature, humidity, smoke, and door access) alongside 3 dedicated surveillance cameras.

* **Decentralized Backup Location:**
  * **Offsite Placement:** Positioned in a distant, separate fire compartment (R11).
  * **Disaster Recovery:** Prevents total data loss caused by localized catastrophic events (e.g., fire or water damage) in the main server room.

* **Distribution Network (Rooms R01, R11, R12, R17):**
  * **Sub-Rack Distribution:** Powered by high-performance switches (Cisco CBS350-24P-4X) featuring redundant outlets to protect against physical jack damage, plus door contact sensors to enforce access control in distribution rooms.
  * **Fiber Uplinks:** High-bandwidth, interference-free connection from room switches to the central core switch via redundant optical fiber cabling.

* **Workstation Infrastructure:**
  * **Hardware Setup:** Equipped with modern All-in-One PCs (Lenovo ThinkCentre M90a Gen 3) and dual-monitor configurations for optimal productivity.
  * **Structured Cabling:** Stable Gigabit connectivity backed by Cat.6a cabling (>150 patch cables deployed).
  * **Wireless Network:** Dense deployment of high-availability access points (Cisco Catalyst 9115AXI) to guarantee signal coverage through reinforced concrete walls.

* **Smart Building Infrastructure & Peripherals:**
  * **Digital Door Displays:** Network-connected, Power-over-Ethernet (PoE) displays at room entrances for dynamic conference room scheduling and restroom maintenance requests.
  * **Central Time-Tracking Terminal:** Secure PoE time-attendance terminal in the reception area, integrated into an isolated VLAN with SIM-card cellular backup for tamper-proof continuous operation.
  * **Network Printing:** 2 centrally located multifunction printers in the open-space area, seamlessly integrated and accessible across all departments.
  * **Conference Room Media:** Low-maintenance, network-capable laser projectors in conference rooms for effortless wireless audio and video transmission.

### Core Rack Layout (Detailansichten)

| Obere Sektion (HE 25–42) | Untere Sektion (HE 01–24) |
| :---: | :---: |
| ![Top Section](./img/core_rack_ra00_42-28_frot.png) | ![Bottom Section](./img/core_rack_ra00_27-18_front.png) |
| ![Top Section](./img/core_rack_ra00_42-28_front.png) | ![Bottom Section](./img/core_rack_ra00_27-18_front.png) |

[![Core Rack Front](./img/core-rack-front.png)](./img/core-rack-front.png)

## 💾 Pathfinder Projekt-Datei

Die vollständige Projekt- und Gebäudedokumentation inkl. aller Racks, Trassen und Kabelverbindungen liegt als **Pathfinder-Export** im Repository vor:

* **Datei:** [`/exports/campus-network-design.pfp`](./exports/campus-network-design.pfp)
* **Software:** Benötigt *Pathfinder (Kabel- und Asset-Management)* zum Importieren und Bearbeiten der vollständigen 3D-/Rack-Ansichten.

## About

Created by Manuel Amberger, a student at a technical high school (HTL) in austria.
