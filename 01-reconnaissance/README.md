# 01 - Reconnaissance

## Objective

The objective of this phase is to gather information about the target environment before performing detailed scanning and enumeration.

## Scope

The assessment is limited to the authorized and isolated laboratory environment.

## Activities

- Identify the target IP address
- Identify the network range
- Identify live hosts
- Collect initial information about the target environment
- Document the reconnaissance results

## Tools

- Nmap
- Linux networking tools

## Methodology

The reconnaissance phase begins with host discovery and basic network identification.

No exploitation is performed during this phase.

## Results

Results will be documented after completing the reconnaissance activities.

## Status

---

## Finding 1 - robots.txt

### Objective

Identify information exposed through the website's `robots.txt` file.

### Command

$curl http://<TARGET_IP>/robots.txt


## Finding 2  - Web Technology Identification

### Objective

Identify the web application technology and version running on the target.

### Tool

Nmap

### Command

nmap -A <TARGET_IP>

---

## Finding 3 - Directory Listing

### Objective

Identify publicly accessible directories and files on the target web server.

### Tool

DIRB

### Command

```bash
dirb http://<TARGET_IP>
