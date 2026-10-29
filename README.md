# Cybersecurity Lab Environment Setup
### Building an isolated virtual lab for penetration testing and ethical hacking practice

---

## 📌 Project Overview

In this project, I set up a virtual cybersecurity and penetration-testing laboratory using **VirtualBox** and **Kali Linux**.

I configured the lab on a private virtual network (NAT Network) so that I can add more machines later and use them as targets for authorized security testing.

---

## 🎯 Objectives

My objectives for this project were to:

- Install VirtualBox.
- Create a private NAT Network for my lab.
- Import and run Kali Linux as a virtual machine.
- Verify the IP address of my Kali VM.
- Check network connectivity and DNS resolution.
- Verify that Nmap is installed and working.
- Document the complete setup process.

---

## 🛡️ Purpose of the Lab

I built this lab as an isolated and controlled environment for cybersecurity learning and authorized security testing, such as:

- Network reconnaissance
- Port scanning
- Vulnerability assessment
- Packet analysis
- Web security testing
- Security-tool experimentation

> ⚠️ **Important:** I will only use this laboratory on systems that I own or have explicit permission to test. I will not use the lab or its tools to attack unauthorized systems.

---

## ⚙️ Lab Configuration

| 🧩 Component | ⚙️ Configuration |
|---|---|
| 🖥️ Host OS | Windows |
| 🧰 Hypervisor | Oracle VirtualBox |
| 🐉 Security OS | Kali Linux 2026.3 (`kali-linux-2026.3-virtualbox-amd64`) |
| 💽 VM Name | My Fresh Kali Linux |
| 🌐 Virtual Network | NAT Network (`NatNetwork`) |
| 📡 Network Address | 10.0.0.0/24 |
| 🐧 Kali IP Address | 10.0.0.2/24 |
| 🚪 Default Gateway | 10.0.0.1 |
| 🌍 DNS Server | 8.8.8.8 |

---

## 🪜 Lab Setup Procedure

### Step 1. Install VirtualBox
I installed Oracle VirtualBox as my hypervisor. The screenshot below shows VirtualBox Manager ready to use.

![VirtualBox Manager](images/01-virtualbox-manager.png)

### Step 2. Create the NAT Network
I created a dedicated NAT Network in VirtualBox under **NAT Networks**.

**My configuration:**
- Name: `NatNetwork`
- IPv4 Prefix: `10.0.0.0/24`
- DHCP: Enabled
- IPv6: Disabled

![NAT Network Configuration](images/02-nat-network.png)
