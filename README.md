# IBM-QRadar-SIEM-Investigation

## Overview
IBM QRadar is an enterprise-grade Security Information and Event Management (SIEM) platform designed to provide intelligent insights into network traffic, user activity, and vulnerability management. This report documents a detailed investigation into a sophisticated cyber attack against HACKDEFEND.local, performed using QRadar to analyze integrated log sources.

## Scenario:
A financial company was compromised, and they are looking for a security analyst to help them investigate the incident. The company suspects that an insider helped the attacker get into the network, but they have no evidence.
The initial analysis performed by the company's team showed that many systems were compromised. Also, alerts indicate the use of well known malicious tools in the network. As a SOC analyst, you are assigned to investigate the incident using QRadar SIEM and reconstruct the events carried out by the attacker.
 
## Dataset:
- Sysmon - swift on security configuration.
- Powershell logging.
- Windows Eventlog.
- Suricata IDS.
- Zeek logs (conn, HTTP).

## tools:
- IBM Qradar.
- MITTR ATTACK framework.
- Github

## Case Analysis 
- How many log sources available?
- What is the IDS software used to monitor the network?

<img width="1273" height="686" alt="image" src="https://github.com/user-attachments/assets/fbe973cd-3471-4bfe-ba58-0b0d1a05e22a" />

- What is the domain name used in the network?

<img width="1798" height="920" alt="image" src="https://github.com/user-attachments/assets/3454ea3a-022d-475a-82ad-c5a324a4d89b" />

- Multiple IPs were communicating with the malicious server. One of them ends with "20". Provide the full IP.

<img width="422" height="172" alt="image" src="https://github.com/user-attachments/assets/85d2951c-bdef-4099-9477-b701e51b7cad" />

- What is the SID of the most frequent alert rule in the dataset?

<img width="1798" height="783" alt="image" src="https://github.com/user-attachments/assets/65fe7844-a744-432f-bb11-bd8822e9ef33" />

- What is the attacker's IP address?

<img width="1770" height="861" alt="image" src="https://github.com/user-attachments/assets/664180f9-eaf3-4b20-a85b-f2e0470e8595" />
<img width="1519" height="268" alt="image" src="https://github.com/user-attachments/assets/86caf4e3-29d6-4511-a06f-0fe2542267f6" />

- The attacker was searching for data belonging to one of the company's projects, can you find the name of the project?
  
<img width="1767" height="630" alt="image" src="https://github.com/user-attachments/assets/a79ad02b-c2d8-4398-9b31-27d3c9429b37" />
<img width="1768" height="384" alt="image" src="https://github.com/user-attachments/assets/3c66420a-990b-485e-9496-c48a9b861339" />

- What is the IP address of the first infected machine?

<img width="800" height="256" alt="image" src="https://github.com/user-attachments/assets/fee6004d-11c4-4e54-93e7-cb75c91969ca" />
<img width="1474" height="137" alt="image" src="https://github.com/user-attachments/assets/1dad4dea-5317-45d8-85f1-9820ead57671" />

- What is the username of the infected employee using 192.168.10.15?

<img width="1416" height="427" alt="image" src="https://github.com/user-attachments/assets/8a5f883a-e67b-413d-a45c-43ca6e5a4c7e" />

- Hackers do not like logging, what logging was the attacker checking to see if enabled?
Current Filters:
Username is any of nour

<img width="1608" height="325" alt="image" src="https://github.com/user-attachments/assets/7115d761-deda-454b-be32-8fdaa59035fd" />

- Name of the second system the attacker targeted to cover up the employee?

<img width="1252" height="366" alt="image" src="https://github.com/user-attachments/assets/cf8e37dc-6752-4161-bc6a-ff0f6189555e" />
<img width="1754" height="681" alt="image" src="https://github.com/user-attachments/assets/d9a8c8f9-ddb1-4c4b-bae9-08a4ad64b562" />

- When was the first malicious connection to the domain controller (log start time - hh:mm:ss)?

<img width="1768" height="584" alt="image" src="https://github.com/user-attachments/assets/f6acdba7-d51e-482a-95f4-f3ae8bae7ad4" />

- What is the md5 hash of the malicious file?
Payload Contains is md5

<img width="1589" height="288" alt="image" src="https://github.com/user-attachments/assets/30e084de-2fda-4f88-a8aa-7e1f74b9b09a" />

