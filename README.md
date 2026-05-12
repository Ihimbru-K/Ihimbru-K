<div align="center">

```
╔══════════════════════════════════════════════════════════╗
║  Building software for real-world constraints,           ║
║  not ideal conditions.                                   ║
╚══════════════════════════════════════════════════════════╝
```

# Ihimbru Kanyimi

**Full-Stack Engineer · Mobile-First Systems · Emerging Market Infrastructure**

Bamenda, Cameroon — where load shedding is real, bandwidth is a luxury,  
and users still need software that works.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/ihimbru-kanyimi-46a973227)
[![Email](https://img.shields.io/badge/kanihims25@gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:kanihims25@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Ihimbru-K)
[![HackerRank](https://img.shields.io/badge/HackerRank-2EC866?style=flat-square&logo=hackerrank&logoColor=white)](https://www.hackerrank.com/ihimbrukanyimi)

</div>

---

## Who I Am

I'm a Computer Engineer building production systems for markets that most engineers design around — not for.

No stable internet. No AWS data centers nearby. Users on 3G who can't retry a failed request. Landlords who don't trust apps. Doctors serving patients who've never used telemedicine. That's my normal.

My work sits at the intersection of **mobile-first architecture**, **constrained infrastructure**, and **real operational problems**: property management for Cameroonian landlords, telemedicine for sub-Saharan clinics, biometric exam systems for universities, and church reporting platforms for distributed organizations. These aren't demos. They're deployed or in active use.

I run a small tech startup. I care deeply about system design, clean APIs, and shipping things that actually hold up.

---

## Projects

### 🏥 SheyDoc — Telemedicine for Low-Bandwidth Africa
> *Flutter · FastAPI · Firebase · Stream Video SDK · Appwrite*

A doctor-patient telemedicine platform built for environments where video calls drop, reconnections are frequent, and users can't afford to restart a consultation.

**The hard engineering problems:**
- Adaptive video quality caps for 3G/unstable networks with live reconnecting banners
- Join-window enforcement logic so appointments don't bleed into each other
- Voice notes + reply-to tagging in chat, with FCM foreground listener reliability fixes
- Doctor vs. patient role separation inside shared video call screens
- Appwrite + Firebase dual-backend without coupling either to the core domain

**What makes it real:** designed for Cameroon-specific network conditions, not ideal conditions.

🔗 [GitHub Profile](https://github.com/Ihimbru-K)

---

### ⛪ CellTrack — Church Cell Group Reporting Platform
> *FastAPI · PostgreSQL (Neon.tech) · SQLAlchemy Async ORM · JWT · Flutter*

Built for BLW Cameroon Zone B — a multi-level distributed church organization covering regions, zones, fellowships, senior cells, and individual cells — with hundreds of reporting units.

**The hard engineering problems:**
- Hierarchical data model with circular FK dependencies, resolved cleanly
- Full async SQLAlchemy ORM with asyncpg SSL-compatible connection strings on Neon
- Pydantic V2 migration and enum mismatch resolution across the model layer
- Swagger JWT injection for development auth without breaking production flow
- Seed script covering the full BLW Zone B org hierarchy — production-ready from day one

**What makes it real:** live client, real organizational hierarchy, no mocked data.

---

### 🏠 Propti (TRMS) — Tenant & Rent Management for Cameroonian Landlords
> *Flutter · FastAPI · PostgreSQL · Firebase*

Property management built for a market that runs on trust, WhatsApp, and cash. Not for SaaS-native users.

**The hard engineering problems:**
- In-app tenancy agreement generation with lawyer-drafted templates and digital signature capture
- PDF generation shareable directly over WhatsApp (how landlords actually operate)
- Partial payment tracking, overdue cycle management, and rent receipt generation
- Freemium monetization with per-agreement fees — matching how local landlords think about value
- Multi-tenant backend architecture handling multiple properties per landlord

**What makes it real:** built for Bamenda landlord psychology, not a generic CRUD rental app.

🔗 [Propti Backend](https://github.com/Propti-app/Propti_backend)

---

### 🎓 Authentikate — Biometric Exam Attendance for Universities
> *Flutter · FastAPI · PostgreSQL · Firebase · JWT*

Exam impersonation (known locally as "ghost writing") is a systemic problem in Cameroonian state universities. Authentikate uses fingerprint verification to tie a student's identity to their exam session — no hardware readers required beyond a mobile device.

**The hard engineering problems:**
- Fingerprint-based identity verification in a mobile-first, offline-tolerant flow
- Role-based access control across student, invigilator, and admin tiers
- Session and department management at institutional scale
- Attendance reporting with audit trails that satisfy administrative requirements

**What makes it real:** addresses an actual institutional failure mode, not a manufactured use case.

🔗 [Repository](https://github.com/Ihimbru-K)

---

## Technical Stack

```
Languages      Python · Dart · TypeScript · Java
Mobile         Flutter (primary — production apps shipped)
Backend        FastAPI · Spring Boot · Node.js
Databases      PostgreSQL · Firebase Firestore
ORM/Query      SQLAlchemy (async) · asyncpg
Auth           JWT · Firebase Auth · Appwrite Auth
Real-time      Stream Video SDK · FCM · WebSockets
Cloud          Render · Neon.tech · Firebase · Appwrite
DevOps         Docker · Git · GitHub Actions
Other          Pydantic V2 · REST API design · PDF generation
```

**Strongest in:** FastAPI + PostgreSQL backend systems · Flutter mobile · API architecture · systems that survive bad networks

---

## Engineering Philosophy

> **KISS first. Complexity is a cost, not a feature.**

I've debugged circular FK dependencies at midnight. I've chased asyncpg SSL errors across three deployment environments. I've shipped features to users who told me the old version was fine and they'd rather not update.

Real software has edges. My job is to find them before users do, build around the actual constraints (not the assumed ones), and ship things that hold up when conditions aren't ideal — which in my context, is always.

---

## Currently

- 🔨 Shipping SheyDoc to doctors and patients across Cameroon
- 📐 Hardening Propti's tenancy agreement and monetization flow
- 🌱 Building a startup internship pipeline from NAHPI Computer Engineering
- 📖 Reading: whatever helps me think more clearly about systems and people

---

## Open To

Freelance contracts · Technical consulting · Remote engineering roles · Collaborations on health-tech, fintech, or civic infrastructure in emerging markets

---

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=ihimbru-k&show_icons=true&theme=default&hide_border=true&include_all_commits=true&count_private=true&title_color=0e75b6&icon_color=0e75b6" height="160"/>
<img src="https://streak-stats.demolab.com/?user=ihimbru-k&hide_border=true&theme=default&stroke=0e75b6&ring=0e75b6&currStreakLabel=0e75b6" height="160"/>

</div>

---

<div align="center">

*Bamenda, Cameroon · Open to remote · Building for the world that exists, not the one in the docs*

</div>
