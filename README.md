<div align="center">
  <h1>Ihimbru Kanyimi</h1>
  <p><strong>Systems engineer building operational infrastructure</strong></p>
  <p>Full-stack · Offline-first · Low-bandwidth aware · Institutional scale</p>
  <p>Bamenda, Cameroon</p>
</div>

---

## Overview

I engineer systems, not features. Full-stack ownership across architecture, database design, offline synchronization, and cloud deployment. Specialization in low-bandwidth environments, institutional-scale constraints, and operational reliability.

Core competency: taking complex, under-resourced problems and building production infrastructure that actually works in the field.

---

## How I Approach Systems

- **Offline-first by default** — Assume connectivity is constrained. Design for unreliable networks, device storage limits, and intermittent syncing.
- **Architecture before aesthetics** — Database schema, API design, and deployment strategy matter more than UI polish. Get the foundation right.
- **Operational thinking** — Build monitoring, logging, and graceful degradation into the system from day one, not as an afterthought.
- **Real-world constraints** — Understand actual deployment environments: device capabilities, network reality, power consumption, institutional compliance, and hardware limitations.
- **Systems integration** — Hardware-to-cloud pipelines. Biometric scanners talking to backends. Payment systems with fallbacks. Nothing in isolation.

---

## Projects & Architecture

### **Authentikate** — Institutional Biometric Infrastructure
**Status:** Live pilot · University of Bamenda · ~30k students

Designed and built end-to-end biometric attendance infrastructure for institutional scale.

**Architecture:**
- **Client:** Flutter app with offline-first local database; queues attendance records for sync when connectivity returns
- **Hardware integration:** ZK-Teco Live 20R biometric scanner communicating via REST; device fallback logic for scanner disconnects
- **Backend:** FastAPI REST API coordinating student/examiner/admin state; role-based access control with institutional hierarchies
- **Data:** PostgreSQL with student enrollment, exam schedules, attendance records, audit trails
- **Deployment:** Containerized on Render; database on Neon
- **Sync strategy:** Conflict resolution for simultaneous attendance submissions; reconciliation of offline submissions with server state

**Engineering challenges solved:**
- Device fingerprint data integrity in high-volume exam halls
- Offline attendance recording with guaranteed submission when connectivity restored
- Role-based permissions across student/examiner/admin/institutional-admin layers
- Audit trail compliance for institutional record-keeping

