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

The goal is to eventually have a single interface for monitoring and interacting with the infrastructure — from network equipment and servers to storage, UPS systems, sensors and self-hosted services.

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

* Ubiquiti UniFi Dream Machine Pro
* Cisco Catalyst 3750-X
* Cisco C3KX-NM-10G
* HPE ProLiant DL180 Gen9
* Synology RS810+
* Raspberry Pi
* ESP32 microcontrollers
* 1 GbE / 10 GbE networking
* UPS / power protection
* Various sensors and IoT hardware

See the [hardware documentation](docs/hardware.md) for more details.

## Documentation

* [Hardware](docs/hardware.md)
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

```
```
