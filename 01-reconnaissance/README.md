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

$curl http://target.ine.local/robots.txt
