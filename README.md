# Azure VM CPU ALERT SYSTEM
Azure Monitor CPU alert system with Action Groups and real-time alert validation

## Project Overview

This project demonstrates how to monitor a virtual machine in Microsoft Azure and configure automated alerts for high CPU usage. It simulates real-world L1 support tasks such as performance monitoring, alert configuration, and incident validation.

##  Problem Statement

In production environments, high CPU usage can impact application performance. The goal of this project is to proactively detect CPU spikes and notify administrators using Azure Monitor and Action Groups.

##  Architecture

Azure VM → Azure Monitor Metrics → Alert Rule (CPU > 80%) → Action Group → Email Notification

## Technologies Used

* Microsoft Azure
* Azure Virtual Machines (Linux - Ubuntu)
* Azure Monitor
* Azure Alerts
* Action Groups
* SSH (Secure Shell)

## Implementation Steps

### 1. Create Virtual Machine

* Deployed Ubuntu Linux VM in Azure
* Configured SSH access

### 2. Install Stress Tool

* Connected via SSH
* Installed stress tool to simulate CPU load

### 3. Monitor Metrics

* Used Azure Monitor to track CPU usage
* Verified metrics in Azure portal

### 4. Create Action Group

* Configured email notification for alerts

### 5. Configure Alert Rule

* Metric: Percentage CPU
* Condition: Greater than 80%
* Evaluation period: 5 minutes

### 6. Trigger Alert

* Generated CPU load using stress command
* Verified alert firing in Azure Monitor

##  Screenshots

* VM Creation
* SSH Connection
* Stress Tool Installation
* CPU Metrics Graph
* Action Group Configuration
* Alert Rule Configuration
* Alert Fired

##  Test Command Used

```bash
stress --cpu 2 --timeout 300
```

## ✅ Results

* Successfully monitored CPU usage
* Alert triggered when CPU exceeded threshold
* Verified alert in Azure portal


## 🎯 Conclusion

This project demonstrates real-world cloud monitoring and alerting skills relevant for Azure Administrator and L1 Support roles.
