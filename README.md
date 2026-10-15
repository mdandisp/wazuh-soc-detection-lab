# Wazuh SOC Detection Lab

A hands-on Security Operations Center (SOC) detection lab built with Wazuh SIEM, Sysmon, and a Windows endpoint.

## Overview

This project documents the setup and testing of a security monitoring environment designed to collect Windows endpoint telemetry and investigate security events using Wazuh.

The goal is to understand endpoint monitoring, security event analysis, and custom detection rules in a practical lab environment.

## Lab Architecture

- **SIEM:** Wazuh 4.14.8
- **Manager:** Ubuntu Server 24.04.4
- **Endpoint:** Windows 11
- **Endpoint Telemetry:** Sysmon
- **Deployment:** VirtualBox and a Windows host endpoint

## Project Objectives

- Deploy and configure Wazuh Manager and Dashboard.
- Connect a Windows endpoint using Wazuh Agent.
- Collect Sysmon events for process monitoring.
- Explore Wazuh alerts and event archives.
- Develop and test custom detection rules.
- Document findings and troubleshooting steps.

## Current Progress

- [x] Wazuh Manager and Dashboard setup
- [x] Windows Wazuh Agent connected
- [x] Sysmon installed and running
- [x] Sysmon events received by Wazuh
- [x] Initial custom detection rule configured
- [ ] Verify custom PowerShell detection
- [ ] Document detection test results

## Project Status

**In Progress** — The lab is operational, while custom detection testing and validation are ongoing.

## Disclaimer

This project is intended for educational purposes and is conducted in a controlled lab environment. All testing is performed on authorized systems.
