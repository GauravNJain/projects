<p align="center">
  <img src="https://github.com/GauravNJain/Netwizard-plusplus/blob/main/imgs/Netwizard%2B%2B%20Banner%20Image.png" alt="NetWizard++ Banner" width="80%">
</p>

# NetWizard++ Toolkit

NetWizard++ is a lightweight, Bash-based **network mapping and pentesting toolkit** designed for fast reconnaissance, subnet analysis, host discovery, and simple visualization using Nmap and Graphviz.

It is intended for **educational purposes, labs, and authorized security testing only**.

---

## ✨ Features

- 📐 **Subnet Calculator**

  <img src="https://github.com/GauravNJain/Netwizard-plusplus/blob/main/imgs/Subnet%20Calculator%20Image.png" alt="NetWizard++ Banner" width="50%">
  
  - Network ID
  - Broadcast address
  - Subnet mask
  - Usable IP range and host count

- 🔍 **Host Discovery**

  <img src="https://github.com/GauravNJain/Netwizard-plusplus/blob/main/imgs/Host%20discovery%20image.png" alt="NetWizard++ Banner" width="50%">
  
  - Ping-scan based live host detection using Nmap

- 📊 **Readable Host Table**

  <img src="https://github.com/GauravNJain/Netwizard-plusplus/blob/main/imgs/readable%20host%20table%20image.png" alt="NetWizard++ Banner" width="50%">
  
  - IP address
  - Hostname (if available)
  - MAC address and vendor (when detected)

- 🗺️ **Network Map Visualization**

  <img src="https://github.com/GauravNJain/Netwizard-plusplus/blob/main/imgs/Network%20Map%20Visualizer%20img.png" alt="NetWizard++ Banner" width="50%">
  
  - ASCII host list
  - Automatically generated PNG network map using Graphviz

- 🛡️ **Pentest Enumeration**

  <img src="https://github.com/GauravNJain/Netwizard-plusplus/blob/main/imgs/Pentest%20Enumeration%20img.png" alt="NetWizard++ Banner" width="50%">
  
  - SYN scan
  - Service/version detection
  - OS detection
  - Output saved for reporting

- 🔔 **New Device Detection**

  <img src="https://github.com/GauravNJain/Netwizard-plusplus/blob/main/imgs/new%20device%20detection%20(baseline%20creation).png" alt="NetWizard++ Banner" width="35%">  <img src="https://github.com/GauravNJain/Netwizard-plusplus/blob/main/imgs/newly%20added%20device%20detection.png" alt="NetWizard++ Banner" width="35%">
  
  - Detects new hosts appearing on a network by comparing scans

---

## 🧠 How Network Mapping Works

NetWizard++ does **not** perform physical topology discovery.

Instead, it:
1. Uses `nmap -sn` to detect live hosts
2. Writes a **Graphviz DOT file** describing relationships between the network and hosts
3. Uses Graphviz (`dot`) to render a **logical host relationship map**

This produces a clean, report-friendly visualization of discovered assets.

---

## 📦 Requirements

NetWizard++ relies on the following tools:

- `bash`
- `nmap`
- `gawk`
- `util-linux`
- `graphviz` (optional, for PNG network maps)

The installer will attempt to install these automatically.

---

## 🚀 Installation

Clone the repository and run the installer:

```bash
git clone https://github.com/GauravNJain/Netwizard-plusplus.git
cd Netwizard-plusplus
sudo bash ./installer.sh
```

---

## 👤 Author

- Developed by Gaurav N Jain

📧 Contact: [LinkedIn Profile](https://www.linkedin.com/in/gauravnjain/)<br>
Github: [repo link](https://github.com/GauravNJain/Netwizard-plusplus/)
