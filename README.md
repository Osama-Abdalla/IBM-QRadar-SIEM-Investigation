# IBM-QRadar-SIEM-Investigation

## Overview
IBM QRadar is an enterprise-grade Security Information and Event Management (SIEM) platform designed to provide intelligent insights into network traffic, user activity, and vulnerability management. This report documents a detailed investigation into a sophisticated cyber attack against HACKDEFEND.local, performed using QRadar to analyze integrated log sources.

## Scenario:
A financial company was compromised, and they are looking for a security analyst to help them investigate the incident. The company suspects that an insider helped the attacker get into the network, but they have no evidence.
The initial analysis performed by the company's team showed that many systems were compromised. Also, alerts indicate the use of well known malicious tools in the network. As a SOC analyst, you are assigned to investigate the incident using QRadar SIEM and reconstruct the events carried out by the attacker.
 
## Dataset:
- Sysmon - swift on security configuration
- Powershell logging
- Windows Eventlog
- Suricata IDS
- Zeek logs (conn, HTTP)

## tools:
- IBM Qradar
- MITTR ATTACK framework
