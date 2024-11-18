# Foundational SOC Lab: Windows, Kali Linux, Sysmon, and Splunk Integration

This repository contains the setup and configuration for a **foundational Security Operations Center (SOC)** lab designed to help develop skills in log aggregation, event monitoring, and threat detection. The lab uses **VirtualBox** to create an isolated environment with **Windows 10** and **Kali Linux** VMs, along with **Sysmon** and **Splunk** for enhanced logging and log aggregation.

## Objective

The goal of this project was to create a basic SOC environment to:

- Set up and configure a Windows 10 VM and a Kali Linux VM in VirtualBox.
- Enhance Windows logging using **Sysmon** to track critical security events.
- Set up **Splunk** for log aggregation, searching, and visualization.
- Simulate network activity using **Nmap** from Kali Linux to test detection capabilities in Sysmon and Splunk.

## Tools & Technologies

- **Windows 10** VM
- **Kali Linux** VM
- **VirtualBox** (for virtualization and internal network setup)
- **Sysmon** (Windows event monitoring and logging)
- **Splunk** (log aggregation and analysis)
- **Nmap** (network scanning)

## Lab Setup

1. **Virtual Machine Configuration**:  
   - Created **Windows 10** and **Kali Linux** VMs in **VirtualBox**.
   - Configured an internal network for VM communication.

2. **Sysmon Setup on Windows 10**:  
   - Installed and configured **Sysmon** for enhanced logging (process creation, network connections, file creation times).
   - Logs collected in **Windows Event Viewer**.

3. **Splunk Configuration**:  
   - Installed **Splunk** on Windows to monitor and index **Sysmon** logs and **Windows Event Viewer** logs.
   - Configured Splunk to visualize and search event data.

4. **Network Activity Simulation**:  
   - Performed an **Nmap scan** from **Kali Linux** to simulate network activity.
   - Used **Sysmon** and **Splunk** to detect and analyze the scan.

## Key Features

- **Sysmon Log Configuration**: Tracks process creation, network connections, and file activity.
- **Splunk Log Aggregation**: Collects and indexes logs from both Sysmon and the Windows Event Viewer for easy search and visualization.
- **Network Threat Detection**: Simulates a basic **Nmap scan** to test the ability of Sysmon and Splunk to detect suspicious network activity.
