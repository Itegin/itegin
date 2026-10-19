<div align="center">

# Привет, я Itegin Baltabaev 👋

**Linux & Monitoring Engineer**
Москва, Россия · открыт к удалённым инфраструктурным / DevOps-ролям

🇬🇧 [English version](README.md)

[![Сайт](https://img.shields.io/badge/Сайт-itegin-8A2BE2?style=flat-square&logo=readthedocs&logoColor=white)](https://itgnroadmap.duckdns.org:9443/?src=github)
[![Telegram](https://img.shields.io/badge/Telegram-@itegin-26A5E4?style=flat-square&logo=telegram&logoColor=white)](https://t.me/itegin)
[![Email](https://img.shields.io/badge/Email-iteginbt%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:iteginbt@gmail.com)

</div>

---

### Обо мне

Единственный системный администратор в компании на двух площадках: Linux (Debian, Ubuntu, Astra), Windows Server и Proxmox VE. Внедрил мониторинг на Prometheus и Grafana с алертами в Telegram, заявки в Jira и базу знаний в Confluence, перевёл сервисы на Docker и k3s. До этого вёл всю IT-часть офиса на 8 рабочих мест. Занимаюсь мониторингом и разбором инцидентов, а свои сервисы довожу до продакшена сам.

**С чем работаю:**

![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes_(k3s)-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Proxmox](https://img.shields.io/badge/Proxmox-E57000?style=flat-square&logo=proxmox&logoColor=white)
![nginx](https://img.shields.io/badge/nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Jira](https://img.shields.io/badge/Jira-0052CC?style=flat-square&logo=jira&logoColor=white)
![Confluence](https://img.shields.io/badge/Confluence-172B4D?style=flat-square&logo=confluence&logoColor=white)

---

### Проекты

<table>
<tr>
<td width="50%" valign="top">

**[IT-Deck](https://github.com/Itegin/it-deck)** · последний релиз [v0.6.1](https://github.com/Itegin/it-deck/releases/latest)

Старый iPhone становится пультом и веб-камерой для Windows-ПК: живые тайлы, настройка по QR-коду, без сервера и Docker.

`Python` `FastAPI` `WebSocket` `WebRTC` `GitHub Actions`

<img src="assets/it-deck-screenshot.jpg" width="100%" alt="IT-Deck на телефоне">

</td>
<td width="50%" valign="top">

**itegin — личный сайт** *(исходники закрыты)*

Мой сайт-визитка и портфолио, написан с нуля: собственная аутентификация и админка (черновик → публикация), счётчик просмотров без cookies, витрина GitHub, обновляемая по вебхуку. Работает в продакшене на VPS.

`Flask` `SQLite` `Docker Compose` `nginx` `CI: ruff + pytest`

[→ живой сайт](https://itgnroadmap.duckdns.org:9443/?src=github) · [→ репозиторий-витрина](https://github.com/Itegin/pygodevops-guide-showcase)

</td>
</tr>
</table>

---

### Как работает сайт

```mermaid
flowchart LR
    U[Браузер] -->|HTTPS| N[nginx, TLS]
    subgraph VPS
        N --> A[Docker: сайт на Flask]
        A --> DB[(SQLite, volume)]
    end
    DB -. ежедневный бэкап .-> H[Домашний сервер] -. раз в неделю .-> P[Мой ПК]
```

nginx терминирует TLS на VPS и проксирует в контейнер; GitHub Actions при каждом пуше гоняет lint, тесты и сборку Docker-образа. База ежедневно копируется на VPS, затем на домашний сервер (он же тестовый стенд) и дальше на мой ПК.

---

### Ключевое

- Единственный сисадмин на двух площадках компании: Linux, Windows Server, Proxmox VE, сеть, бэкапы, поддержка пользователей
- Внедрил **мониторинг на Prometheus + Grafana с алертами в Telegram**: о сбоях узнаю раньше пользователей
- Завёл **заявки в Jira и базу знаний в Confluence** с инструкциями; перевёл сервисы на **Docker и k3s**
- **IT-Deck**: публичный проект с релизами по тегам, тестами на Linux и Windows и Windows-сборкой `.exe` через CI
- Сам держу **продакшен-сервисы**: этот сайт работает в Docker за nginx + TLS на VPS, с автоматическими бэкапами

---

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Itegin/itegin/output/github-contribution-grid-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Itegin/itegin/output/github-contribution-grid-snake.svg">
  <img alt="contribution snake" src="https://raw.githubusercontent.com/Itegin/itegin/output/github-contribution-grid-snake.svg">
</picture>

<sub>Открыт к удалённым инфраструктурным / DevOps-ролям. Пишите в [Telegram](https://t.me/itegin) или на [iteginbt@gmail.com](mailto:iteginbt@gmail.com).</sub>
