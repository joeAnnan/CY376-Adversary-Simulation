# CY376 Adversary Simulation

## Red Team Engagement: Initial Access to Objective

This repository contains the supporting materials for a CY376 (Network Security, Auditing and Monitoring) individual project completed at the University of Mines and Technology (UMaT).

The project presents a full Red Team adversary simulation carried out within an isolated VMware lab. The engagement followed a realistic attack lifecycle, starting with reconnaissance, moving through initial access and privilege escalation, and concluding with successful access to a simulated confidential objective.

## 

## Project Information

* Student: **Joseph Oboh Annan**
* Index Number: FCM.41.018.060.23
* Course: CY376 Network Security, Auditing and Monitoring
* Institution: University of Mines and Technology (UMaT)
* Project Type: Individual Red Team Adversary Simulation

## 

## Project Objectives

The project set out to achieve the following:

* Design and deploy an isolated adversary simulation laboratory
* Identify exposed services through reconnaissance
* Gain initial access using a realistic attack vector
* Escalate privileges from a standard user account to root
* Demonstrate successful access to a protected objective
* Document findings and provide security recommendations

## 

## Lab Environment

The simulation was conducted entirely within an isolated VMware environment made up of two Ubuntu 22.04 virtual machines.

|Machine|Purpose|
|-|-|
|Attacker VM|Reconnaissance and exploitation|
|Victim VM|Simulated PaySwift Ghana server|

A host only network was used throughout the lab to keep all attack traffic contained and isolated from external systems.

## 

## Tools Used

* VMware Workstation
* Ubuntu 22.04 LTS
* Nmap
* Nikto
* Hydra
* OpenSSH
* Docker
* Damn Vulnerable Web Application (DVWA)
* GTFOBins

## 

## Attack Lifecycle

The engagement was structured around the following phases:

1. Reconnaissance
2. Service Enumeration
3. Initial Access
4. Foothold
5. Privilege Escalation
6. Objective Access

## 

## Repository Structure

**docs**
Contains the final project report.

**evidence**
Contains screenshots collected throughout the engagement.

**scripts**
Contains the commands used during the engagement and a custom password wordlist, where applicable.

**configs**
Contains supporting configuration files and notes.

**diagrams**
Contains network or lab diagrams, where applicable.

## 

## Evidence

Screenshots are organised by engagement stage:

* Reconnaissance
* Initial Access
* Privilege Escalation
* Objective
* Web Enumeration

## 

## Report

The complete project report can be found in the docs directory.

## 

## Academic Notice

This project was carried out entirely within an isolated laboratory environment built for academic purposes. No third party systems were targeted, and none of the techniques described in this repository were used against production or unauthorized environments.

## 

## License

This repository is made available solely for academic assessment and educational purposes.

