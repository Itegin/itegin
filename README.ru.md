<div align="center">

# Привет, я Itegin 👋

**Сетевой и системный администратор, перехожу в DevOps.**
21 год · Россия/Казахстан · выпускник колледжа по кибербезопасности · сейчас на стажировке, параллельно меняю направление.

🇬🇧 [English version](README.md)

[![Telegram](https://img.shields.io/badge/Telegram-@itegin-26A5E4?style=flat-square&logo=telegram&logoColor=white)](https://t.me/itegin)
[![Email](https://img.shields.io/badge/Email-iteginbt%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:iteginbt@gmail.com)
[![Resume](https://img.shields.io/badge/Resume-сайт-8A2BE2?style=flat-square&logo=readthedocs&logoColor=white)](https://itgnroadmap.duckdns.org:9443/resume)

</div>

---

### Обо мне

У меня свой домашний сервер (Proxmox + Debian, контейнеры, reverse proxy, VPN и туннель через CGNAT, чтобы всё это было видно снаружи), и я прохожу Python, Go, основы Linux, Docker, CI/CD и IaC — по порядку, по собственному плану, урок за уроком. Сейчас стажируюсь и разворачиваю этот опыт в сторону DevOps.

**Сейчас изучаю / использую:**

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

### Проекты

<table>
<tr>
<td width="50%" valign="top">

**[IT-Deck](https://github.com/Itegin/it-deck)**

Старый iPhone становится Stream Deck для Windows-ПК: живые тайлы (микрофон, громкость, VPN, CPU/RAM), один `.exe`, без сервера и Docker, подключение по QR-коду в локальной сети.

`Python` `WebSocket` `Windows COM` `PWA`

<img src="assets/it-deck-screenshot.jpg" width="100%" alt="IT-Deck на телефоне">

</td>
<td width="50%" valign="top">

**PyGoDevOps-guide** *(исходники закрыты)*

Самостоятельный трекер обучения, который я написал под свой план Python → Go → DevOps: 12 фаз, 77 уроков, прогресс по трекам, теория + практика + самопроверка. Крутится на домашнем сервере.

`Flask` `SQLite` `Docker` `nginx` `CI: ruff + pytest`

[→ живой сайт](https://itgnroadmap.duckdns.org:9443/resume)

</td>
</tr>
</table>

---

### Домашний сервер

```mermaid
flowchart LR
    U[Браузер] -->|HTTPS, TLS| N[nginx]
    N -->|SSH-туннель, CGNAT| S[Сервер Debian]
    S --> D1[Docker: PyGoDevOps-guide]
    S --> D2[Docker: другие сервисы]
    D1 --> DB[(SQLite, volume)]
```

Всё на самостоятельном хостинге: Proxmox для виртуализации, Debian + Docker Compose для сервисов, nginx терминирует TLS, SSH-туннель обходит CGNAT, GitHub Actions гоняет lint/тесты/сборку при каждом пуше.

---

<details>
<summary><b>План обучения</b> (Python → Go → DevOps, 12 фаз)</summary>
<br>

- [x] Основы Python
- [x] Linux и основы сетей
- [ ] Основы Go
- [ ] Docker и контейнеры
- [ ] CI/CD пайплайны
- [ ] Управление конфигурацией (Ansible)
- [ ] Infrastructure as Code (Terraform)
- [ ] Kubernetes / k3s
- [ ] Мониторинг и observability
- [ ] Основы облаков
- [ ] Security hardening
- [ ] Итоговый проект

Полный трекер (исходники закрыты, прогресс публичный): [itgnroadmap.duckdns.org:9443/resume](https://itgnroadmap.duckdns.org:9443/resume)

</details>

---

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Itegin/itegin/output/github-contribution-grid-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Itegin/itegin/output/github-contribution-grid-snake.svg">
  <img alt="contribution snake" src="https://raw.githubusercontent.com/Itegin/itegin/output/github-contribution-grid-snake.svg">
</picture>

<sub>Открыт к удалённым инфраструктурным/DevOps-ролям.</sub>
