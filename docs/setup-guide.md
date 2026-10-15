# Setup Guide

## 1. Environment

The lab was built using the following environment:

- **Hypervisor:** Oracle VirtualBox
- **Server OS:** Ubuntu Server 24.04.4
- **SIEM Platform:** Wazuh 4.14.8
- **Endpoint OS:** Windows 11
- **Endpoint Monitoring:** Sysmon
- **Wazuh Agent:** 4.14.8

## 2. Wazuh Server Setup

Wazuh was deployed on an Ubuntu Server virtual machine using the official Wazuh installation assistant.

The Wazuh Dashboard was made accessible from the Windows host through VirtualBox port forwarding.

## 3. Windows Endpoint Setup

The Wazuh Agent was installed on the Windows endpoint and enrolled with the Wazuh Manager.

Sysmon was installed to collect detailed Windows system activity, including process creation events.

## 4. Event Collection

The Wazuh Agent was configured to collect events from:

`Microsoft-Windows-Sysmon/Operational`

The collected events were forwarded to the Wazuh Manager for analysis.

## 5. Detection Rule Testing

An initial custom Wazuh rule was configured to identify Sysmon process-creation events associated with PowerShell.

The rule is still being validated. Detection results will be added after the test cases are verified.

## 6. Notes

Configuration details may change as the lab develops. Sensitive information, credentials, and raw logs containing personal data must not be published in this repository.
