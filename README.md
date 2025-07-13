# 🛡️ SOC-Analyst-HomeLab – Malware Reverse Shell Lab

This repository documents a hands-on reverse shell malware test in a secure SOC analyst home lab using Kali Linux and Windows 10 virtual machines. The goal is to simulate a real-world attack and detection workflow while keeping everything safely isolated.

---

## ✅ What I Did

- Set up a Kali Linux VM and a Windows 10 VM in VirtualBox
- Configured both VMs on an Internal Network (`MyTest`) to isolate them from the internet
- Assigned static IPs:
  - Kali: 192.168.20.11
  - Windows: 192.168.20.10
- Disabled Windows Firewall to allow ping and reverse shell
- Performed an Nmap scan from Kali and discovered port 3389/tcp (RDP) was open
- Created a malicious reverse shell payload using msfvenom
- Set up a Metasploit multi/handler listener to capture the reverse shell
- Served the file from Kali using a local web server
- Downloaded and executed the file on the Windows VM
- Verified the reverse shell was active through network and task manager tools
- Took VM snapshots before and after testing to preserve clean and infected states

---

## 📁 Project Structure

- Nmap Scan section: Identifies target ports and services
- Payload Generation: Reverse shell creation
- Exploit Handler: Listener setup
- Malware Delivery: File hosting and retrieval
- Shell Verification: Confirming successful connection

---

⚠️ This project is for educational purposes only. All activities were conducted in a safely isolated environment. Never run malware on your host machine or public network.

---

**Author:** Harrison  
SOC Analyst in Training | Cybersecurity Student