**Links:** [Frontend](https://github.com/Ihimbru-K/Authentikate_shipping_frontend) · [Backend](https://github.com/Ihimbru-K/Authentikate_backend)

---

### **SheyDoc** — Telemedicine Infrastructure for Sub-Saharan Deployment
**Status:** In development

Mental health telemedicine platform built from the ground up for sub-Saharan Africa's connectivity and device constraints.

**Architecture:**
- **Client:** Lightweight Flutter app designed for low-end devices; offline-capable medical records (patient history, consultation notes, prescriptions); local caching for all static data
- **Consultation coordination:** FastAPI backend orchestrating real-time video calls, async messaging, and appointment scheduling
- **Media handling:** Appwrite for medical document storage and retrieval; bandwidth-aware image compression; fallback mechanisms for failed uploads
- **Notifications:** Firebase Cloud Messaging with SMS fallback for regions where push notifications unreliable
- **Data layer:** Firestore for real-time presence (who's online), Firebase Auth for patient/provider auth, PostgreSQL for consultation records and medical history

**Engineering complexity:**
- Video consultation fallback to audio-only for low-bandwidth regions
- Offline medical records syncing with conflict resolution (notes written offline, provider notes written during consultation)
- HIPAA-adjacent data handling: encryption at rest, patient privacy boundaries, provider access controls
- Device capability detection: graceful degradation for devices with low storage/RAM
- Multi-region presence tracking: knowing if a provider is available without constant polling

**Key insight:** Building for Africa means optimizing for what's actually available (2G fallbacks, 1GB devices, erratic power), not what the cloud assumes.

**Link:** [Backend](https://github.com/Sheydocc/sheydoc_backend)

---

### **Propti** — Rent Management Operational Infrastructure
**Status:** In development

System replacing informal property management (WhatsApp, voice notes, handwritten agreements) with digital operational infrastructure.

**Architecture:**
- **Client:** Flutter app for tenants (pay rent, view agreements, submit maintenance requests) and landlords (track payments, manage properties, send notices)
- **Payment coordination:** FastAPI backend integrating MTN Mobile Money and Orange Money; payment reconciliation across providers; fallback handling for failed transactions
- **Document lifecycle:** PDF generation of tenancy agreements; in-app signing with signature capture; document versioning and audit trail
- **State management:** PostgreSQL storing properties, tenants, leases, payment records; relational integrity for rent-due-date calculations
- **Deployment:** Containerized backend; database migrations managed in CI/CD

**Engineering challenges:**
- Payment idempotency: handling duplicate payment submissions and reconciling with provider APIs
- Multi-currency support: MTN and Orange Money transactions in local currency with exchange rate tracking
- Legal document integrity: agreements must be signed, timestamped, and immutable once executed
- Offline signature capture: signatures collected offline, validated and stored on sync
- Reconciliation: daily payment sync with provider APIs to catch missing/failed transactions

**Link:** [Backend](https://github.com/Propti-app/Propti_backend)

---

### **Cellytics** — Analytics & Reporting Pipeline
**Status:** Production

Reporting and analytics platform built for the Christ Embassy's global hierarchical structure. Processes cell-group data (prayer meetings, attendance, offerings, conversions) across 50+ countries.

**Architecture:**
- **Client:** Lightweight web interface for data entry at cell level; offline-capable form submissions
- **Data aggregation:** FastAPI backend accepting submissions from distributed regions; ETL pipeline normalizing data across different input formats
- **Analytics layer:** PostgreSQL data warehouse; SQL-based report generation; hierarchical rollup (cell → zone → region → country)
- **Export & distribution:** PDF report generation; automated email distribution to regional leaders

**Engineering insight:** Building for institutional reporting means understanding hierarchical approval workflows, regional autonomy (each region has different data entry capacity), and the need for auditability at every level.

**Link:** [Backend](https://github.com/Cellytics/cellytics_backend)

---

## Technical Stack

### **Application Layer**
- **Mobile:** Flutter (Dart) — production-grade apps with offline-first state management
- **Backend:** FastAPI (async Python) — high-throughput APIs with minimal overhead; Spring Boot for institutional integrations
- **Web:** Next.js / TypeScript — when web interfaces needed (admin dashboards, reporting)

### **Data Layer**
- **Relational:** PostgreSQL — schema design, migrations, query optimization
- **Real-time:** Firebase (Firestore, Realtime Database) — presence, notifications, soft state
- **Document storage:** Appwrite — media handling, file versioning
- **ORM:** SQLAlchemy (Python), Prisma (TypeScript) — migration-first approach

### **Infrastructure & Deployment**
- **Containerization:** Docker — environment parity from dev to production
- **Cloud platforms:** Render (app hosting), Neon (managed PostgreSQL), Firebase (backend-as-a-service components)
- **CI/CD:** GitHub Actions — automated testing, migrations, deployments
- **Authentication:** JWT-based auth, OAuth 2.0 integrations, role-based access control
- **Monitoring:** Structured logging, error tracking, application performance visibility

### **Key Integrations**
- Payment systems (MTN Mobile Money, Orange Money)
- Hardware communication (biometric scanners, serial protocols)
- Real-time video (custom WebRTC, Stream SDK)
- SMS fallback services
- PDF generation & digital signing

---

## What Gets Built

**Institutional-scale systems** with real operational constraints:
- Biometric infrastructure for universities
- Telemedicine platforms for under-resourced regions
- Financial tracking systems for informal markets
- Hierarchical reporting platforms for distributed organizations
- Analytics pipelines processing institutional data

**Not:** SaaS templates, consumer apps, feature-focused MVPs.

**Always:** Systems that work in the field, handle real constraints, and stay operational under pressure.

---

## Work Domains

**Fintech for informal markets** — Payment systems for regions with limited banking infrastructure
**Edtech for institutional deployment** — Systems built to work inside universities, schools, training centers
**Medtech in low-bandwidth regions** — Healthcare infrastructure for areas with erratic connectivity
**Proptech in developing markets** — Digitizing informal property management, tenant tracking, payment collection

---

## Contact & Links

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/ihimbru-kanyimi-46a973227)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:kanihims25@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-333?style=flat-square&logo=github&logoColor=white)](https://github.com/Ihimbru-K)

---

<div align="center">
  <p><em>Building systems that work where infrastructure is constrained and stakes are real.</em></p>
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
</div> --> -->
