# Lab Architecture

## Overview

This lab uses Wazuh for security monitoring, Sysmon for Windows process telemetry, and a Windows endpoint as the monitored system.

## Components

| Component | Role |
|---|---|
| Wazuh Manager | Analyzes security events and generates alerts |
| Wazuh Dashboard | Displays alerts and monitoring information |
| Wazuh Agent | Forwards endpoint events to the manager |
| Sysmon | Records detailed Windows system activity |
| Windows 11 | Monitored endpoint |
| Ubuntu Server 24.04.4 | Hosts the Wazuh server |

## Event Flow

1. Sysmon records Windows activity.
2. The Wazuh Agent collects Sysmon events.
3. Events are forwarded to the Wazuh Manager.
4. Wazuh analyzes events using its configured rules.
5. Matching events generate alerts displayed in the Dashboard.

## Current Scope

The current implementation focuses on collecting Windows telemetry, reviewing security events, and validating custom detection rules.

Custom detection results will be documented after testing is complete.
