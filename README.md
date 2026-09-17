# ⚡ Omar Mohammed | Software Engineer (.NET & AI Systems)

<div align="center">

[![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=24&pause=1000&color=0078D4&center=true&vCenter=true&width=700&lines=Back-End+.NET+Engineer;AI+Systems+%26+Cloud+Integrations;Clean+Architecture+%26+Domain-Driven+Design;Building+High-Concurrency+%26+Production-Ready+APIs)](https://git.io/typing-svg)

**🎓 B.Sc. in Artificial Intelligence** | **🏆 ITI Graduate (.NET Track)** | **📍 Cairo, Egypt**

<br/>

[![Download Resume](https://img.shields.io/badge/📄_Resume-Download_CV-0078D4?style=for-the-badge&logo=adobeacrobatreader&logoColor=white)](https://drive.google.com/file/d/1LV-yIG0IXE-lWFUW7zeWRvzdBByG1Yjw/view?usp=drive_link)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/omar-mahamad-omd)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Chat-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/201015850226)
[![Email](https://img.shields.io/badge/Email-Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:omarmahamadomd@gmail.com)

</div>

---

### 💡 About Me

I am a **Software Engineer** specializing in **.NET Back-End Architecture** and **AI-Driven Cloud Systems**. Blending a formal academic background in **Artificial Intelligence Engineering** with enterprise .NET practices, I architect resilient, scalable, and zero-trust backend systems adhering strictly to **Clean Architecture** and **Domain-Driven Design (DDD)**.

* 🚀 **Production-Tested Scale:** Solo architected the backend for a commercial AI voice platform serving **500+ active users** with **99.9% uptime**.
* 🏛️ **Domain-Driven Design (DDD):** Deep hands-on experience enforcing domain invariants, rich entities, immutable Value Objects, and transactional domain events.
* ⚡ **High Concurrency & Fault Tolerance:** Designing resilient APIs utilizing atomic credit locking, race-condition mitigation, and asynchronous background worker queues.
* 🛡️ **Zero-Trust Security & Anti-Fraud:** Implementing advanced cryptographic protections, HMAC verification, device fingerprinting, and defensive media pipelines.

---

### 🏆 Featured Flagship Case Studies

<table>
<tr>
<td>

### 🎙️ Case Study 01: [Sada AI — Commercial AI Audio Platform](https://sadaai.io)
**Role:** Solo Backend Architect & Engineer &nbsp;|&nbsp; **Status:** Production / Commercial &nbsp;|&nbsp; **Link:** [sadaai.io](https://sadaai.io)

> **A high-concurrency commercial Arabic Text-to-Speech (TTS) and voice orchestration SaaS engineered from scratch.**

* 📈 **Commercial Scale:** Orchestrates **168+ AI voice profiles** across multiple upstream vendors, serving **500+ users** with **99.9% production uptime**.
* ⚡ **High-Concurrency TTS & Atomic Locking:** Built an intelligent provider-routing abstraction with smart request queuing and atomic credit locking to completely eliminate race conditions and prevent wallet overspending during high-traffic spikes.
* 🛡️ **In-House Device Intelligence & Anti-Fraud:** Engineered a custom risk-operations engine detecting account farming and free-tier entitlement abuse using device clustering, browser fingerprinting, and HMAC-signed installation tokens.
* 🔒 **Defensive Media Security Pipeline:** Integrated low-level media sanitization using **SkiaSharp** to inspect magic bytes and re-encode user-uploaded imagery, neutralizing steganography and polyglot payloads prior to Cloudflare R2 persistence.
* 🌐 **Hardened Linux Infrastructure:** Orchestrated rootless Docker deployments behind an NGINX reverse proxy with Cloudflare Origin TLS, automated EF Core migrations, and server-side telemetry via Meta Conversions API (CAPI).

**Tech Stack:** `.NET 9` `C#` `Clean Architecture (DDD)` `EF Core` `SQL Server 2022` `Cloudflare R2 & WAF` `Docker` `NGINX` `Serilog`

</td>
</tr>
<tr>
<td>

### ⚡ Case Study 02: [Temp-Back_End — Enterprise Web API Foundation](https://github.com/OmarMahamad/Temp-Back_End)
**Role:** Author & Maintainer &nbsp;|&nbsp; **Status:** Open Source &nbsp;|&nbsp; **Repo:** [github.com/OmarMahamad/Temp-Back_End](https://github.com/OmarMahamad/Temp-Back_End)

> **An enterprise-grade, production-ready .NET 9 Web API starter template built with strict Clean Architecture, Domain-Driven Design (DDD), and automated CI/CD.**

* 📊 **Commercial Impact:** Adopted across **3 commercial client implementations**, slashing initial backend scaffolding and setup time by **50%**.
* 🛡️ **Zero Build Degradation:** Maintained **0 Errors, 0 Warnings** under strict compiler analyzers and automated static checks.
* 🧪 **Comprehensive Test Harness:** **58 automated unit tests** (xUnit + Moq) executing in **~1.0 second** with 100% pass rate.
* 🔑 **Zero-Trust Identity Hardening:** PBKDF2 cryptographic hashing (100,000 iterations + 128-bit salt), constant-time comparisons (`CryptographicOperations.FixedTimeEquals`) to eliminate timing attacks, and stateful JWT with 7-day sliding refresh token rotation and multi-device revocation.
* 🔄 **Automated Domain Events:** MediatR-powered domain event publication dispatched automatically inside EF Core's `ChangeTracker` during `SaveChangesAsync`.

```text
┌─────────────────────────────────────────────────────────────┐
│                      Presentation / API                     │
│  Controllers ── Swagger / OpenAPI ── RFC Exception Filters  │
└──────────────────────────────┬──────────────────────────────┘
                               │ references
┌──────────────────────────────▼──────────────────────────────┐
│                      Application Core                       │
│    Commands & Queries (CQRS / MediatR) ── DTOs ── Mappers   │
└──────────────┬──────────────────────────────┬───────────────┘
               │                              │
    implements │                              │ references
┌──────────────▼──────────────┐┌──────────────▼───────────────┐
│        Infrastructure       ││            Domain            │
│  EF Core 9 ── SQL Server    ││  Entities (Private Setters)  │
│  Cloudinary CDN ── Docker   ││  Value Objects ── Domain Evt │
└─────────────────────────────┘└──────────────────────────────┘
```

**Tech Stack:** `.NET 9.0` `C# 13` `EF Core 9` `SQL Server 2022` `Docker` `GitHub Actions (CI/CD)` `xUnit / Moq` `MediatR`

</td>
</tr>
</table>

---

### 🛠️ Technical Arsenal

<div align="center">

| Domain | Technologies & Frameworks |
| :--- | :--- |
| **Backend & Core** | ![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=c-sharp&logoColor=white) ![-NET](https://img.shields.io/badge/.NET_8%20%2F%209-512BD4?style=flat-square&logo=dotnet&logoColor=white) ![ASP.NET Core](https://img.shields.io/badge/ASP.NET_Core_Web_API-512BD4?style=flat-square&logo=.net&logoColor=white) ![EF Core](https://img.shields.io/badge/EF_Core_9-512BD4?style=flat-square&logo=.net&logoColor=white) |
| **Architecture & Design** | ![Clean Architecture](https://img.shields.io/badge/Clean_Architecture-0078D4?style=flat-square) ![DDD](https://img.shields.io/badge/Domain--Driven_Design_(DDD)-0078D4?style=flat-square) ![CQRS](https://img.shields.io/badge/CQRS_%26_MediatR-blueviolet?style=flat-square) ![RESTful](https://img.shields.io/badge/RESTful_APIs-orange?style=flat-square) |
| **Databases & Storage** | ![SQL Server](https://img.shields.io/badge/SQL_Server_2022-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white) ![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white) ![Cloudflare R2](https://img.shields.io/badge/Cloudflare_R2-F38020?style=flat-square&logo=cloudflare&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) |
| **DevOps & Cloud** | ![Docker](https://img.shields.io/badge/Docker_(Rootless)-2496ED?style=flat-square&logo=docker&logoColor=white) ![NGINX](https://img.shields.io/badge/NGINX-009639?style=flat-square&logo=nginx&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions_CI%2FCD-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![Cloudflare](https://img.shields.io/badge/Cloudflare_Edge-F38020?style=flat-square&logo=cloudflare&logoColor=white) |
| **Testing & Reliability** | ![xUnit](https://img.shields.io/badge/xUnit-512BD4?style=flat-square) ![Moq](https://img.shields.io/badge/Moq-blueviolet?style=flat-square) ![Serilog](https://img.shields.io/badge/Serilog-0078D4?style=flat-square) ![RFC-7807](https://img.shields.io/badge/RFC--7807_Errors-gray?style=flat-square) |

</div>

---

### 📈 GitHub Insights

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=OmarMahamad&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=0078D4&icon_color=0078D4&text_color=C9D1D9&count_private=true&include_all_commits=true" alt="GitHub Stats" width="48%" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=OmarMahamad&layout=compact&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=0078D4&text_color=C9D1D9&langs_count=6" alt="Top Languages" width="48%" />

</div>

---

### 🎓 Education & Professional Foundation

* **B.Sc. in Artificial Intelligence** — Egyptian Russian University (*Graduation Project: One Blood — Grade: A+*)
* **Information Technology Institute (ITI)** — Back-End .NET Development Track (Intensive Program)
* **Industry Experience:** Full-Stack .NET Developer at **Clutch** (Engineered API & SQLite synchronization, background worker services, and resolved 70+ compiler warnings across POS/Inventory modules).
* **Awards:** Ranked among **Top 30 Teams Nationwide** at the *Egyptian Grand Museum Hackathon 2* (AI Backend Integration).

---

<div align="center">

### 🤝 Let's Build Something Exceptional

Open for **Back-End .NET Engineer** and **AI Systems Integration** opportunities.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/omar-mahamad-omd)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Chat-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/201015850226)
[![Email](https://img.shields.io/badge/Email-Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:omarmahamadomd@gmail.com)

</div>
