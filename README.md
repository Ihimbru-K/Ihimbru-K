






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












