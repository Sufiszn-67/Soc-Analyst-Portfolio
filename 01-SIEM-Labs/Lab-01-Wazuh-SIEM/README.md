#  🔵 Lab 01 - Wazuh SIEM Home Lab 

## Overview 



This lab was designed to simulate how a real-world cyberattack would unfold when vulnerabilities are present on endpoint. The overall goal was to understand how threat actors perform reconnaissance and brute force attacks, and how SOC analyst monitors and detect those attacks through a security information and events management tool. Therefore by building this environment from scratch, I gained hands-on experience from both the offensive and defensive sides of a security incident.

---

## Environment 

The lab consisted of three virtual machines all simultaneously running on the same isolated network infrastructure within the Oracle VM Virtual Box. The three virtual machines were:


- Wazuh version 4.14.5 – The security information and events management system
- Windows 10 pro – The target/victim machine with the Wazuh agent deployed on and installed upon.
- Kali Linux 2026.1 – The attacker machine.


All three machines were connected via the Nat Network which I named SOC-Lab-01-Wazuh for familiarly sake within the subnet 10.0.2.0/24 provided automatically, which allowed them to all communicate with each other whilst remaining completely isolated from the real network.

| Machine | Role | IP Address |
|---------|------|------------|
| Wazuh v4.14.5 | SIEM Server | 10.0.2.10 |
| Windows 10 Pro | Target Machine | 10.0.2.5 |
| Kali Linux 2026.1 | Attacker Machine | 10.0.2.6 |
