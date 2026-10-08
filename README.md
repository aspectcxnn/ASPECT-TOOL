# ⚡ ASPECT OSINT SUITE ⚡

### Ethical Open Source Intelligence & Security Toolkit

[Features](#-features--modules) • [Installation](#-installation) • [Usage](#-usage) • [Desktop Integration](#-arch--kde-plasma-integration) • [Disclaimer](#-disclaimer)

---

## 📌 Overview

**ASPECT** is an interactive terminal suite that brings open-source intelligence (OSINT) workflows into a unified, lightweight interface. Tailored specifically for Arch Linux and KDE Plasma terminal environments, it features a distinctive neon/cyberpunk aesthetics.

Featuring an intuitive multi-page menu system (`n` / `b`), ASPECT enables quick reconnaissance and information gathering across multiple targets without requiring cumbersome command-line configurations.

---

## 🚀 Features / Modules

ASPECT utilizes a fast, multi-page terminal navigation system:

### 🔍 Page 1: Core OSINT Modules

* **Username Reconnaissance:** Scan for handles and digital footprints across major platforms and networks.
* **Email Intelligence:** Format validation, MX/DNS verification, and identity presence analysis.
* **Domain Investigation:** Comprehensive WHOIS lookup, active DNS record extraction (A, NS, MX, TXT), and host availability.
* **IP Intelligence:** Geolocation data (GeoIP), ASN/ISP details, organizational registry, and open port profiling.
* **Phone Number OSINT:** International E.164 parsing, carrier identification, line type classification, and search dorks.
* **GitHub Profiling:** Developer activity tracking, public repositories, and commit-level insights.
* **Web Analysis & URL Inspection:** Server fingerprinting, security headers audit, redirection tracing, and link risk checks.

### 🎮 Page 2 & 3: Utilities & Integrations

* **Platform Templates:** Schema and pattern testing utilities for target formats.
* **Discord Utilities:** Webhook verification, bot token inspections, and community query utilities.

---

## 🛠️ Installation

### Prerequisites

* Python 3.10+
* Bash shell
* Python virtual environment support (`python3-venv`)

### Quick Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/YOUR_USERNAME/ASPECT-TOOL.git
   cd ASPECT-TOOL
   ```

2. **Grant execution permissions to the launcher:**
   ```bash
   chmod +x run.sh
   ```

3. **Launch ASPECT:**
   ```bash
   ./run.sh
   ```

   > *Note: `run.sh` automatically provisions an isolated Python virtual environment (`venv`) and installs the dependencies from `requirements.txt` on first launch.*

---

## 🖥️ Arch / KDE Plasma Integration

To integrate ASPECT directly into your desktop environment (KDE Application Launcher / KRunner):

1. **Copy the desktop entry to your local applications directory:**
   ```bash
   cp ASPECT.desktop ~/.local/share/applications/
   ```

2. **Dynamically configure the project directory path:**
   ```bash
   sed -i "s|/home/aspect/Projeler/ASPECT-TOOL|$PWD|g" ~/.local/share/applications/ASPECT.desktop
   ```

You can now search for and launch **"ASPECT OSINT Tool"** directly from your application launcher or terminal run-dialog.

---

## 📦 Dependencies

The toolkit is powered by the following core libraries:

* `requests` — Synchronous HTTP client
* `aiohttp` — High-concurrency asynchronous network engine
* `dnspython` — Robust DNS queries and zone checks
* `python-whois` — Domain registry and registrar queries
* `phonenumbers` — International phone number parsing and verification
* `beautifulsoup4` — Web scraping and DOM evaluation

---

## ⚖️ Disclaimer

This tool is designed strictly for **educational purposes, legitimate security research, and authorized penetration testing**. Collecting data against systems or individuals without explicit authorization may violate local and international laws. The developer assumes no responsibility or liability for any misuse or damage caused by this software.