- What is the MITRE persistence technique ID used by the attacker?
EventID (custom) is any of 13
<img width="1780" height="708" alt="image" src="https://github.com/user-attachments/assets/b4ef5704-b785-450f-818d-3e08b1ab59f5" />
<img width="1602" height="361" alt="image" src="https://github.com/user-attachments/assets/59b8be9f-b90f-4e25-9ddb-18d1cd253de6" />
<img width="1755" height="549" alt="image" src="https://github.com/user-attachments/assets/2e4ca161-5bf6-4df7-80d8-bcc9eb35147f" />

- What protocol is used to perform host discovery?
  
<img width="1082" height="401" alt="image" src="https://github.com/user-attachments/assets/2904eb07-369a-4a94-801c-b5c051fef9ae" />
<img width="1771" height="629" alt="image" src="https://github.com/user-attachments/assets/3642fb75-a17d-41e3-8432-6dc0470c55d8" />
<img width="1525" height="335" alt="image" src="https://github.com/user-attachments/assets/d291f667-0e4c-48eb-a623-64cc4ea36a2e" />

- What is the email service used by the company?

<img width="800" height="151" alt="image" src="https://github.com/user-attachments/assets/6f7b0f4a-1023-4f2a-a47c-aeb74ad12fee" />
<img width="1770" height="250" alt="image" src="https://github.com/user-attachments/assets/9bdf2497-2073-4c68-bd41-3f82cfe6d156" />
<img width="911" height="320" alt="image" src="https://github.com/user-attachments/assets/e3a721b9-caea-41e8-a785-b0f870ced3c4" />

office365

- What is the name of the malicious file used for the initial infection?

  <img width="1770" height="468" alt="image" src="https://github.com/user-attachments/assets/e73a3e1e-8315-43d2-aed3-7bb2080e7799" />
  <img width="1682" height="374" alt="image" src="https://github.com/user-attachments/assets/a11438a0-1f58-41f7-a9fb-360b369e0101" />

- What is the name of the new account added by the attacker?
EventID (custom) is any of 4720

<img width="1568" height="370" alt="image" src="https://github.com/user-attachments/assets/5feea077-9ad6-497d-8314-286ddb685823" />

- What is the PID of the process that performed injection?

EventID (custom) is any of 8

<img width="1610" height="371" alt="image" src="https://github.com/user-attachments/assets/187a162b-cc83-4c53-af5c-7b251322c85a" />

- What is the name of the tool used for lateral movement?

<img width="1790" height="863" alt="image" src="https://github.com/user-attachments/assets/ed4d169a-f9e3-422f-8816-b36858c87a75" />
<img width="1764" height="124" alt="image" src="https://github.com/user-attachments/assets/b7064a5f-dae1-4aec-a836-d992f0dac733" />
<img width="1780" height="645" alt="image" src="https://github.com/user-attachments/assets/de2d7612-9c2f-430f-9abe-fef2e8c3cf22" />
<img width="1603" height="907" alt="image" src="https://github.com/user-attachments/assets/aac967f0-421f-4671-8ed9-130b7f8d7d53" />

- Attacker exfiltrated one file, what is the name of the tool used for exfiltration?

<img width="1686" height="371" alt="image" src="https://github.com/user-attachments/assets/43e53d48-15aa-4ceb-bbcc-88ecb1ef5c2e" />

- Who is the other legitimate domain admin other than the administrator?
EventID (custom) is any of 4672

<img width="1374" height="187" alt="image" src="https://github.com/user-attachments/assets/fbb8cf2f-1b2a-4850-a1f8-a0abb4b9b94a" />
<img width="1374" height="187" alt="image" src="https://github.com/user-attachments/assets/bc38604d-07be-4ac5-9cad-36a714338ce8" />

- What is the name of the employee who hired the attacker?

<img width="1759" height="639" alt="image" src="https://github.com/user-attachments/assets/948adea8-a111-4c0a-b9b1-96263cad433a" />
<img width="1609" height="355" alt="image" src="https://github.com/user-attachments/assets/dd08f681-867a-4010-bec3-919035799ac0" />

sami

## Disclaimer & Acknowledgement
This investigation was conducted as part of the QRadar 101 lab provided by Cyber Defenders. All scenarios and data are designed for educational purposes to develop and hone forensic investigation skills in a simulated environment.


