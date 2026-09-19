# -Phases-of-Ethical-Hacking-Reconnaissance-and-Scanning.-

Reconnaissance and Scanning of the target in authorised lab environment.

## ⚠️ 1. Liability Disclaimer

I have performed these activities only on the systems & devices where I had secured written permission or the devices/systems that I own myself. All these materials are for education and research purpose only. Do not use anything from here to break the law. The instructor, the authors and Networkwalks are not responsible for what you do with this knowledge. Every action you take is your own responsibility. Misuse can lead to criminal charges, heavy fines, loss of your job and a permanent record. In most countries unauthorised access is a crime even when nothing is damaged.

## 📌 2. Project Overview

In this Repository documents contains the 2nd week's project of Cybersecurity Internship Program at Networkwalks. It covers the first 2 phases of Ethical Hacking,

* Footprinting and Reconnaissance
* Scanning

## 🛠️ 3. Tools and Resources Used

| Tools/Resources   | Description                                                                                    |
| ----------------- | ---------------------------------------------------------------------------------------------- |
| Kali Linux        | An Operating system used by Cyber Security professionals for various ethical hacking purposes. |
| Windows 11        | Common software used in most of PCs for GUI and CLI purposes.                                  |
| theHarvester      | OSINT (Open Source Intelligence) reconnaissance tool used in Kali Linux.                       |
| Zenmap (Nmap GUI) | GUI based network mapping tool, used for network scanning and mapping.                         |

## ⚙️ 4. Execution Process

### Phase 1: Footprinting & Reconnaissance using theHarvester for information gathering.

**Task 1:** In Task 1, we executed a target search against microsoft.com. We used the "Baidu" module with a limit of 1000 results.

**Note:** In the command:

* `-d` is used for domain selection
* `-l` is used to limit result limits
* `-b` is used for selecting data sources

**Command:**

```bash
theHarvester -d microsoft.com -l 1000 -b baidu
```

**Task 2:** In Task 2, we executed a broader search on microsoft.com.

**Command:**

```bash
theHarvester -d microsoft.com -l 50 -b all
```

**Output:**

```text
starting the harvester
```

### Phase 2: Scanning Networks

Open Windows Command Prompt, type the command `ipconfig` and hit Enter. By doing this, we can find our local IP address, subnet mask, and default gateway.

Open Zenmap, enter the local subnet range, select the **Ping scan** profile, and start the scan. Zenmap will scan the local network and provide the available hosts and open ports on the network.

Locate the **Topology** tab and head to **Fisheye**. In this tab, we can find the topology of the network.

## 🚩 Challenges Encountered and Solutions

**Problem:** Due to slow network speed in the Kali Linux Lab, theHarvester scan was dismissed and the terminal froze.

**Solution:** Reviewed the network settings, repaired the subnet range, and restarted the Linux lab.

## 🛠️ Resource Used

* **Kali Linux 2026.2** :- https://kali.org/get-kali
* **theHarvester** :- OSINT and Footprinting tool
* **Zenmap** :- https://nmap.org/download.html

## 👤 Author

**Mithilesh Vijay Sonavane**
Cyber Security and Forensics Student
LinkedIn: https://www.linkedin.com/in/mithilesh-sonavane-a08766374?utm_source=share_via&utm_content=profile&utm_medium=member_android

## 🗂️ Project Information

**Program Name:** Cybersecurity at Networkwalks
**Week:** 02
**Project:** Penetration Testing Report: Footprinting & Network Scanning (theHarvester & Zenmap)
**Repository:** GitHub
