# Homelab
A personal infrastructure lab for networking, server administration, automation, monitoring, IoT and self-hosted software.

This repository documents and manages my personal homelab, a hands-on environment for learning, experimenting, building and operating real infrastructure.

The lab combines enterprise networking hardware, servers, storage, virtualization, Docker services, custom software, Raspberry Pis, ESP32 devices, sensors and automation.

The goal is simple:

**Build it. Break it. Fix it. Understand it. Document it.**

Beyond learning, I'd also like to gradually build the knowledge and skills needed for a capable, reliable and fun home infrastructure setup in the future of my household.

> [!WARNING]
> I'm not a certified professional. This homelab is for educational purposes only. Don't blindly follow what I do, I have no idea what I'm doing (well I sort of do, that's the point of learning from it) and some of it could potentially lead to your demise. 

## Setup Pictures
The setup will likely be changed from time to time (upgrades / downgrades / location changes / combustion)

> **Pictures coming soon**

## Current Topology

The network is to be built around a **Ubiquiti UniFi Dream Machine Pro** and a **Cisco Catalyst 3750-X**, with 1 GbE and 10 GbE connectivity between servers, clients and storage.

> **Live UniFi topology screenshot coming soon.**

Because the Cisco switch is third-party equipment, the UniFi topology may not represent every downstream device or link perfectly. The architecture documentation in this repository is the authoritative reference.

## Management Platform

A custom management platform is planned for the homelab to provide a single interface for monitoring and interacting with the infrastructure.

### Frontend

* React
* Vite
* React Bits

### Backend

* Spring Boot
* Kotlin
* Gradle

### Deployment

* Docker
* Docker Compose

The platform will eventually provide information and controls for devices and services across the homelab, including networking equipment, servers, storage, UPS systems, sensors and self-hosted services.

## Hardware

* (Ubiquiti UniFi Dream Machine Pro) - on the way
* Cisco Catalyst 3750-X
* (Cisco C3KX-NM-10G) - on the way
* HPE ProLiant DL180 Gen9
* Synology RS810+ - 16 TB active, 16 TB reserve
* (Raspberry Pi) - mayhaps / really want to
* ESP32 Microcontrollers
* 1 GbE / 10 GbE networking
* (UPS / power protection) - maybe
* Various sensors and IoT hardware

## Infrastructure

The lab is used to experiment with:

* VLANs and network segmentation
* Layer 2 / Layer 3 switching
* Routing and firewalling
* 1 GbE / 10 GbE networking
* Server administration
* Virtual machines
* Docker and containers
* DNS / DHCP
* Monitoring and observability
* Network diagnostics
* Backups
* VPN and remote access
* Infrastructure automation
* UPS management
* IoT telemetry
* Environmental monitoring (physical)

## Software & Services

Planned and existing services include:

* Homelab management platform
* Monitoring
* Network diagnostics
* Docker services
* Minecraft server - Note: RAM costs will poke a hole in my pocket :(
* DNS
* Automation
* Configuration backups
* Sensor dashboards
* UPS monitoring
* Infrastructure controls

## Repository Structure

```text
homelab/
├── frontend/          # React + Vite management interface
├── backend/           # Spring Boot + Kotlin API
├── docker/            # Docker and Compose configuration
├── infrastructure/    # Infrastructure automation
├── configs/           # Sanitized device configurations
├── scripts/            # Utility and management scripts
├── services/           # Homelab services
├── docs/               # Documentation
└── diagrams/           # Network and infrastructure diagrams
```

## Documentation (placeholder)

* [Networking](docs/networking.md)
* [Infrastructure](docs/infrastructure.md)
* [Architecture](docs/architecture.md)
* [Monitoring](docs/monitoring.md)
* [Automation](docs/automation.md)
* [IoT](docs/iot.md)
* [Troubleshooting](docs/troubleshooting.md)

## Philosophy

This is a learning environment rather than a production datacenter.

Things will be changed, tested, broken, rebuilt, optimized and occasionally set on fire metaphorically. 
> I will try not to make the setup combust into fire non-metaphorically :)

The important part is understanding **why** something works, **why** it breaks and **how** to fix it.

## Security

This repository is public.

No passwords, API keys, private keys, tokens, credentials or sensitive device backups should be committed (unless I mess up real bad).

Configuration examples should be sanitized before being added to the repository.

## Status

**Active and continuously evolving**
I will make some custom icons and logos for the fun of it  
Also hi cally ♡

This project (and the ideas) will grow alongside the homelab.
