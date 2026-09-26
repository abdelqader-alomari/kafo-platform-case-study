<div align="center">

<img src="./assets/cover.svg" alt="Kafo Platform case study" width="100%"/>

[![Live](https://img.shields.io/badge/Live-kafo.team-22c55e?style=for-the-badge&logo=googlechrome&logoColor=white)](https://kafo.team) ![Source](https://img.shields.io/badge/Source-private-64748b?style=for-the-badge&logo=lock&logoColor=white)

</div>

> 🔒 **The source code is private** (production / client work). This repository is a case study: what the product does, how it is built, and my role. A code walkthrough is available on request: [abdelqader.pro](https://abdelqader.pro) · [LinkedIn](https://www.linkedin.com/in/abdelqader-al-omari/).

## Overview
Kafo is a non-profit youth team in Amman (founded 2018) offering free training, dialogue sessions and volunteering across
Jordan and the Arab world. I designed and built its whole digital ecosystem: every product below runs in production.

| Product | What it does |
|---|---|
| 🌱 **Main platform** ([kafo.team](https://kafo.team)) | Opportunities directory, blog, archive, member accounts |
| 📚 **Digital library** ([library.kafo.team](https://library.kafo.team)) | Free books by category, reading, community summaries; Laravel 12 + Inertia + React with **SSR** for speed and SEO |
| 🤝 **Recruitment** ([join.kafo.team](https://join.kafo.team)) | Applications for the four volunteer committees |
| 🎥 **Meetings** | Secure self-hosted video meetings for the team |
| ✅ **Tasks** | Task & committee management |
| ✉️ **Mail · Drive** | Webmail on real IMAP/SMTP (Laravel + Livewire) and file storage |

## Architecture

```mermaid
flowchart TB
    U([👥 Volunteers & public]) --> CDN[⚡ CDN + TLS]
    CDN --> M[🌱 Main platform]
    CDN --> L[📚 Library<br/>Inertia + React SSR]
    CDN --> J[🤝 Recruitment]
    CDN --> T[✅ Tasks]
    CDN --> E[✉️ Webmail]
    CDN --> V[🎥 Meetings]
    M & L & J & T --> DB[(🗄️ MySQL)]
    E --> IMAP[📮 IMAP / SMTP]
    OPS[⚙️ Automated deploys · backups · monitoring] -.-> M & L & J & T & E
```

## Highlights
- **RTL-first** Arabic interfaces with careful typography, responsive on every screen
- The library is **server-side rendered** (Inertia SSR) so pages are fast and indexable
- All products deploy automatically from private repositories, with encrypted backups and monitoring

## My role
Product design and full-stack development of every product, plus the infrastructure they run on.

## Tech
![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white) ![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black) ![Inertia](https://img.shields.io/badge/Inertia-9553E9?style=for-the-badge&logo=inertia&logoColor=white) ![Livewire](https://img.shields.io/badge/Livewire-4E56A6?style=for-the-badge&logo=livewire&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white) ![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)

## Screenshots

<p align="center"><img src="./assets/kafo-team.jpg" alt="kafo.team: opportunities, blog and member accounts" width="100%"/><br/><sub>kafo.team: opportunities, blog and member accounts</sub></p>

<p align="center"><img src="./assets/library.jpg" alt="Digital library: browse, read and summarize books (server-side rendered)" width="100%"/><br/><sub>Digital library: browse, read and summarize books (server-side rendered)</sub></p>

<p align="center"><img src="./assets/join.jpg" alt="Recruitment site for the team&#x27;s four committees" width="100%"/><br/><sub>Recruitment site for the team&#x27;s four committees</sub></p>


---

<div align="center">

**Built by [Abdelqader Al-Omari](https://github.com/abdelqader-alomari)** · Senior Full-Stack Engineer · AI & Enterprise Solutions

[![Portfolio](https://img.shields.io/badge/abdelqader.pro-8b5cf6?style=for-the-badge&logo=googlechrome&logoColor=white)](https://abdelqader.pro) [![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abdelqader-al-omari/) [![More work](https://img.shields.io/badge/More_case_studies-111827?style=for-the-badge&logo=github&logoColor=white)](https://github.com/abdelqader-alomari)

</div>
