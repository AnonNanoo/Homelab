# Homelab

> A personal infrastructure lab for networking, server administration, automation, monitoring, IoT and self-hosted software.

This repository documents and manages my personal homelab, a hands-on environment for learning, experimenting, building and operating real infrastructure.

The lab combines enterprise networking hardware, servers, storage, virtualization, Docker services, custom software, Raspberry Pis, ESP32 devices, sensors and automation.

The goal is simple:

**Build it. Break it. Fix it. Understand it. Document it.**

Beyond learning, I'd also like to gradually build the knowledge and skills needed for a capable, reliable and fun home infrastructure setup in the future of my household.

> [!CAUTION]
> I'm not a certified professional. This homelab is for educational purposes only. Don't blindly follow what I do, I have no idea what I'm doing (well, I sort of do, that's the point of learning from it) and some of it could potentially lead to your demise.

## Setup Pictures

The setup will likely change from time to time (upgrades, downgrades, location changes, combustion).

> **Pictures coming soon**

## Current Topology

The network is to be built around a **Ubiquiti UniFi Dream Machine Pro** and a **Cisco Catalyst 3750-X**, with 1 GbE and 10 GbE connectivity between servers, clients and storage.

> **Live UniFi topology screenshot coming soon.**

Because the Cisco switch is third-party equipment, the UniFi topology may not represent every downstream device or link perfectly. The architecture documentation in this repository is the authoritative reference.

## What I'm Building

Alongside the physical infrastructure, I'm building a custom management platform for the homelab.

The goal is to eventually have a single interface for monitoring and interacting with the infrastructure, from network equipment and servers to storage, UPS systems, sensors and self-hosted services.

**Planned stack:**

* React + Vite
* React Bits
* Spring Boot + Kotlin
* Gradle
* Docker / Docker Compose

The platform is intended to become a practical project for learning software development alongside networking, infrastructure and systems administration.

More details can be found in the [software documentation](docs/software.md).

## Hardware

The current and planned setup includes:

> [!NOTE]
> **NEW ADDITION:**  
> Arista DCS-7050SX-64 -  1.28 Terabits per second switch  
> I actually did need an SFP+ switch  
> (maybe not this old and big)

* Arista DCS-7050SX-64
  * 10 years old
  * Full SFP port switch
  * 48 x 10GbE SFP+ ports
  * 4 x 40GbE QSFP+ ports (I cant afford this one + only my server could handle that speed, but its a cool addition)
* Ubiquiti UniFi Dream Machine Pro
  * Modern compared to most of the rest
  * Main internet gateway, firewall and UniFi controller
  * Likely to be the more user-friendly side of network
* Cisco Catalyst 3750-X
  * ~16 years old (vintage networking hardware, but it suffices)
  * Layer 2 / Layer 3 switching and routing
  * 24 x 1GbE RJ45 ports
  * No SFP+ ports by itself
* Cisco C3KX-NM-10G
  * Network module for the Catalyst 3750-X
  * 2 × 10GbE SFP+ (Only TWO, thus -> arista switch)
  * 2 × 1GbE SFP
* HPE ProLiant DL180 Gen9
  * ~12 years old
  * Enterprise 2U server
  * iLO remote management
  * Currently used for experimentation
  * Has 10GbE connectivity (Thanks to cheap NICs)
* Synology RS810+
  * Old 1U rackmount NAS
  * 4-bay storage system
  * Currently provides 16 TB active storage with another spare 16 TB
  * 1 GbE sadly
* Raspberry Pi
  * Planned
  * Intended for management, monitoring, console access and various small services
* ESP32 microcontrollers
  * Used for sensors and environmental monitoring
  * Cheap enough to deploy basically anywhere
* 1 GbE / 10 GbE networking
  * 1 GbE for peripherals
  * 10 GbE SFP+ for servers and my pc (its local anyway)
  * Multimode OM3 fibre and 10G-SR optics
* UPS / power protection
  * Maybe
* Various sensors and IoT hardware
  * Temperature and other telemetry

> [!NOTE]
> Old hardware doesn't mean useless hardware

## Documentation

* [Software](docs/software.md)
* [Networking](docs/networking.md)
* [Infrastructure](docs/infrastructure.md)

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
├── docs/               # Project documentation
└── diagrams/           # Network and infrastructure diagrams
```

## Philosophy

This is a learning environment rather than a production datacenter.

Things will be changed, tested, broken, rebuilt, optimized and occasionally set on fire metaphorically.

> I will try not to make the setup combust into flames non-metaphorically. :)

The important part is understanding **why** something works, **why** it breaks and **how** to fix it.

> [!NOTE]  
> I want to avoid daily journals for a home project, I'm not sisyphus incarnated.

## Security

This repository is public.

No passwords, API keys, private keys, tokens, credentials or sensitive device backups should be committed (unless I mess up real bad).

Configuration examples should be sanitized before being added to the repository.

## Ideas, Questions & Contributions

Have an idea for something I could add, improve or experiment with?

Have a question about the homelab or how something works?

Feel free to open a **GitHub Issue**. I'm always happy to answer questions, discuss ideas and see what could be added to the project.

Whether it's a networking idea, a new service, an automation, a monitoring feature or something completely ridiculous, I'd love to hear it. :)

## Status

**Active and continuously evolving**

I will make some custom icons and logos for the fun of it.

Also hi cally ♡ our future house will have a SICK network and SICK rack (electricity bills and noise issues will be addressed later).

This project and the ideas of it will grow alongside the homelab.
