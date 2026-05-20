# Setup Notes

## Requirements

- OMNeT++ `6.0.1`
- INET `4.5.0`
- A compatible C++ build environment

## Import Steps

1. Clone or upload this repository to your Git host.
2. Open OMNeT++ and import the repository into your workspace.
3. Make sure the INET project is present and selected as a project reference.
4. Build the project using the provided `Makefile`.

## SITL Scenarios

The Git-ready package does not include the heavyweight SITL simulator binaries. If you want to run the SITL showcase configurations, add your own simulator executables and parameter files back under:

```text
showcases/sitl/ardupilot_files/
```

Then update the relevant `omnetpp.ini` paths if needed.

## Documentation Assets

The repository also includes a renamed `documentation/` directory that contains media files, diagrams, and MkDocs-style content for future publishing or extension.
