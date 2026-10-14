# Kali Linux System Information & Network Testing

## Project Overview

This project demonstrates practical Linux and networking fundamentals using a Kali Linux virtual machine (VM). Completed as part of a 10Alytics practical assignment, the work involved gathering system information, checking system resources, and testing basic network connectivity.

The project documents the commands used, the results obtained, and supporting screenshots as evidence of the practical work.

## Project Objectives

- Identify the current Linux username, hostname, and working directory.
- Retrieve operating system and kernel information.
- Check memory usage and available disk space.
- Test network connectivity to a known IP address.
- Test domain name resolution and connectivity using a domain name.
- Record and interpret network response times and packet loss.
- Document technical results clearly using screenshots and a written report.

## Tools & Technologies

- **Operating System:** Kali Linux
- **Environment:** Virtual machine
- **Command Line:** Linux terminal
- **System Information:** `whoami`, `hostname`, `pwd`, `uname -a`
- **Resource Monitoring:** `free -h`, `df -h`
- **Network Testing:** `ping`
- **Evidence:** Terminal screenshots and practical assignment report

## Project Tasks & Methodology

### 1. Identify the System Environment

I used basic Linux commands to identify the current user, hostname, and working directory.

**Commands used:**

```bash
whoami
hostname
pwd
```

**Results:**

- Username: `kali`
- Hostname: `stephen`
- Working directory: `/home/kali`

**What I learned:** These commands help establish the current user context and location within the Linux filesystem when working in a terminal.

### 2. Check Operating System Information

I used the `uname -a` command to retrieve information about the Linux kernel and system environment.

**Command used:**

```bash
uname -a
```

**Recorded result:**

- Linux kernel version: `6.19.14+kali-amd64`

**What I learned:** Kernel information is useful when identifying the operating system environment and documenting a system for troubleshooting or technical assessment.

### 3. Check Memory Usage

I used `free -h` to inspect memory and swap usage.

**Command used:**

```bash
free -h
```

**Recorded result:**

- Total RAM: approximately 1.9 GiB

**What I learned:** Memory information helps provide an overview of available system resources and supports basic system troubleshooting.

### 4. Check Available Disk Space

I used `df -h` to inspect filesystem capacity and available storage.

**Command used:**

```bash
df -h
```

**Recorded result:**

- Available space on the main `/dev/sda1` partition: approximately 59 GB

**What I learned:** Checking disk capacity helps identify available storage and can assist with basic system maintenance and troubleshooting.

### 5. Test Connectivity to a Known IP Address

I used `ping` to test connectivity to `8.8.8.8`.

**Command used:**

```bash
ping -c 2 8.8.8.8
```

**Results:**

- Packets transmitted: 2
- Packets received: 2
- Packet loss: 0%
- Average round-trip time: 16.803 ms

**What I learned:** The test received responses to both packets, with no packet loss observed during this short test. The round-trip time provided a basic measure of network response time.

### 6. Test Domain Name Resolution and Connectivity

I then tested connectivity using the domain name `google.com`.

**Command used:**

```bash
ping -c 4 google.com
```

**Results:**

- Domain tested: `google.com`
- Resolved IP address: `142.251.30.113`
- Packets transmitted: 4
- Packets received: 4
- Packet loss: 0%
- Average round-trip time: 12.961 ms

The `-c 4` option instructs `ping` to send four packets before stopping.

**What I learned:** The domain resolved to an IP address, and all four packets received responses. This demonstrated successful name resolution and connectivity to the destination during the test.

## Results Summary

| Test | Result |
|---|---|
| Username | `kali` |
| Hostname | `stephen` |
| Working directory | `/home/kali` |
| Linux kernel | `6.19.14+kali-amd64` |
| Total RAM | Approximately 1.9 GiB |
| Available space on `/dev/sda1` | Approximately 59 GB |
| Connectivity test to `8.8.8.8` | 0% packet loss |
| Average response time to `8.8.8.8` | 16.803 ms |
| Domain tested | `google.com` |
| Resolved IP address | `142.251.30.113` |
| Connectivity test to `google.com` | 0% packet loss |
| Average response time to `google.com` | 12.961 ms |

These figures reflect the results recorded in the assignment and apply to the test session. Network response times can vary depending on network conditions and the destination.

## Evidence & Screenshots

The accompanying practical assignment PDF contains screenshots supporting the following activities:

1. **System identification:** `whoami`, `hostname`, and `pwd` — page 2.
2. **Kernel information:** `uname -a` — page 3.
3. **Memory and disk usage:** `free -h` and `df -h` — page 4.
4. **IP connectivity test:** `ping -c 2 8.8.8.8` — page 5.
5. **Domain connectivity test:** `ping -c 4 google.com` — page 6.
6. **Consolidated results:** summary table — page 7.

The screenshots provide evidence of the commands executed and the results observed.

## Key Learning Outcomes

Through this project, I developed practical experience in:

- Using Linux terminal commands to inspect a system.
- Identifying basic operating system and kernel information.
- Checking memory and disk resources.
- Performing basic network connectivity tests.
- Understanding packet transmission, packet loss, and round-trip time.
- Observing DNS name resolution when testing a domain.
- Recording technical results and supporting them with evidence.

## Relevance to Cybersecurity

System visibility, basic networking knowledge, and accurate technical documentation are useful foundations for cybersecurity and IT security work.

These skills support further learning in system administration, network troubleshooting, security operations, and evidence-based technical reporting.

## Scope & Limitations

This project focused on basic system information and network connectivity testing.

- It was not a penetration test or vulnerability assessment.
- It did not include vulnerability scanning or exploitation.
- The results represent a limited test session and do not establish continuous network availability or overall network security.
- Commands such as `lscpu` and `uptime` were not included in the supplied evidence.

## Future Improvements

Potential extensions to this lab include:

- Collecting additional system information and documenting the results.
- Exploring network configuration and interface details.
- Practising additional Linux troubleshooting commands.
- Capturing and analysing network traffic in a controlled lab.
- Building a separate network security lab using Cisco Packet Tracer.
- Improving the documentation with further screenshots and repeatable test procedures.

## Author

**Stephen Adesina**

Cybersecurity | Information Security | Networking | GRC

This project forms part of my ongoing practical learning and portfolio development in cybersecurity and information security.

