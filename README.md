






<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,100:302b63&height=180&section=header&text=Ihimbru%20Kanyimi&fontSize=48&fontColor=ffffff&fontAlignY=52&desc=systems%20engineer%20%C2%B7%20infrastructure%20architect%20%C2%B7%%C2%B7%20%2C%20&descSize=13&descAlignY=72&descColor=888888" width="100%"/>
</div>

<br/>

<div align="center">

```
I engineer operational systems end-to-end.

```

</div>

<br/>

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/ihimbru-kanyimi-46a973227)
[![Email](https://img.shields.io/badge/Gmail-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:kanihims25@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Ihimbru-K)

</div>

---

## engineering approach

> I architect systems, Full ownership: The hard problems are in the architecture, not the UI.

---

## systems & infrastructure

| domain | focus |
|--------|-------|
| **offline-first architectures** | conflict resolution, eventual consistency, deterministic sync |
| **institutional-scale systems** | role-based access control, audit trails, compliance constraints |
| **low-bandwidth optimization** | smart caching, progressive data loading, graceful degradation |
| **realtime coordination** | event-driven backends, websocket infrastructure, presence tracking |
| **hardware integration** | biometric systems, scanner drivers, device constraints |
| **payment infrastructure** | reconciliation, multi-provider SDKs, transaction integrity |

---

## projects

### Authentikate : Biometric Institutional Infrastructure

**Status:** Live pilot University of Bamenda (30k+ students)

**System overview:**
Offline-first biometric attendance system designed for exam-hall environments with unreliable connectivity. Flutter clients store attendance locally during exams and synchronize with a FastAPI backend when connectivity returns. Fingerprint capture is handled via ZK-Teco Live 20R devices integrated at the hardware layer. Access is strictly role-based (admin, proctor, student) enforced through JWT-secured APIs.

**Engineering focus:**
- Offline-first attendance capture with later synchronization
- Conflict-safe syncing when multiple devices report overlapping sessions
- Biometric hardware integration in constrained environments
- Audit-safe attendance tracking for institutional use

**Repository:** [Frontend](https://github.com/Ihimbru-K/Authentikate_shipping_frontend) · [Backend](https://github.com/Ihimbru-K/Authentikate_shipping_backend)

---

### SheyDoc : Telemedicine Infrastructure for Low-Connectivity Regions

**Status:** In development targeting underserved healthcare access in Cameroon

**System overview:**
Lightweight telemedicine platform built for unstable connectivity environments. Flutter client supports offline medical records and deferred synchronization. Backend coordinates consultations and notification delivery via FastAPI, with Firebase/Appwrite handling media under bandwidth constraints. FCM is primary notification channel with SMS fallback where connectivity is unreliable.

**Engineering focus:**
- Offline-capable patient records with delayed sync
- Low-bandwidth video/document handling strategies
- Reliable appointment coordination under unstable networks
- Multi-channel notification fallback (FCM + SMS)

**Repository:** [Backend](https://github.com/Sheydocc/sheydoc_backend) · [Frontend](https://github.com/Sheydocc/sheydoc_app)

---

### Propti: Rent & Tenant Management Infrastructure

**Status:** Community testing

**System overview:**
Digital replacement for informal rental workflows. Tenants and landlords interact via Flutter clients connected to a FastAPI backend managing payments, leases, and documents. Payments integrate MTN Mobile Money and Orange Money with reconciliation logic for failed or delayed transactions. Documents are versioned and tracked through a PostgreSQL schema designed for multi-tenant isolation.

**Engineering focus:**
- Payment reconciliation across unreliable mobile money APIs
- Offline-capable lease agreement signing and sync
- Document versioning with audit tracking
- Multi-tenant data isolation at database level

**Repository:** [Backend](https://github.com/Propti-app/Propti_backend)

---

### Cellytics: Cell Reporting & Analytics Platform

**Status:** Production analytics infrastructure

**System overview:**
Distributed reporting system that aggregates structured reports into a central analytics pipeline. Designed for hierarchical organizations requiring visibility across multiple reporting levels. Backend processes event-based inputs into queryable datasets powering real-time dashboards.

**Engineering focus:**
- Event ingestion from distributed sources
- Time-based aggregation for reporting consistency
- Real-time dashboard queries
- Data integrity across hierarchical reporting flows

**Link:** [Live link](https://cellytics-backend.vercel.app/)


---

## technical stack

```
languages      →   Dart · Python · TypeScript · SQL
Frontend       →   NextJs · Tailwind CSS · TypeScript ·
mobile         →   Flutter (Android/iOS)
backend        →   FastAPI (async Python) · Spring Boot · Node.js
data           →   PostgreSQL (schema design, migrations)
                   Firebase/Appwrite (media, realtime), Neon
infrastructure →   Docker · Render · Neon · GitHub Actions
realtime       →   WebSockets · Firebase Realtime · Appwrite
integrations   →   Biometric scanners (ZK-Teco)
                   Payment APIs (MTN, Orange, Stripe)
                   FCM · SMS fallbacks
```

---

## what matters to me

- Architecture that survives low-bandwidth reality
- Database design that handles institutional complexity
- Deployment thinking from day one
- Understanding hardware & device constraints
- Operations-first mentality





<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Ihimbru-K&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true&title_color=7B77F5&icon_color=7B77F5" height="165"/>
&nbsp;
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Ihimbru-K&layout=compact&theme=tokyonight&hide_border=true&title_color=7B77F5" height="165"/>

</div>

<br/>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:302b63,100:0f0c29&height=120&section=footer&text=systems%20engineer%20%2F%20infrastructure%20architect&fontSize=16&fontColor=666666&fontAlignY=65" width="100%"/>
</div>














<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,100:302b63&height=180&section=header&text=Ihimbru%20Kanyimi&fontSize=48&fontColor=ffffff&fontAlignY=52&desc=systems%20engineer%20%C2%B7%20infrastructure%20architect%20%C2%B7%20offline-first%20%C2%B7%20bamenda%2C%20cameroon&descSize=13&descAlignY=72&descColor=888888" width="100%"/>
</div>

<br/>

<div align="center">

```
I engineer operational systems end-to-end.
Architecture decisions matter more than features.
Offline-first. Low-bandwidth aware. Deployed at scale.
```

</div>

<br/>

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/ihimbru-kanyimi-46a973227)
[![Email](https://img.shields.io/badge/Gmail-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:kanihims25@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Ihimbru-K)

</div>

---

## engineering approach

> I architect systems, not features. Full ownership: database schema, API design, offline synchronization, deployment infrastructure. Focus on institutional-scale constraints, low-bandwidth optimization, and operational reliability. The hard problems are in the architecture, not the UI.

---

## systems & infrastructure

| domain | focus |
|--------|-------|
| **offline-first architectures** | conflict resolution, eventual consistency, deterministic sync |
| **institutional-scale systems** | role-based access control, audit trails, compliance constraints |
| **low-bandwidth optimization** | smart caching, progressive data loading, graceful degradation |
| **realtime coordination** | event-driven backends, websocket infrastructure, presence tracking |
| **hardware integration** | biometric systems, scanner drivers, device constraints |
| **payment infrastructure** | reconciliation, multi-provider SDKs, transaction integrity |

---

## projects

### Authentikate — Biometric Institutional Infrastructure
**Status:** Live pilot at University of Bamenda (30k+ students)

**Architecture:** Distributed offline-first system. Flutter clients cache enrollment & attendance data locally; FastAPI backend orchestrates synchronization via PostgreSQL state machine. ZK-Teco Live 20R biometric scanner integration handles device-level fingerprint capture. Role-based access control (admin, proctor, student) enforced at API boundary with JWT tokens.

**Technical depth:** Real-time attendance synchronization with conflict resolution; exam-hall connectivity constraints handled via smart offline fallbacks; audit trail integrity maintained through database triggers; institutional approval workflow embedded in schema.

**Repository:** [Frontend](https://github.com/Ihimbru-K/Authentikate_shipping_frontend) · [Backend](https://github.com/Ihimbru-K/Authentikate_shipping_backend)

---

### SheyDoc — Telemedicine Infrastructure for Sub-Saharan Constraints
**Status:** In development (targeting Cameroon's 4M+ patients without mental healthcare access)

**Architecture:** Lightweight Flutter client with offline-capable medical records; FastAPI backend orchestrating consultation coordination; Firebase/Appwrite for media handling with bandwidth-aware compression. FCM notifications with SMS fallback for low-connectivity regions.

**Technical depth:** Medical record sync with HIPAA-adjacent data handling; video/document caching optimized for limited device storage; low-battery considerations in client design; consultation state machine ensuring no missed appointments; payment integration for practitioner compensation.

**Key constraint:** Sub-Saharan device diversity (2G connectivity common, limited RAM, inconsistent power). Architecture accounts for all of it.

**Repository:** [Backend](https://github.com/Sheydocc/sheydoc_backend) · [Frontend](https://github.com/Sheydocc/sheydoc_app)

---

### Propti — Rent Management System (Digital Infrastructure)
**Status:** In development (community testing)

**Architecture:** Flutter frontend for tenant/landlord interactions; FastAPI backend coordinating payment reconciliation (MTN Mobile Money, Orange Money integration), document lifecycle management, and relational state. PostgreSQL schema handles multi-tenant isolation, payment idempotency, and legal document versioning.

**Technical depth:** Payment reconciliation across multiple SMS-based provider APIs; digital signature generation & validation with offline signing support; PDF document generation with audit trail; offline agreement signing with sync validation; real-time notification coordination.

**Operational problem:** Replacing analog workflows (handshakes, WhatsApp voice notes, ledger fraud). System-level solution required.

**Repository:** [Backend](https://github.com/Propti-app/Propti_backend)

---

### Cellytics — Analytics & Reporting Platform
**Status:** Production analytics infrastructure

**Architecture:** Data pipeline ingesting event streams from distributed sources; analytics backend processing cell-level metrics; queryable reporting frontend. Designed for operational transparency across hierarchical structures.

**Technical depth:** Time-series data aggregation; distributed event ingestion; real-time dashboard queries; data integrity at scale.

**Repository:** [Backend](https://github.com/Cellytics/cellytics_backend)

---

## technical stack

```
languages      →   Dart · Python · TypeScript · SQL
mobile         →   Flutter (offline-first, low-bandwidth optimization)
backend        →   FastAPI (async Python) · Spring Boot · Node.js
data           →   PostgreSQL (schema design, migrations)
                   Firebase/Appwrite (media, realtime)
infrastructure →   Docker · Render · Neon · GitHub Actions
realtime       →   WebSockets · Firebase Realtime · Appwrite
integrations   →   Biometric scanners (ZK-Teco)
                   Payment APIs (MTN, Orange)
                   FCM · SMS fallbacks
```

---

## what matters to me

Building systems for markets that are **underdeveloped** (limited connectivity), **underserved** (no existing infrastructure), and **underestimated** (dismissed as "too hard"). This requires real engineering:

- Architecture that survives low-bandwidth reality
- Database design that handles institutional complexity
- Deployment thinking from day one
- Understanding hardware & device constraints
- Operations-first mentality

Not: pixel perfection, feature lists, marketing language.

---

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Ihimbru-K&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true&title_color=7B77F5&icon_color=7B77F5" height="165"/>
&nbsp;
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Ihimbru-K&layout=compact&theme=tokyonight&hide_border=true&title_color=7B77F5" height="165"/>

</div>

<br/>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:302b63,100:0f0c29&height=120&section=footer&text=systems%20engineer%20%2F%20infrastructure%20architect&fontSize=16&fontColor=666666&fontAlignY=65" width="100%"/>
</div>










<!-- <div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,100:302b63&height=180&section=header&text=Ihimbru%20Kanyimi&fontSize=48&fontColor=ffffff&fontAlignY=52&desc=solutions%20builder%20%C2%B7%20mobile-first%20%C2%B7%20full-stack%20%C2%B7%20bamenda%2C%20cameroon&descSize=13&descAlignY=72&descColor=888888" width="100%"/>
</div>

<br/>

<div align="center">

```
I build things that solve problems people actually have.
Pixel-sharp mobile frontends. Backends that scale. Idea to deployment, start to finish.
```

</div>

<br/>

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/ihimbru-kanyimi-46a973227)
[![Email](https://img.shields.io/badge/Gmail-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:kanihims25@gmail.com)
[![HackerRank](https://img.shields.io/badge/HackerRank-2EC866?style=flat-square&logo=hackerrank&logoColor=white)](https://www.hackerrank.com/ihimbrukanyimi)

</div>

---

### what i build

> Full-stack, mobile-first. I architect systems end-to-end : Flutter frontends, FastAPI/Spring Boot backends, database design, cloud deployment. I own the whole thing, not just a layer.

---

### domains i care about

<div align="center">

`💳 fintech` &nbsp;&nbsp; `🎓 edtech` &nbsp;&nbsp; `🏥 medtech` &nbsp;&nbsp; `🏘️ proptech`

*building digital infrastructure in spaces that are underdeveloped, underserved, and overdue for change*

</div>

---

### shipped & building

| | project | what i built | impact |
|---|---|---|---|
| 🟢 | **[Authentikate](https://github.com/Ihimbru-K/Authentikate_shipping_frontend)** `live pilot` | Designed and built a biometric exam attendance system from scratch  fingerprint authenication with ZK-Teco Live 20R scanner, real-time tracking, role-based admin, REST API, full deployment | Pilot live at University of Bamenda · ~30k students at full institutional approval |
| 🔵 | **[SheyDoc](https://github.com/Sheydocc/sheydoc_backend)** `in dev` | Architected a mental health telemedicine platform for sub-Saharan Africa  video consults, FCM notifications, medical records, optimized for low-bandwidth conditions | Targeting Cameroon's 4M+ patients with no reliable access to mental healthcare |
| 🔵 | **[Propti](https://github.com/Propti-app/Propti_backend/tree/main)** `in dev` | Built a rent & tenant management system end-to-end : payment tracking, digital tenancy agreements, PDF generation, in-app signing | Digitizing a property market that still runs on handshakes and WhatsApp voice notes |

---

### stack

```
mobile     →   Flutter · Dart
backend    →   FastAPI · Spring Boot · Node.js
data       →   PostgreSQL · SQLAlchemy · Firebase · Appwrite
infra      →   Docker · Render · Neon · JWT · Stream SDK
```

---

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Ihimbru-K&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true&title_color=7B77F5&icon_color=7B77F5" height="165"/>
&nbsp;
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Ihimbru-K&layout=compact&theme=tokyonight&hide_border=true&title_color=7B77F5" height="165"/>

</div>

<br/>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:302b63,100:0f0c29&height=120&section=footer&text=let%27s%20build%20something%20that%20matters&fontSize=16&fontColor=666666&fontAlignY=65" width="100%"/>
</div>










<!-- <div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,100:302b63&height=180&section=header&text=Ihimbru%20Kanyimi&fontSize=48&fontColor=ffffff&fontAlignY=52&desc=solutions%20builder%20%C2%B7%20mobile-first%20%C2%B7%20full-stack%20%C2%B7%20bamenda%2C%20cameroon&descSize=13&descAlignY=72&descColor=888888" width="100%"/>
</div>

<br/>

<div align="center">

```
I don't just write code — I build things that solve problems people actually have.
Pixel-sharp mobile frontends. Backends that scale. Idea to deployment, start to finish.
```

</div>

<br/>

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/ihimbru-kanyimi-46a973227)
[![Email](https://img.shields.io/badge/Gmail-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:kanihims25@gmail.com)
[![HackerRank](https://img.shields.io/badge/HackerRank-2EC866?style=flat-square&logo=hackerrank&logoColor=white)](https://www.hackerrank.com/ihimbrukanyimi)

</div>

---

### what i build

> Full-stack, mobile-first. I architect systems end-to-end — Flutter frontends, FastAPI/Spring Boot backends, database design, cloud deployment. I own the whole thing, not just a layer.

---

### domains i care about

<div align="center">

`💳 fintech` &nbsp;&nbsp; `🎓 edtech` &nbsp;&nbsp; `🏥 medtech` &nbsp;&nbsp; `🏘️ proptech`

*building digital infrastructure in spaces that are underdeveloped, underserved, and overdue for change*

</div>

---

### shipped & building

| | project | what i built | impact |
|---|---|---|---|
| 🟢 | **[Authentikate](#)** `live pilot` | Designed and built a biometric exam attendance system from scratch — fingerprint auth, real-time tracking, role-based admin, REST API, full deployment | Pilot live at University of Bamenda · ~30k students at full institutional approval |
| 🔵 | **[SheyDoc](#)** `in dev` | Architected a telemedicine platform for sub-Saharan Africa — video consults, FCM notifications, medical records, optimized for low-bandwidth conditions | Targeting Cameroon's 4M+ patients with no reliable access to mental healthcare |
| 🔵 | **[Propti](#)** `in dev` | Built a rent & tenant management system end-to-end — payment tracking, digital tenancy agreements, PDF generation, in-app signing | Digitizing a property market that still runs on handshakes and WhatsApp voice notes |

---

### stack

```
mobile     →   Flutter · Dart
backend    →   FastAPI · Spring Boot · Node.js
data       →   PostgreSQL · SQLAlchemy · Firebase · Appwrite
infra      →   Docker · Render · Neon · JWT · Stream SDK
```

---

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Ihimbru-K&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true&title_color=7B77F5&icon_color=7B77F5" height="165"/>
&nbsp;
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Ihimbru-K&layout=compact&theme=tokyonight&hide_border=true&title_color=7B77F5" height="165"/>

</div>

<br/>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:302b63,100:0f0c29&height=120&section=footer&text=let%27s%20build%20something%20that%20matters&fontSize=16&fontColor=666666&fontAlignY=65" width="100%"/>
</div> -->  -->
