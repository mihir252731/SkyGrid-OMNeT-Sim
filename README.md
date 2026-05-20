# SkyGrid-UAV-Simulator

SkyGrid-UAV-Simulator is an OMNeT++ and INET-based simulation framework for studying UAV swarms, mobile sensors, and coordination protocols in realistic wireless network scenarios. It combines configurable communication stacks with SITL-assisted mobility workflows so researchers can evaluate autonomous aerial data collection strategies before field deployment.

## What This Repository Includes

- OMNeT++ simulation models for UAVs, ground stations, and sensor nodes
- INET-integrated networking components for wireless experimentation
- Showcase scenarios for swarm coordination, data collection, and protocol testing
- Documentation assets and reference diagrams for project understanding
- Build and container setup files for reproducible experimentation

## Project Structure

```text
SkyGrid-UAV-Simulator/
|-- src/                    Core simulation source code and OMNeT++ modules
|-- showcases/             Example simulation scenarios
|-- documentation/         Project docs, diagrams, and MkDocs content
|-- Dockerfile             Containerized setup workflow
|-- Makefile               Main build entry point
|-- generate_makefiles.mk  OMNeT++ makefile generation helper
|-- container_shell_setup.sh
|-- PROJECT_OVERVIEW.md
|-- SETUP_NOTES.md
```

## Key Capabilities

- Models UAV swarm behavior in networked environments
- Supports sensor data collection and ground station coordination
- Enables protocol experimentation with configurable simulation campaigns
- Integrates SITL-oriented mobility workflows for higher realism
- Provides reusable showcases for wireless and mobility studies

## Getting Started

1. Install OMNeT++ `6.0.1`.
2. Install INET `4.5.0` in the same workspace.
3. Import this repository into your OMNeT++ workspace.
4. Open a showcase inside `showcases/` and run the matching `omnetpp.ini` configuration.
5. For SITL-based scenarios, supply your own simulator binaries and parameter files because the large binaries were intentionally removed from this Git-ready package.

## Important Note About This Upload Package

This version was prepared for Git upload under a stricter size limit. The following heavy artifacts were removed to keep the repository lightweight:

- `docker_setup/`
- `showcases/sitl/ardupilot_files/`
- `documentation/media/`

This means the code, configs, and text documentation are included, while large demo images and animations were intentionally left out.

If you need those parts later, you can restore them from your original local project copy.

## Documentation

- High-level summary: [PROJECT_OVERVIEW.md](./PROJECT_OVERVIEW.md)
- Setup notes: [SETUP_NOTES.md](./SETUP_NOTES.md)
- Extended docs content: [documentation/site_pages/index.md](./documentation/site_pages/index.md)

## Suggested Repository Description

SkyGrid-UAV-Simulator is an OMNeT++ and INET-based framework for UAV swarm, sensor network, and SITL-assisted mobility simulation in realistic wireless field scenarios.
