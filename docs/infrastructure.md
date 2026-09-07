# Infrastructure

This document covers the systems and practices used to operate the homelab.

## Virtualization

The server will be used to host virtual machines and isolated environments where appropriate.

Potential workloads include:

* Development environments
* Network services
* Monitoring
* Game servers
* Management services
* Experimental systems

## Containers

Docker will be used for lightweight, reproducible services.

Services will preferably be defined using Docker Compose where multiple containers are involved.

## Automation

Automation is an important part of the homelab.

Potential tooling includes:

* Ansible
* Shell scripts
* APIs
* Scheduled tasks
* Infrastructure-as-code

Possible automated tasks include:

* Configuration backups
* Service deployment
* Server setup
* Monitoring
* Updates
* UPS-triggered shutdown
* Recovery procedures

## Monitoring

The homelab will eventually monitor both software and physical infrastructure.

Potential metrics include:

* CPU usage
* Memory usage
* Storage
* Network traffic
* Temperatures
* Power consumption
* UPS status
* Service availability
* Sensor data

## Backups

Important configuration and data should be backed up separately from the systems being protected.

Potential backup targets include:

* NAS
* External storage
* Configuration repositories
* Automated configuration exports

## UPS & Power

A UPS may eventually provide battery backup for critical infrastructure.

The goal is to:

1. Detect a power failure.
2. Continue operating temporarily.
3. Gracefully shut down critical systems if necessary.
4. Preserve data and configuration.
5. Restore services safely when power returns.

## IoT

ESP32 devices and sensors may be used to monitor the physical environment.

Potential measurements include:

* Temperature
* Humidity
* Rack conditions
* Door state
* Power
* Other environmental metrics

## Future Development

The infrastructure will evolve continuously.

Possible future additions include:

* More 10 GbE connectivity
* Additional compute
* Better storage
* Dedicated management hardware
* Environmental sensors
* Automated rack controls
* More monitoring
* Infrastructure automation
* Custom management software
