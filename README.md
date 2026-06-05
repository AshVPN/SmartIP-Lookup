<div align="center">

<img src="images/icon128.png" width="80" alt="SmartIP Lookup">

# ⚡ SmartIP Lookup

### The browser extension that sees through the internet


**IP intel · Threat score · V2ray/Xray toolkit · Clean IP scanner · TCP ping · SNI health**

[📥 Chrome](#-chrome) · [🦊 Firefox](#-firefox) · [🔷 Edge](#-edge) · [✨ Features](#-features)

</div>

---

## 🚀 What is this?

SmartIP Lookup is a **free browser extension** that gives you instant deep intelligence on any IP, domain, or V2ray/Xray config — directly from your browser, from **your location**.

Built for **VPN operators, V2ray/Xray users, security researchers, and network engineers**.

No server. No subscription. No data collection. Everything runs locally.

---

## ✨ Features

### 🌍 IP & Domain Lookup
- Auto-detects IPs/domains when you **copy, click, or select** text anywhere
- Full geo: country 🏳️, city, region, ISP, ASN, ZIP, timezone, coordinates
- **4-API waterfall** — works for Cloudflare, Fastly, Akamai, any CDN IP
- Reverse DNS, Google Maps link, country flag

### 🛡️ Threat Intelligence
- **Threat Score 0–100** with animated bar
- Proxy / VPN / Hosting / Mobile detection with badges
- Risk factors: Proxy +35, Datacenter +25, Risky ASN +15, No rDNS +5
- 🟢 CLEAN → 🔵 LOW → 🟡 MODERATE → 🔴 HIGH RISK

### 🔌 TCP Ping & Connectivity
- **TCP-level ping** — like ping.pe / check-host.net but from **your location**
- Min / Avg / Max / Loss% with live animated bars + canvas chart
- DNS check, HTTP reachability, Block detection
- Works for Cloudflare, Fastly, Akamai, any IP or domain

### ⚡ V2ray / Xray Toolkit

**1. Clean IP Scanner**
- 395 IPs across all 16 official Cloudflare CIDR ranges
- Live concurrent probing — up to 400 IPs per scan
- Export clean list in one click

**2. Bulk IP Checker**
- Paste any list → test all at once → sorted by latency

**3. Config Tester** *(the star feature)*
- Supports: `vless://` `vmess://` `trojan://` `ss://` `hysteria2://` `tuic://` + JSON
- Parses ALL fields: protocol, transport, security, SNI, host, path, flow, fingerprint, Reality public key, short ID
- **Handles domain addresses** (e.g. `fr5.niekotin.de:80`) — auto DNS resolves to real IP
- **Port-aware probing** — http:// for port 80/8080/8880, https:// for others
- Probes **3 sections separately**: Server IP + Host domain + SNI
- Each section shows: full geo, ISP, ASN, threat score, CF colo, latency, DNS, block status
- **Built-in TCP ping** button on every probe card — 5 rounds live

**4. Port Scanner** — tests all V2ray ports: 443, 80, 8443, 2053, 2083, 2087, 2096, 8080, 8880

**5. Real IP Finder** — finds origin IP behind Cloudflare via DNS/MX/subdomains/TXT

### 🔒 SNI Health Check
- Verifies SNI routing on target IP
- CF edge colo, CF-seen SNI, match status, CF edge IP

### 📊 "Who's Watching You" Banner
- Slim info bar on every page: flag, server IP, ISP, threat score, health
- Auto-hides (configurable). Per-site dismiss. Excluded sites list.

### 📋 History + ⚙️ Settings
- Full lookup history with search/filter
- Toggle every feature. Live settings — no reload.

---

## 📥 Chrome

1. Download **`SmartIP-Lookup-v6-chrome.zip`** from [Releases](https://github.com/AshVPN/SmartIP-Lookup/releases/latest)
2. Unzip it
3. Chrome → `chrome://extensions` → enable **Developer mode**
4. Click **Load unpacked** → select the unzipped folder
5. Done ✓

---

## 🦊 Firefox

1. Download **`SmartIP-Lookup-v6-firefox.xpi`** from [Releases](https://github.com/AshVPN/SmartIP-Lookup/releases/latest)
2. Firefox → `about:addons` → ⚙️ → **Install Add-on From File**
3. Select the `.xpi` ✓

---

## 🔷 Edge

1. Download **`SmartIP-Lookup-v6-chrome.zip`** from [Releases](https://github.com/AshVPN/SmartIP-Lookup/releases/latest)
2. Unzip it
3. Edge → `edge://extensions` → enable **Developer mode**
4. Click **Load unpacked** → select the unzipped folder ✓

---

## 🛠️ Supported Config Formats

| Format | Example |
|--------|---------|
| VLESS Reality | `vless://uuid@ip:443?security=reality&sni=cf.com&fp=chrome&flow=xtls-rprx-vision#name` |
| VLESS WS | `vless://uuid@domain:80?type=ws&host=cdn.com&path=/vless#name` |
| VMess | `vmess://base64encoded...` |
| Trojan | `trojan://pass@ip:443?type=ws&host=x.com&sni=x.com#name` |
| Shadowsocks | `ss://method:pass@ip:port#name` |
| Hysteria2 | `hysteria2://pass@ip:port?sni=x.com#name` |
| TUIC | `tuic://uuid:pass@ip:port?sni=x.com#name` |
| JSON | Full xray/v2ray outbound config |

---

## 🔒 Privacy

- **Zero data collection** — nothing sent to our servers
- All lookups use public APIs (ipwho.is, ipinfo.io, Google DoH)  
- History stored locally only
- No analytics, no tracking, no ads

---

## 👨‍💻 Made by AshVPN

[![GitHub](https://img.shields.io/badge/GitHub-AshVPN-181717?style=flat-square&logo=github)](https://github.com/AshVPN)

<div align="center">

⭐ **Star this repo if it helped you** ⭐

*Built for the V2ray community. Free forever.*

</div>
