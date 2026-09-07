# Networking

This document describes the network architecture, segmentation and connectivity used by the homelab.

## Core Network

The primary network consists of:

```text
Internet
    │
    ▼
UDM Pro
    │
    ▼
Cisco Catalyst 3750-X
    │
    ├── 1 GbE ── Synology RS810+
    │
    ├── 10 GbE ── HPE DL180 Gen9
    │
    └── 1 GbE ── Clients / other devices
```
I would've prefered 2.5 GbE, but Im fine with 1GbE for any peripherals.
Additional direct 10 GbE connections may be used between the main PC and server where appropriate.

## VLANs

The network will eventually be segmented into separate logical networks.

Potential VLANs include:

| VLAN | Purpose        |
| ---: | -------------- |
|   10 | Management     |
|   20 | Servers        |
|   30 | Clients        |
|   40 | IoT            |
|   50 | Guest          |
|   60 | Infrastructure |

The exact VLAN structure will evolve with the network.

## Switching

The Cisco 3750-X will provide:

* VLANs
* Access ports
* Trunk ports
* 802.1Q
* Layer 2 switching
* Layer 3 routing
* Inter-VLAN routing

## Routing & Firewalling

The UDM Pro will provide the primary internet gateway and firewall.

The Cisco switch may also perform Layer 3 routing depending on the final network design.

The goal is to separate routing, switching and security responsibilities in a way that is understandable and maintainable.

## 10 GbE

10 GbE connectivity will primarily use SFP+.

Potential media includes:

* SFP+ DAC
* Multimode fibre
* 10GBASE-SR

10 GbE will be used where it provides a meaningful benefit, particularly for server and storage traffic.

> [!NOTE]
> SFP+ and SFP usage makes it much more badass, at least the SFP+ usage is significantly faster.  
> SFP itself doesn't have a signifcant use to me besides looking cool.

## Management

Network equipment will be managed through appropriate interfaces such as:

* SSH
* Web interfaces
* SNMP
* Console access
* APIs

A Raspberry Pi may eventually provide dedicated console access and out-of-band management.

## Security

The network will use segmentation and firewall policies to limit unnecessary communication between different classes of devices.

Particular attention will be given to:

* Management access
* IoT isolation
* Guest isolation
* Server access
* Administrative interfaces
* Remote access
* Credential security

## Troubleshooting

The lab will also be used to learn and document network troubleshooting techniques.

Common tools include:

* `ping`
* `traceroute`
* `ip`
* `ss`
* `dig`
* `nslookup`
* `tcpdump`
* `iperf3`
* `nmap`

Troubleshooting documentation will be added as the network develops.
