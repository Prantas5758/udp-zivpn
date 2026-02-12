<p align="center">
  <img src="zivpn.png" width="420" alt="ZiVPN UDP Server"/>
</p>

<h1 align="center">ZiVPN UDP Server</h1>

<p align="center">
  Installer & manager untuk menjalankan <b>ZiVPN Tunnel (UDP)</b> di VPS Linux (Debian/Ubuntu).<br/>
  <sub>Auto-detect arsitektur • Auto install binary • Auto systemd • Auto UFW & NAT</sub>
</p>

<p align="center">
  <!-- Repo -->
  <a href="https://github.com/prantas5758/udp-zivpn">
    <img alt="GitHub Repo" src="https://img.shields.io/badge/GitHub-udp--zivpn-181717?logo=github&logoColor=white">
  </a>
  <!-- Release / Downloads / Last Commit -->
  <a href="https://github.com/prantas5758/udp-zivpn/releases">
    <img alt="Release" src="https://img.shields.io/github/v/release/prantas5758/udp-zivpn?display_name=tag&logo=github">
  </a>
  <a href="https://github.com/prantas5758/udp-zivpn/releases">
    <img alt="Downloads" src="https://img.shields.io/github/downloads/prantas5758/udp-zivpn/total?logo=github">
  </a>
  <a href="https://github.com/prantas5758/udp-zivpn/commits/main">
    <img alt="Last Commit" src="https://img.shields.io/github/last-commit/prantas5758/udp-zivpn?logo=github">
  </a>
</p>

<p align="center">
  <img alt="OS" src="https://img.shields.io/badge/OS-Debian%20%7C%20Ubuntu-2b6cb0">
  <img alt="Arch" src="https://img.shields.io/badge/Arch-amd64%20%7C%20arm%20%7C%20arm64-0ea5e9">
  <img alt="Service" src="https://img.shields.io/badge/Service-systemd-10b981">
  <img alt="Firewall" src="https://img.shields.io/badge/Firewall-UFW%20%2B%20NAT-f59e0b">
</p>

---

## 📌 Table of Contents
- [✨ Overview](#-overview)
- [✅ Fitur](#-fitur)
- [🚀 Instalasi](#-instalasi)
  - [Quick Install (Menu Installer)](#quick-install-menu-installer)
  - [Install Release (Auto Verify SHA256)](#install-release-auto-verify-sha256)
- [🧰 Operasional](#-operasional)
- [📸 Screenshots (Menu)](#-screenshots-menu)
- [🖥️ Supported Architecture](#️-supported-architecture)
- [⚙️ Default Configuration](#️-default-configuration)
- [📱 Client App](#-client-app)
- [🧯 Fix & Update](#-fix--update)
- [🧹 Uninstall](#-uninstall)
- [🆘 FAQ](#-faq)
- [🤝 Kontribusi](#-kontribusi)
- [📄 License](#-license)
- [📞 Support](#-support)

---

## ✨ Overview
**ZiVPN UDP Server** menyediakan script installer yang fokus pada kemudahan deploy:
- Instalasi cepat & minim interaksi
- Service stabil (**systemd + auto restart**)
- Firewall & NAT siap pakai
- Menu manager untuk operasional harian

---

## ✅ Fitur
- Auto detect arsitektur VPS (**amd64 / arm / arm64**)
- Auto download & install **binary terbaru**
- Auto setup **systemd service** (`zivpn.service`)
- Auto configure **UFW firewall** & **NAT**
- Apply konfigurasi default (**password: `zi`**)
- Support **Debian / Ubuntu** (minimal OS)
- Opsi mode: **Dual SC** atau **ZiVPN Only**
- Alias command: `menu` → `/usr/local/bin/zivpn-manager`

---

## 🚀 Instalasi

### Quick Install (Menu Installer)
```bash
apt update -y && wget -q https://raw.githubusercontent.com/prantas5758/udp-zivpn/main/install.sh -O /usr/local/bin/install.sh && chmod +x /usr/local/bin/install.sh && /usr/local/bin/install.sh
