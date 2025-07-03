#  Cybersecurity Internship Task 1 Report

**Date:** July 2, 2025  
**Intern:** Soham Sharma

---

## 🔍 Task Objectives

- Scan your local network for open ports  
- Analyze a phishing email sample  
- Create a report and upload it to GitHub

---

## ✅ Task 1: Scan Your Local Network for Open Ports

### 🛠️ Tools Used

- **Nmap** – Network scanning tool  
- **Wireshark** – Packet analyzer  
- **ifconfig** & **ip addr** – Network interface inspection

---

### 📡 Network Setup

| Interface | IP Address | MAC Address         |
|----------:|:-----------|:--------------------|
| `eth0`    | 10.0.2.15  | 08:00:27:99:e3:fa   |
| `lo`      | 127.0.0.1  | N/A                 |

---

### 🔎 Nmap Command Used

```bash
nmap -sS 10.0.2.15/24
```
### Nmap Scan Results
Host 10.0.2.2
**Open Ports:**

135/tcp – Microsoft RPC

445/tcp – Microsoft-DS (SMB)

3306/tcp – MySQL

5432/tcp – PostgreSQL

Host 10.0.2.3
Open Ports:

53/tcp – DNS

Host 10.0.2.15 (Self)
All 1000 scanned ports are closed.

---

### 🧪 Wireshark Traffic Analysis
Captured live traffic on interface eth0

Observed TCP SYN, RST-ACK handshake behavior

**Source:** 10.0.2.2

**Destination:** 10.0.2.15

Indicated active scanning behavior

---

📸 Screenshot Evidence
✅ Network interfaces using ifconfig and ip addr

✅ Nmap scan results

✅ Wireshark capture of TCP traffic
![1c39ff17-31f0-4e02-97c7-74a259349ce0](https://github.com/user-attachments/assets/d2d9ee02-95e0-4e1b-a0d9-00ecff82405f)

![1f6dac22-770f-46df-bcaa-e8a8c8e88756](https://github.com/user-attachments/assets/e94dba20-3b85-4151-bb13-5efcbb2b07b5)


All screenshots are included in the repository under /screenshots/
