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

## Finding 1 - robots.txt

### Objective

Identify information exposed through the website's `robots.txt` file.

### Command

$curl http://<TARGET_IP>/robots.txt


## Finding 2  - Web Technology Identification

### Objective

Identify the web application technology and version running on the target.
We can find http-generator: Web Application Technology (i.e.WordPress 6.5.3) 

### Tool

Nmap

### Command

nmap -A <TARGET_IP>
Option -A Enable OS detection, version detection, script scanning, and traceroute

**RESULTS**

**http-generator: WordPress 6.5.3 - FL@G2{XXXXXXXXXXX}** 


## Finding 3 - Directory Listing

### Objective

Identify publicly accessible directories and files on the target web server.

### Tool

DIRB

### Command

$dirb http://<TARGET_IP>

## Finding 4 - WordPress Configuration Backup

### Objective

Identify publicly accessible backup files that may expose sensitive configuration information.

### Tool

WPScan

### Command

$wpscan --url http://<TARGET_IP>


## Finding 5 - Mirrored Website Content Analysis

### Objective

Identify potentially interesting information contained within the website by creating a local mirror.

### Tool

HTTrack

### Command

$httrack

**OUTPUT**
A cache (hts-cache/) has been found in the directory 
That means that a transfer has been aborted
OK to Continue httrack httrack?

Press <Y><Enter> to confirm, <N><Enter> to abort 

**DIGIT Y**
Enter the information and mirror the website. By default the folder is root/websites/name of the project
Once inside digit the follow command:

### Command
$grep -r "FLAG" 
