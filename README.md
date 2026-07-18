# Network Reconnaissance with Nmap

## Overview

## Objectives
1. Understand host discovery
2. Identify live systems
3. Enumerate open ports
4. Detect running services
5. Perform OS fingerprinting
6. Interpret scan results
7. Produce a professional reconnaissance report

## Lab Environment

Oracle Virtualbox VMs with Kali Linux and Windows 10
Same lab set up as cybersecurity_home_lab >> https://github.com/jaya049/cybersecurity_home_lab.git

## Architecture

<img width="451" height="251" alt="portscan drawio" src="https://github.com/user-attachments/assets/1b6b9686-fd5c-4740-a02f-8d2d6837c6f1" />


## Reconnaissance Methodology

### Phase 1: Verify Connectivity
From Kali : ping <windows_ip>
<img width="358" height="131" alt="image" src="https://github.com/user-attachments/assets/cae74e3b-7f6b-4a86-87d3-a4ab345bc4f8" />

### Phase 2: Host Discovery
From Kali : nmap -sn <windows_ip>
<img width="307" height="68" alt="image" src="https://github.com/user-attachments/assets/b4899f71-30f6-47f6-b685-aa4556696d94" />

- This checks whether a host is online without scanning for open ports.
- With -sn Nmap skips port scan and only check which devices are online; Faster than port scan. Instead of scanning every single IP for open ports (which is slower), you first discover which devices are actually online.
- Benefits
    - Faster scanning
    - Less unnecessary network traffic
    - Better organized reconnaissance
    - Common first step during penetration testing and network inventories
- Findings (From out screenshot)
    -  The target host responded successfully to the host discovery scan.
    -  Host is online
    -  VirtualBox network adapter detected


## Scan Results

## Findings

## Recommendations

## Lessons Learned
