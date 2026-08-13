/Test-1/
   <h1 align="center"> 💻 Cybersecurity Lab Environment Setup </h1>

<p align="center">
</p>
<p align="center">

  <img src="https://img.shields.io/badge/Cybersecurity-0F172A?style=for-the-badge&labelColor=2563EB&logo=kalilinux&logoColor=white" alt="Cybersecurity" />

  <img src="https://img.shields.io/badge/Kali%20Linux-v2026.2-111827?style=for-the-badge&labelColor=0EA5E9&logo=kalilinux&logoColor=white" alt="Kali Linux" />

  <img src="https://img.shields.io/badge/VirtualBox-v7.2.14-111827?style=for-the-badge&labelColor=2563EB&logo=virtualbox&logoColor=white" alt="VirtualBox" />

  <img src="https://img.shields.io/badge/Linux-111827?style=for-the-badge&labelColor=475569&logo=linux&logoColor=white" alt="Linux" />

  <img src="https://img.shields.io/badge/Networking-111827?style=for-the-badge&labelColor=0891B2" alt="Networking" />

  <img src="https://img.shields.io/badge/Penetration%20Testing-111827?style=for-the-badge&labelColor=7C3AED&logo=kalilinux&logoColor=white" alt="Penetration Testing" />

  <img src="https://img.shields.io/badge/Ethical%20Hacking-111827?style=for-the-badge&labelColor=4F46E5&logo=kalilinux&logoColor=white" alt="Ethical Hacking" />

  <img src="https://img.shields.io/badge/Network-10.0.0.0%2F24-111827?style=for-the-badge&labelColor=0891B2" alt="Network" />

  <img src="https://img.shields.io/badge/Virtualization-111827?style=for-the-badge&labelColor=2563EB&logo=virtualbox&logoColor=white" alt="Virtualization" />

  <img src="https://img.shields.io/badge/Networkwalks-111827?style=for-the-badge&labelColor=2563EB" alt="Networkwalks" />

  <img src="https://img.shields.io/badge/Mentor-Waqas%20Karim%20(CCIE)-111827?style=for-the-badge&labelColor=475569" alt="Waqas Karim CCIE" />

  <img src="https://img.shields.io/badge/Developer-Syed%20Bilal%20Ahmed-111827?style=for-the-badge&labelColor=0F766E&logo=github&logoColor=white" alt="Syed Bilal Ahmed" />
</p>
<p align="center">
  <strong
     
  <strong>networkwalks-B082-week1-Cybersecurity-lab-setup</strong>
</p>

<p align="center">
  VirtualBox • Kali Linux • Virtual Networking • Linux Networking
</p>

---
---

## 📋 Table of Contents

1. [Lab Overview]
2. [Lab Environment Specifications]
3. [Lab Architecture]
4. [Phase 01 — Step-by-Step Implementation]
5. [Project Demo]
6. [Key Takeaways & Learnings]
7. [Ethics & Acknowledgments]

---

## 🎯 Lab Overview

The purpose of this project is to construct a **controlled, isolated, and secure cybersecurity lab environment** utilizing Oracle VirtualBox and Kali Linux. Establishing an independent virtual lab ensures a safe framework for practicing penetration testing and network security concepts without risking production systems or unauthorized networks.

This environment acts as the core foundational base for upcoming practical learning modules in:

* Ethical Hacking & VAPT (Vulnerability Assessment and Penetration Testing)
* Advanced Linux Networking and Routing
* Security Automation & Python Scripting
* Threat Analysis and Mitigation Labs

---

## 🖥️ Lab Environment Specifications

| Component | Details |
| --- | --- |
| **Host Operating System** | Windows 11 |
| **Processor** | Intel Core i3 / i5 |
| **Memory (RAM)** | 8 GB – 16 GB |
| **Storage** | 512 GB – 1 TB |
| **Virtualization Platform** | Oracle VirtualBox 7.2.14 |
| **Guest Operating System** | Kali Linux 2026.2 |
| **Network Type** | NAT Network |
| **Network CIDR** | `10.0.0.0/24` |
| **Kali Linux IP Address** | `10.0.0.2/24` |
| **Default Gateway** | `10.0.0.1` |
| **DNS Server** | `8.8.8.8` |

---

## 🏗️ Lab Architecture

```text
Host Machine (Windows 11)
      │
      ▼
Oracle VirtualBox (v7.2.14)
      │
      ▼
NAT Network (10.0.0.0/24)
      │
      ▼
Kali Linux VM (10.0.0.2/24)
      │
      ▼
Isolated Cybersecurity Testing Ground

```

---

## 🚀 Phase 01 — Step-by-Step Implementation

The workflow for Phase 01 is structured into six sequential deployment stages:

### 1️⃣ 7-Zip Installation

* **Action:** Installed 7-Zip to manage and extract compressed virtual machine archives.
* **Objective:** Extract Kali Linux VM files prior to hypervisor import.
* **Status:** ✅ Completed

