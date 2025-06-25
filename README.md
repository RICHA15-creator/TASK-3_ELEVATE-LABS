# TASK-3_ELEVATE-LABS
# Perform-a-Basic-Vulnerability-Scan-on-your-PC

## Tasks
In kali linux terminal

## Introduction
In this project,  A basic vulnerability scan is a process where automated tools search for known security flaws in IT systems and software. This includes identifying missing updates, misconfigurations, and exposed secrets. The goal is to help organizations quickly identify and prioritize vulnerabilities for remediation, reducing the risk of security breaches. 

**Types of Vulnerability scan:**

  1.Network-based scans. 
  2.Web application scans. 
  3.Host-based scans.
## Pre-requisites
- Basic understanding of networking concepts (IP addresses, ports, etc.).
- Familiarity with using the OpenVAS.
- Kali Linux installed on your machine (either natively, on a virtual machine, or as a live boot).

## Lab Set-up and Tools

### Tools
- **Kali Linux:** A Debian-derived Linux distribution designed for digital forensics and penetration testing.
- **OpenVAS:** OpenVAS (Open Vulnerability Assessment System) is primarily used for vulnerability scanning and assessment. It's an open-source tool designed to identify and assess security vulnerabilities in computer systems, applications, and networks. By scanning for known vulnerabilities, OpenVAS helps organizations proactively identify weaknesses that could be exploited by malicious Actor.
                                                       **or**
- **Nessus Essentials**:Nessus is a remote security scanning tool, which scans a computer and raises an alert if it discovers any vulnerabilities that malicious hackers could use to gain access to any computer you have connected to a network.

### Installation
Install OpenVAS or Nessus Essentials. You can verify the installation or update it using the following command:
```sh
sudo apt-get update && sudo apt-get install nmap
```

## Tasks
In kali linux terminal
# Perform a Basic Vulnerability scan 
**Objective:** Use free tools to identify common vulnerabilities on your computer.
**Tools:** OpenVAS Community Edition(free vulnerability scanner) or Nessus Essentials.

## 1. Update Kali Linux official website
Before starting, update your system to avoid issues.

 ```sh
sudo apt update && sudo apt upgrade -y
```
<img width="956" alt="image" src="https://github.com/user-attachments/assets/b4387cd8-dd09-4012-9c25-8892d775bd49" />


## 2.Download Nessus Essentials for Linux

**Go to:**
> https://www.tenable.com/downloads/nessus?loginAttempted=true
<img width="954" alt="image" src="https://github.com/user-attachments/assets/adf5c2bc-466b-43e8-a782-89dc2bf32178" />

**Under Linux command prompt:**
Use the command after downloading the nessus essentials:
 ```sh
dpkg -i Nessus-<version>-debian<number>_amd64.deb
```
<img width="854" alt="image" src="https://github.com/user-attachments/assets/1cdfdab2-8d2d-4e38-9035-f08d70aa5347" />

**Then follow the instructions given in the last two lines:**

<img width="918" alt="image" src="https://github.com/user-attachments/assets/d94a3010-5a83-414b-bc8e-72c5be8c2eb6" />

## 3.Access Nessus Web
Once Nessus is running, open your browser and go to :
>https://localhost:8834/
(Here my localhost name is Kali)

It might show a certificate warning -click "Advanced">"Proceed".

<img width="789" alt="image" src="https://github.com/user-attachments/assets/65e2fbc3-1063-4021-9577-1d076534b4be" />
<img width="805" alt="image" src="https://github.com/user-attachments/assets/cd02c0f4-549e-4bf5-990d-2eb03b40f4cb" />

**Create an account in Nessus and register with your name and email**
<img width="955" alt="image" src="https://github.com/user-attachments/assets/9cdb3a1d-907e-4f0a-a1e0-f60d26c21903" />
<img width="953" alt="image" src="https://github.com/user-attachments/assets/d1fc0765-e5be-4cee-904d-30a7fd7b33d9" />
<img width="870" alt="image" src="https://github.com/user-attachments/assets/6bba7a0e-f36f-4a8d-89ba-d7052934711c" />


## 4.Create a Basic scan
**After the nessus page is fully initialized:**

<img width="959" alt="image" src="https://github.com/user-attachments/assets/8da5e0fd-94d0-4d3b-b1ed-e930aa778075" />

**Right side corner you have to click new scan but it takes some time for compiling**
after that you see some options by clicking on new .

<img width="927" alt="image" src="https://github.com/user-attachments/assets/ad4187f5-f5ff-4710-818d-cc4d4100f178" />

**Click on Advance scan since you need to scan your own PC.**
**Enter the IP address,to find IP address of your own PC by using the command :**
 ```sh
ip a
```
<img width="788" alt="image" src="https://github.com/user-attachments/assets/5a044342-a241-4123-b3c7-20fc405ff994" />

**Then click on My scans and select the scan type**
<img width="953" alt="image" src="https://github.com/user-attachments/assets/91bb01b1-561b-4d2e-9695-3da012b34c49" />

**Click on launch button to start vulnerability scan**
<img width="956" alt="image" src="https://github.com/user-attachments/assets/5e2e1d70-ea29-4e4d-8c9c-066f83ab50f0" />

**After Scanning is completed it shows the following results:**

<img width="959" alt="image" src="https://github.com/user-attachments/assets/bfa02a69-4c36-4063-9e56-85369a890a54" />


## 5.View the scan report
**Once the scan finishes ,click on scan name to view details**
**Here you'll see:**
Number of vulnerabilities ,severity breakdown(Critical,High,Medium,etc.),Vulnerable services(e.g., SSH,SMB,RDP).

<img width="950" alt="image" src="https://github.com/user-attachments/assets/c5e747f0-be4a-4086-9a1f-b59297b4f415" />



## 6.Documentation of most critical vulnerability of my PC 
**Here's the Description and solution for the critical vulnerability:**
<img width="955" alt="image" src="https://github.com/user-attachments/assets/3180bb6a-8385-44cb-9be4-60df0baa0639" />
<img width="959" alt="image" src="https://github.com/user-attachments/assets/3a5bfa5d-c859-4f34-b904-0656d660ddaf" />
<img width="953" alt="image" src="https://github.com/user-attachments/assets/b97af9b2-d6b6-47c5-9b2f-36d6ff2f60af" />










