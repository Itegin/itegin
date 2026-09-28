<div align="center">

# Hi, I'm Itegin 👋

**Network & system administrator, moving into DevOps.**
21 y.o. · Russia/Kazakhstan · Cybersecurity College grad · currently interning while making the switch.

🇷🇺 [Русская версия](README.ru.md)

[![Telegram](https://img.shields.io/badge/Telegram-@itegin-26A5E4?style=flat-square&logo=telegram&logoColor=white)](https://t.me/itegin)
[![Email](https://img.shields.io/badge/Email-iteginbt%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:iteginbt@gmail.com)
[![Resume](https://img.shields.io/badge/Resume-live%20page-8A2BE2?style=flat-square&logo=readthedocs&logoColor=white)](https://itgnroadmap.duckdns.org:9443/resume)

</div>

---

### About

I run my own home server (Proxmox + Debian, containers, reverse proxy, a VPN and CGNAT tunnel to expose it) and I'm working through Python, Go, Linux internals, Docker, CI/CD and IaC in that order — one guided plan, tracked lesson by lesson. Right now I'm interning and pointing that experience at DevOps.

**Currently learning / using:**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=flat-square&logo=ansible&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![nginx](https://img.shields.io/badge/nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Proxmox](https://img.shields.io/badge/Proxmox-E57000?style=flat-square&logo=proxmox&logoColor=white)

---

### Projects

<table>
<tr>
<td width="50%" valign="top">

**[IT-Deck](https://github.com/Itegin/it-deck)**

An old iPhone becomes a Stream Deck for a Windows PC — real-time tiles (mic, volume, VPN, CPU/RAM), one `.exe`, no server, no Docker, connected over the LAN by QR code.

`Python` `WebSocket` `Windows COM` `PWA`

<img src="assets/it-deck-screenshot.jpg" width="100%" alt="IT-Deck running on a phone">

</td>
<td width="50%" valign="top">

**PyGoDevOps-guide** *(source private)*

A self-hosted learning tracker I built for my own Python → Go → DevOps plan: 12 phases, 77 lessons, per-track progress, theory + practice + self-checks. Runs on my home server.

`Flask` `SQLite` `Docker` `nginx` `CI: ruff + pytest`

[→ live site](https://itgnroadmap.duckdns.org:9443/resume)

</td>
</tr>
</table>

---

### Home server

```mermaid
flowchart LR
    U[Browser] -->|HTTPS, TLS| N[nginx]
    N -->|SSH tunnel, CGNAT| S[Debian server]
    S --> D1[Docker: PyGoDevOps-guide]
    S --> D2[Docker: other services]
    D1 --> DB[(SQLite, volume)]
```

Everything self-hosted: Proxmox for virtualization, Debian + Docker Compose for services, nginx terminating TLS, an SSH tunnel to get around CGNAT, GitHub Actions running lint/tests/build on every push.

---

### Highlights

- Built and deployed **two self-hosted web services** (Flask, FastAPI) from scratch, both public over nginx + TLS
- Run a **home server**: Proxmox VE for virtualization, Docker Compose for services, an SSH tunnel to get around CGNAT
- **IT-Deck** — public project, actively maintained, tagged releases with CI-built Windows binaries
- **PyGoDevOps-guide** — own 12-phase / 77-lesson curriculum, working through it lesson by lesson while building the tracker itself
- Wrote my own auth, admin panel (draft → publish), and a cookie-free page-view counter — no frameworks, no ORM, no shortcuts

---

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Itegin/itegin/output/github-contribution-grid-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Itegin/itegin/output/github-contribution-grid-snake.svg">
  <img alt="contribution snake" src="https://raw.githubusercontent.com/Itegin/itegin/output/github-contribution-grid-snake.svg">
</picture>

<sub>Open to remote infrastructure/DevOps roles.</sub>
