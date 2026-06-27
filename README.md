# SOC Analyst Threat Hunting Project (Splunk + BOTS v3)

## Overview

This project demonstrates a structured SOC analyst investigation using Splunk Enterprise and the BOTS v3 dataset. The objective was to identify authentication activity, investigate failed logons, analyze PowerShell execution, review network communications, and visualize event timelines.

---

## Objectives

- Analyze authentication events
- Investigate failed Windows logons
- Identify suspicious PowerShell execution
- Detect encoded PowerShell commands
- Review network communication patterns
- Build a timeline of activity
- Demonstrate basic threat hunting workflow

---

## Environment

- Splunk Enterprise
- BOTS v3 Dataset
- Windows Security Logs
- Sysmon Operational Logs

---

## Investigation Summary

### 1. Environment Discovery

Identified the primary log sources and monitored hosts within the environment before beginning analysis.

---

### 2. Authentication Analysis

Reviewed successful (Event ID 4624) and failed (Event ID 4625) logon events.

Observed:
- Multiple successful authentications
- Several failed authentication attempts
- Different Windows logon types
- Failure reasons including disabled accounts

---

### 3. PowerShell Investigation

Investigated PowerShell execution across Sysmon logs.

Focused on:

- Encoded PowerShell commands
- Command-line arguments
- Parent processes
- Process execution behavior

Encoded PowerShell activity was successfully identified and examined.

---

### 4. Network Investigation

Reviewed network communications by:

- Source IP
- Destination IP
- Destination Port

This allowed identification of the most common communication patterns across the environment.

---

### 5. Timeline Analysis

Built a visual timeline of activity to identify periods of increased event volume.

The timeline highlighted spikes in activity that would warrant additional investigation during a real SOC engagement.

---

## Skills Demonstrated

- Splunk SPL
- Threat Hunting
- Windows Event Logs
- Sysmon Analysis
- Authentication Investigation
- PowerShell Analysis
- Network Traffic Investigation
- Security Event Correlation
- Incident Triage

---

## Screenshots

The repository contains screenshots demonstrating each stage of the investigation.

---

## Author

**Omid Farani**

CompTIA Security+ Certified

Aspiring SOC Analyst