<img width="1838" height="878" alt="633734948-9ae264c3-6ac4-4186-9119-c63b742e4899" src="https://github.com/user-attachments/assets/567a86e7-5cb9-4b3b-b45d-6633ad649406" />
<img width="570" height="265" alt="633808350-4b6c32b4-e0f5-49a6-832d-8f4e63847b56" src="https://github.com/user-attachments/assets/4c9cd211-c8e9-47c4-935a-2a1d3e1f0fbf" />
<img width="561" height="365" alt="image" src="https://github.com/user-attachments/assets/d33eef88-7a00-4cbd-9fa3-22e3cc0f606c" />


---

### 2️⃣ Oracle VirtualBox Installation

* **Action:** Installed and configured Oracle VirtualBox platform packages.
* **Objective:** Establish the hypervisor layer needed to host target and attacker virtual machines.
* **Status:** ✅ Completed

<img width="1829" height="899" alt="633735623-73042560-7544-4193-9523-544ea40fe796" src="https://github.com/user-attachments/assets/016f3220-3efd-4c22-a053-fa1ea62b049a" />
<img width="1202" height="633" alt="image" src="https://github.com/user-attachments/assets/93ff2714-be59-444e-92cc-3789d9af58ee" />


---

### 3️⃣ NAT Network Configuration

* **Action:** Built a custom isolated NAT Network inside VirtualBox preferences.
* **Objective:** Create a secure network segment for all lab guests with DHCP allocation.
* **Configuration:**
```text
Network Type : NAT Network
Network CIDR : 10.0.0.0/24
DHCP Server  : Enabled

```


* **Status:** ✅ Completed

<img width="956" height="720" alt="image" src="https://github.com/user-attachments/assets/cd382373-4632-4509-b9a9-eaaa259818ab" />


---

### 4️⃣ Kali Linux VM Setup

* **Action:** Downloaded, verified, and imported the Kali Linux virtual appliance into VirtualBox, assigning it to the custom NAT network.
* **Objective:** Deploy the core penetration testing operating system.
* **Configuration:**
```text
Operating System : Kali Linux
Version          : 2026.2
Network Binding  : NatNetwork

```


* **Status:** ✅ Completed

<img width="1272" height="833" alt="image" src="https://github.com/user-attachments/assets/6bbed1ed-8cad-4454-8307-a7520018cbf6" />
<img width="1268" height="725" alt="image" src="https://github.com/user-attachments/assets/8a9cc1d2-1b31-4544-a575-2036faea4438" />


---

### 5️⃣ Kali Linux Network Configuration

* **Action:** Assigned static IP properties to the interface and validated connection reliability.
* **Objective:** Force the VM onto the predetermined lab subnet (`10.0.0.2/24`) and confirm external routing.
* **Configuration:**
```text
IP Address : 10.0.0.2/24
Gateway    : 10.0.0.1
DNS        : 8.8.8.8

```


* **Commands Executed:**
```bash
ifconfig
sudo ifconfig eth0 down
sudo ifconfig eth0 up
ping -c 4 google.com

```


* **Status:** ✅ Completed

<img width="1277" height="798" alt="image" src="https://github.com/user-attachments/assets/29ad616e-6d13-4621-b547-fb6bb1eb1c9c" />
<img width="1262" height="658" alt="image" src="https://github.com/user-attachments/assets/957d33b0-811d-46d8-8046-44e14e1f26ad" />


---

### 6️⃣ VirtualBox Snapshot Configuration

* **Action:** Captured a clean baseline snapshot of the fully set up Kali Linux virtual machine.
* **Objective:** Provide a fast, reliable rollback state in the event of misconfigurations or system corruption during future lab exercises.
* **Status:** ✅ Completed
<img width="1202" height="629" alt="image" src="https://github.com/user-attachments/assets/21d2544a-c1b4-4265-8877-b6e80d510111" />
<img width="1199" height="637" alt="image" src="https://github.com/user-attachments/assets/38c887c8-2890-46b1-9f5e-237d2e1c73a0" />


---

## 🎥 Project Demo

A full walkthrough video of the environment deployment, network mapping, and validation testing:

▶️ **[Watch the Project Demo Video](https://github.com/user-attachments/assets/951e0267-c9e3-40a0-85e6-ecb7daed2ac1)**

---

## 🧠 Key Takeaways & Learnings

* **Virtualization Management:** Practical experience setting up hypervisors and handling virtual machine appliances.
* **Virtual Networking:** Designing custom private segments utilizing NAT networking models.
* **IP Subnetting & Routing:** Managing IPv4 addressing schemes, default gateways, and custom interface scripts in Linux.
* **Disaster Recovery:** Utilizing hypervisor snapshots to safeguard configuration baselines.

---

## 🔐 Ethics & Acknowledgments

* **Scope Statement:** This laboratory setup is built exclusively for **authorized educational purposes, ethical security studies, and controlled testing scenarios**.
* **Mentor Attribution:** Special thanks to **Waqas Karim (CCIE)** for continuous technical mentorship and structural oversight throughout the Networkwalks internship program.

---

### 📊 Phase 01 Progress: **6 / 6 Steps Completed (100%) ✅**

> *🔐 Learn • Practice • Build • Secure*
> **Networkwalks Cybersecurity Internship — Week 01**
