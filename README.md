# Network-Security-Project

A preconfigured virtual network security environment built using VirtualBox and Ubuntu systems to demonstrate secure remote access, firewall management, log monitoring, and network traffic analysis using industry-standard tools.

---

## Project Overview

This project demonstrates the implementation of a small virtual enterprise-style network using multiple Ubuntu virtual machines connected through VirtualBox networking.

The environment was preconfigured and connected previously, including network interfaces and communication setup between the systems.

The project focuses on practical cybersecurity concepts such as:

- Secure remote access using SSH
- Secure file transfer using SCP
- Host-based firewall configuration
- Log monitoring and authentication tracking
- Network traffic analysis using Wireshark
- Connectivity verification and packet inspection

---

## Objectives

- Build and manage a virtual network environment
- Configure secure SSH communication between machines
- Apply firewall rules for controlled access
- Monitor authentication and system logs
- Analyze network traffic and encrypted communication
- Verify connectivity using ICMP and TCP traffic
- Demonstrate secure file transfer between hosts

---

## Environment Setup

### Virtual Machines

- Ubuntu Base
- ubuntu-1
- ubuntu-2

### Virtualization Platform

- VirtualBox

### Network Configuration

The systems were already preconfigured and connected using:

- NAT Adapter (Internet access)
- Host-Only Adapter (Internal communication)

This allowed secure communication between all virtual machines inside the isolated virtual network.

---

## Tools and Technologies Used

| Tool | Purpose |
|------|----------|
| VirtualBox | Virtual machine management |
| Ubuntu Linux | Operating systems |
| OpenSSH Server | Secure remote access |
| OpenSSH Client | SSH client communication |
| SCP | Secure file transfer |
| firewalld | Host-based firewall management |
| journalctl | System and SSH log monitoring |
| grep | Log filtering and analysis |
| Wireshark | Network packet analysis |
| ping | Connectivity testing |
| ip addr | Network interface verification |

---

## Features Implemented

### Secure Remote Access (SSH)

- Installed and configured OpenSSH server
- Enabled secure remote login between machines
- Disabled root login for improved security
- Verified encrypted communication over port 22

### Secure File Transfer (SCP)

- Transferred files securely between Ubuntu systems
- Verified successful encrypted file delivery

### Firewall Configuration

- Configured firewalld service
- Allowed SSH traffic through firewall rules
- Verified firewall policies and active services

### Log Monitoring

- Monitored SSH authentication logs
- Observed successful and failed login attempts
- Analyzed system activity using journalctl

### Network Traffic Analysis

Using Wireshark, the project captured and analyzed:

---

## Sample Commands Used

### SSH Connection

```bash
ssh username@IP_ADDRESS
```

### Secure File Transfer

```bash
scp testfile.txt username@IP_ADDRESS:/home/username
```

### Firewall Verification

```bash
firewall-cmd --list-all
```

### Log Monitoring

```bash
journalctl -u ssh --no-pager
```

### Network Testing

```bash
ping IP_ADDRESS
```

---

## Results

The project successfully demonstrated:

- Stable communication between all virtual machines
- Secure SSH connectivity
- Secure SCP file transfers
- Firewall rule enforcement
- Effective authentication monitoring
- Successful packet capture and protocol analysis using Wireshark

---

## Documentation

For detailed implementation steps, screenshots, configurations, and analysis, please refer to the PDF report included in this repository.

---

## Author

Remas Aljohani
