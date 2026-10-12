# 🛡️ DBA Offline Assistant · MSSQL DBA Console (Enterprise v7)

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Zero Dependencies](https://img.shields.io/badge/Dependencies-0%20(Pure%20HTML5%2FJS)-success.svg)](#-zero-dependencies--100-offline)
[![Air-Gapped Ready](https://img.shields.io/badge/Environment-Air--Gapped%20%26%20Offline%20Ready-brightgreen.svg)](#-why-dba-offline-assistant)
[![Queries & Playbooks](https://img.shields.io/badge/Built--in%20Queries-267%2B%20in%2023%20Topics-orange.svg)](#-23-comprehensive-dba-domains)
[![Bilingual](https://img.shields.io/badge/Bilingual-English%20%7C%20%D9%81%D8%A7%D8%B1%D8%B3%DB%8C-blueviolet.svg)](#-bilingual-support--راهنمای-فارسی)
[![Themes](https://img.shields.io/badge/Themes-12%20Pro%20Themes-informational.svg)](#-12-professional-themes)

> **The Ultimate Air-Gapped Tactical Cockpit & Operational Runbook for Microsoft SQL Server DBAs, SREs, and DevOps Engineers.**  
> Zero installation. Zero internet required. Pure client-side performance.

---

## ⚡ Live Demo & Quick Launch

- 🌐 **Live Web App:** [https://lilarmn.github.io/dba-offline-assistant/](https://lilarmn.github.io/dba-offline-assistant/)
- 💻 **Offline Use:** Download `index.html` (or `mssql-dba-console.html`) and double-click to launch in any modern browser on any OS.

---

## 🎯 Why DBA Offline Assistant?

In production banking clusters, hospital health systems, government datacenters, and secure corporate VPCs, **internet access is strictly blocked**. When a critical **P1 outage**, severe deadlocking storm, or high-CPU freeze strikes:

- ❌ You **cannot Google** or look up documentation online.
- ❌ You **cannot risk running unverified, untested scripts** from random websites.
- ❌ You **cannot wait** for slow corporate approvals to install heavy diagnostic suites.
- ❌ Junior DBAs and on-call engineers may run a query without knowing **how to interpret the results** or **what metric threshold represents an emergency**.

**DBA Offline Assistant solves this entirely.** It delivers a full-featured, zero-dependency, single-file interactive console containing **267+ battle-tested scripts**, **guided playbooks**, and **threshold benchmarks** in both **English and Persian (فارسی)** directly to your air-gapped jump box or workstation.

---

## ✨ Key Features & Capabilities

### 🔒 100% Air-Gapped & Zero Dependencies
- Single portable `.html` file with embedded styling, vector icons, and script logic.
- **No Node.js, no Python, no npm build, no CDN dependencies, no backend server**.
- Compliant with strict security environments (PCI-DSS, HIPAA, SOC 2, ISO 27001).
- Runs instantly in Chrome, Edge, Firefox, Safari, or Brave.

### 🛡️ Production Safety Guard & Risk Classification
Every single query is labeled with a strict, color-coded operational risk badge:
- 🟢 **Read-Only**: Zero modification or locking impact; 100% safe to run on live high-traffic production.
- 🟡 **Caution**: Lightweight configuration queries, plan cache resets, or operations that may incur measurable I/O or memory overhead.
- 🔴 **Destructive / High-Impact**: Commands that drop objects, terminate sessions (`KILL`), or modify instance-level configurations.
- **Environment Context Strip**: Switch between **PROD**, **STAGING**, and **DR** environments with warning accents to stay constantly aware of target risk.

### 🔄 Dynamic Placeholder Replacement
Stop tedious manual find-and-replace! Type your `{db}`, `{schema}`, or `{table}` in the interactive top replacement bar, and **all 267+ queries update in real-time**. Copy the code or export it directly populated with your actual database and table names.

### 📘 Step-by-Step Tactical Playbooks
Includes visual troubleshooting runbooks for common operational emergencies:
- Incident response workflows
- AlwaysOn Availability Group failover procedures
- Model database default assignment repair
- High-severity latency triage

### 🌍 Bilingual Diagnostics (English + فارسی)
Every single query includes two vital operational guidance sections:
1. **When to use / چه زمانی استفاده کنیم**: The exact symptom or alert that calls for this script.
2. **How to read results & Thresholds / نحوه تحلیل نتایج و آستانه‌ها**: Concrete thresholds (e.g., *What wait time is acceptable?*, *When does VLF count indicate severe log stagnation?*, *What disk latency requires storage escalation?*).

### 🎨 12 Tailored Pro Themes
Designed for prolonged operational shifts and high-stress incident rooms:
| Theme | Description | Theme | Description |
|---|---|---|---|
| 🌌 **Midnight** | Default dark operations cockpit | 🏢 **Light** | Crisp high-contrast day mode |
| 🪨 **Graphite** | Neutral slate dark | ⚓ **Navy** | Deep enterprise blue |
| 🧛 **Dracula** | Vampire neon purple & pastel | 🟢 **Monokai** | Cyber neon high-contrast |
| ❄️ **Nord** | Arctic frost palette | ⚛️ **One Dark** | Classic Atom editor theme |
| 🍎 **macOS** | Sonoma clean desktop styling | 🐧 **GNOME** | Ubuntu Yaru modern styling |
| ⛩️ **Omarchy** | Arch Linux & Tokyo Night aesthetic | 💾 **Windows 1.0** | 1985 classic retro computing |

### ⚡ Power-User Keyboard & Productivity Features
- 🚀 **Command Palette (`Ctrl+K`)**: Rapidly search queries, switch categories, or run commands.
- 🔍 **Instant Search (`/`)**: Real-time filtering across titles, tags, and raw T-SQL code.
- 🗂️ **Drag & Drop Import**: Drop any `.sql` file anywhere onto the page to immediately add it to your local library.
- 💾 **Local-First Persistence**: Custom additions, edits, and favorites are automatically persisted in browser `localStorage`.
- 📤 **Export & Backup**: Export your full customized library as **JSON** or generate a complete **Markdown Runbook** with one click.
- 🔲 **Dense View**: Compact layout mode for ultra-dense monitor setups.

---

## 📚 23 Comprehensive DBA Domains

The library ships out-of-the-box with **267+ ready-to-run queries & playbooks** organized across 23 essential administrative areas:

| # | Topic Domain | Typical Use Cases |
|:---:|---|---|
| 1 | **General Queries** | Instance versions, server edition, uptime, system dates, and quick metadata |
| 2 | **Performance & Wait Stats** | Top waits (`PAGEIOLATCH`, `CXPACKET`, `SOS_SCHEDULER_YIELD`), signal vs resource wait ratio |
| 3 | **Locks & Blocking** | Head-blocker detection, lead blocking chains, lock escalation, blocked process report |
| 4 | **Index Maintenance** | High fragmentation detection, missing index impact recommendations, unused indexes |
| 5 | **Backup & Restore** | Backup history, differential/log backup validation, recovery time verification |
| 6 | **TempDB** | Space usage by session, internal object allocation, version store contention |
| 7 | **Query Store** | Regressed queries, highest duration plans, forced execution plans, plan regression triage |
| 8 | **Security & Logins** | Orphaned users, elevated privileges, `sysadmin` audits, default DB `model` bug mitigation |
| 9 | **Jobs & Agent** | Failed jobs in last 24h, currently executing SQL agent jobs, schedule conflicts |
| 10 | **AlwaysOn / Replication** | AG replica health, redo thread backlog, synchronization latency, failover status |
| 11 | **Disk, IO & Files** | Latency per database file (`num_of_reads`, `io_stall`), filegroup free space, growth settings |
| 12 | **Server & Instance Info** | Hardware resources, CPU configuration, hyperthreading, NUMA node topology, service accounts |
| 13 | **Log & Recovery** | Virtual Log File (VLF) count, log reuse wait reasons, transaction log growth diagnostics |
| 14 | **Useful DMVs** | Core system dynamic management views, execution statistics, connection audits |
| 15 | **Memory & Resource Governor** | Buffer cache hit ratio, page life expectancy (PLE), memory clerks, workload group quotas |
| 16 | **Statistics** | Stale / outdated statistics detection, modification counters, histogram health |
| 17 | **Object Inventory & Health** | Table row counts, partitioned table distributions, compression status, data types |
| 18 | **Windows Server (CMD / PS)** | OS-level diagnostics: PowerShell storage checks, cluster logs, event log scrapers |
| 19 | **Network Troubleshooting** | Client-to-server connectivity, port 1433 validation, DNS cache flush, socket states |
| 20 | **Query Templates** | Rapid `{db}`, `{schema}`, `{table}` parameterized diagnostic scripts |
| 21 | **Ola Hallengren** | Standardized execution wrappers for Index Optimize, Database Backup, and Integrity Check |
| 22 | **SQL Incident Log Collector** | Emergency diagnostic data scraper for post-mortem analysis and Sev-1 incidents |
| 23 | **Best Practices** | Cluster and standalone best practices, configuration guards, trace flags |

---

## ⌨️ Keyboard Shortcuts Reference

| Shortcut | Action |
|---|---|
| <kbd>Ctrl</kbd> + <kbd>K</kbd> | Open Command Palette / Global Switcher |
| <kbd>/</kbd> | Instantly focus the Search bar |
| <kbd>?</kbd> | Open Keyboard Shortcuts modal |
| <kbd>Ctrl</kbd> + <kbd>Enter</kbd> | Save query while inside the Query / Playbook editor |
| <kbd>Esc</kbd> | Close active modal, palette, or clear current search filter |
| **Drag & Drop** | Drop any `.sql` file anywhere on screen to import into library |

---

## 🇮🇷 راهنمای فارسی | دستیار آفلاین مدیران پایگاه داده (DBA)

این ابزار یک **کنسول جامع، تعاملی و ۱۰۰٪ آفلاین** برای مدیران پایگاه داده SQL Server، مهندسان SRE و تیم‌های پشتیبانی است:

- 📶 **کاملاً مستقل از اینترنت (Air-Gapped):** نیازی به اینترنت، Node.js، پایتون یا نصب هیچ بسته‌ای ندارد. تنها با یک فایل HTML در تمامی مرورگرها اجرا می‌شود.
- 🔍 **بیش از ۲۶۷ کوئری و سناریوی عملیاتی در ۲۳ موضوع حیاتی:** از تحلیل ویت‌استیت‌ها (Wait Stats) و بلاکینگ‌ها گرفته تا نگهداری ایندکس‌ها، تنظیمات TempDB، کلاسترهای AlwaysOn، کوئری استور و اسکریپت‌های اولا هالنگرین (Ola Hallengren).
- 💡 **تحلیل دقیق و آستانه‌های بحرانی (Thresholds):** هر کوئری دارای دو بخش توضیحات تخصصی به زبان فارسی است:
  - **چه زمانی استفاده کنیم؟** (تشخیص سریع در زمان بروز حادثه)
  - **نحوه خواندن نتایج و آستانه‌ها** (راهنمای اعداد طبیعی در برابر اعدادی که نشان‌دهنده فاجعه هستند)
- ⚠️ **سطوح ایمنی عملیاتی (Risk Levels):** علامت‌گذاری صریح کوئری‌ها با برچسب‌های `Read-Only` (کاملاً امن برای پروداکشن)، `Caution` (نیازمند دقت) و `Destructive` (دستورات حذفی یا تغییر پیکربندی).
- 🔄 **جایگزینی هوشمند پارامترها:** با وارد کردن نام دیتابیس، اسکیما و جدول در نوار بالایی، تمامی کوئری‌ها به صورت لحظه‌ای با نام‌های واقعی شما تنظیم می‌شوند.
- 🎨 **۱۲ پوسته جذاب:** پوسته‌های تاریک حرفه‌ای (Midnight, Graphite, Navy, Dracula, Nord, OneDark, Monokai) به همراه حالت روشن و پوسته‌های نوستالژیک.

---

## 🚀 Getting Started

### Method 1: Instant Browser Launch (Recommended)
1. Clone or download this repository:
   ```bash
   git clone https://github.com/Lilarmn/dba-offline-assistant.git
   ```
2. Double-click `index.html` (or `mssql-dba-console.html`).
3. You are ready! No build step, no npm, no background process.

### Method 2: Single-File Download
Simply download `index.html` directly onto a USB drive or secure jump-host and open it in any browser.

### Method 3: GitHub Pages
Visit [https://lilarmn.github.io/dba-offline-assistant/](https://lilarmn.github.io/dba-offline-assistant/) for an instant online preview.

---

## 🤝 Contributing

Contributions, bug fixes, and new diagnostic playbooks are welcome!
1. Fork the Project.
2. Create your Feature Branch (`git checkout -b feature/NewDiagnosticQuery`).
3. Commit your Changes (`git commit -m 'Add AlwaysOn redo rate diagnostic'`).
4. Push to the Branch (`git push origin feature/NewDiagnosticQuery`).
5. Open a Pull Request.

---

## 📄 License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for more details.

---

<p align="center">
  <b>Built with ❤️ for Database Administrators worldwide.</b><br>
  <i>If this tool saved your production cluster during an incident, please give it a ⭐️ on GitHub!</i>
</p>
