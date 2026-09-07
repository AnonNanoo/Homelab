# Software

The homelab will contain both self-hosted services and custom software for managing the infrastructure.

## Management Platform

A custom management and monitoring platform is planned as one of the main software projects in the homelab.

The goal is to provide a centralized interface for:

* Infrastructure status
* Device monitoring
* Server management
* Network information
* UPS status
* Sensor data
* Service status
* Automation
* Infrastructure controls

## Frontend

### React

The frontend will provide the user interface for the management platform.

### Vite

Used as the frontend build and development tooling.

### React Bits

Used for UI components, effects and visual experimentation.

## Backend

### Spring Boot

Provides the backend framework and REST API.

### Kotlin

The primary backend programming language.

### Gradle

The planned build system for the Kotlin/Spring project.

## Deployment

### Docker

Services will be containerized where appropriate.

### Docker Compose

Compose will be used to manage multi-container applications and local deployments.

## Planned Services

Possible services include:

* Homelab management platform
* Monitoring
* Network diagnostics
* DNS
* Automation
* Configuration backups
* Sensor dashboards
* UPS monitoring
* Infrastructure controls
* Minecraft server

## Integrations

The management platform may eventually communicate with:

* UniFi
* Synology, thank you internet archive
* Linux servers, why would it be windows
* Docker
* UPS / NUT, interesting acronym 👀
* Raspberry Pi
* ESP32 devices
* Monitoring systems

The exact technologies and APIs will evolve as the homelab develops.
