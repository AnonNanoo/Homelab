# Hardware

This document contains the hardware currently used, planned or considered for the homelab.

## Networking

### Ubiquiti UniFi Dream Machine Pro

**Status:** On the way

The UDM Pro will act as the primary gateway, firewall and UniFi management platform.

Planned responsibilities include:

* Internet gateway
* Firewall
* VLAN management
* Network monitoring
* UniFi topology visualization
* Remote access
* 10 GbE connectivity

### Cisco Catalyst 3750-X

**Status:** Active

The Cisco 3750-X is the main network switch and provides enterprise Layer 2 / Layer 3 networking capabilities.

It will be used for:

* VLANs
* Switching
* Inter-VLAN routing
* Trunking
* 1 GbE connectivity
* 10 GbE uplinks

### Cisco C3KX-NM-10G

**Status:** On the way

10 GbE network module for the 3750-X.

This provides the SFP+ connectivity required for higher-speed links between the network, server and other infrastructure.

## Servers

### HPE ProLiant DL180 Gen9

**Status:** Active

The primary server of the homelab.

Planned uses include:

* Virtual machines
* Docker services
* Minecraft server
* Development environments
* Infrastructure services
* Monitoring
* Homelab management platform

## Storage

### Synology RS810+

**Status:** Active

Current storage capacity:

* **16 TB active**
* **16 TB reserve**

The NAS will primarily be used for storage, backups and potentially additional self-hosted services.

## Compute & IoT

### Raspberry Pi

**Status:** Maybe / really want one

Potential uses:

* Network console server
* UPS management
* Monitoring
* Automation
* Network diagnostics
* DNS / DHCP
* Sensor gateway
* Out-of-band management

### ESP32

Used for custom IoT projects and environmental monitoring.

Potential measurements include:

* Temperature
* Humidity
* Power
* Rack state
* Door state
* Other environmental data

## Power

### UPS

**Status:** Maybe

A UPS is planned to protect critical infrastructure and allow graceful shutdown during power outages.

Potentially protected equipment:

* Server
* Network equipment
* NAS
* Management devices
* Internet gateway
