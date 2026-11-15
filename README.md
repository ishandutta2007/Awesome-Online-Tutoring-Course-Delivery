# Awesome-Online-Tutoring-Course-Delivery

# Awesome Online Tutoring & Course Delivery

> A curated list of top Online Tutoring and Course Delivery platforms — both SaaS/Hosted commercial course platforms and open-source alternatives for creating, delivering, and monetizing online learning experiences.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [Teachable](#teachable)
  - [Thinkific](#thinkific)
  - [Kajabi](#kajabi)
  - [Podia](#podia)
  - [LearnWorlds](#learnworlds)
- [Open-Source Software](#-open-source-software)
  - [Euron Open LMS](#euron-open-lms)
  - [LearnHouse](#learnhouse)
  - [Scibly](#scibly)
  - [Oppia](#oppia)
  - [LiaScript](#liascript)
  - [VibeLMS](#vibelms)
  - [Open edX](#open-edx)
  - [Moodle](#moodle)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Online Tutoring and Course Delivery platforms. These are not open-source but are included as reference points for feature comparison.

### Teachable
**Type:** All-in-one course creation and sales platform
Teachable provides course authoring, student management, payment processing, and marketing tools in a single platform. It is positioned for creators and small businesses wanting to sell online courses without technical overhead, with tiered pricing based on features and transaction fees.

### Thinkific
**Type:** Course platform with strong customization
Thinkific offers course building, quizzes, certificates, and a customizable storefront, with a free plan for getting started. It is often compared to Teachable, with strengths in design flexibility and a lower barrier to entry.

### Kajabi
**Type:** Knowledge commerce platform with marketing automation
Kajabi combines course delivery with marketing funnels, email automation, and landing pages, positioning itself as a complete business platform for knowledge entrepreneurs. Pricing is higher than competitors but bundles marketing tools that would otherwise require separate subscriptions.

### Podia
**Type:** Creator platform for courses, downloads, and communities
Podia provides course hosting, digital downloads, webinars, and community features with no transaction fees on paid plans. It is positioned for creators wanting an all-in-one storefront without per-sale commissions.

### LearnWorlds
**Type:** Course platform with interactive video and assessments
LearnWorlds provides course authoring with interactive video, assessments, certificates, and a built-in community. It is positioned for educators and businesses wanting a more sophisticated learning experience than basic course hosting.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Online Tutoring and Course Delivery tools. The open-source ecosystem spans **full LMS platforms with commerce**, **AI-native learning platforms**, **interactive tutoring systems**, and **Markdown-based course authoring**.

### Euron Open LMS
**Stack:** TypeScript / Node.js / PostgreSQL / Terraform | **License:** Open Source (self-hosted)
Euron Open LMS is a comprehensive open-source, self-hosted LMS covering the full course delivery lifecycle: course catalog with full-text search and filters, a classroom with HLS video player (quality, speed, captions, resume, watermark), articles and PDFs, quizzes with question banks and server-side grading, assignments with rubrics and AI-assisted draft grading, verifiable certificates with public verification pages, reviews and Q&A, and a full commerce layer with Stripe and Razorpay billing . The **control plane** provides role-scoped admin areas for admins, support, finance, and instructors, with revenue/MRR dashboards, curriculum builder, learner management, grading, orders and refunds, coupons, moderation, and audit logs . Security includes identity from tokens (never body), access decisions in one place, payment signature verification in constant time, short-lived access tokens with refresh token rotation, and two-factor authentication . Deploys to AWS via Terraform with multi-AZ production configuration, or locally with Floci . A companion **mobile app** for iOS and Android supports offline video downloads and push notifications .
**Best for:** Organizations wanting a production-grade, self-hosted LMS with real payment processing, verifiable certificates, and full administrative control, accepting the AWS/Terraform deployment complexity.

### LearnHouse
**Stack:** Next.js / FastAPI / PostgreSQL / Hocuspocus | **License:** AGPL-3.0 (Enterprise features separate)
LearnHouse is a next-generation open-source learning platform with a **block-based, Notion-like content editor**, courses and collections, assignments, discussions, podcasts, analytics, and **AI-generated interactive playgrounds** [citation:11]. It includes **real code execution with auto-grading in 30+ languages**, real-time collaborative whiteboards, auto-generated certificates, user groups, and SEO optimization [citation:11]. The official CLI (`npx learnhouse@latest setup`) handles self-hosting, updates, and backups with a setup wizard walking through domain, database, and admin account configuration [citation:11]. **Important licensing note:** The core is AGPL-3.0, with enterprise features (payments, SSO, multi-org) under a separate license [citation:11].
**Best for:** Educators and organizations wanting a modern, feature-rich LMS with code execution and AI playgrounds, accepting the AGPL licensing and enterprise gating for payments/SSO.

### Scibly
**Stack:** Next.js / TypeScript / PostgreSQL / Prisma | **License:** AGPLv3 (core) / Enterprise (billing)
Scibly is an open-source, **AI-native learning platform** that transforms documents and internal knowledge into structured, interactive courses in minutes [citation:3]. It includes course authoring, learning, and a notebook, with real-time collaboration via Hocuspocus/Yjs, Stripe payments (enterprise slice), transactional email, and product analytics [citation:3]. Self-hosting via Docker Compose spins up PostgreSQL and all three apps in one command [citation:3]. **Important licensing note:** Everything outside the `ee/` directory is AGPLv3; the `ee/` directory (Stripe billing) is source-available but requires a separate license for production use [citation:3].
**Best for:** Teams wanting an AI-native platform that turns existing knowledge into courses quickly, accepting the open-core licensing model with billing gated to enterprise.

### Oppia
**Stack:** Python / Angular / Google App Engine | **License:** Apache-2.0
Oppia is an online learning tool that enables anyone to create and share **interactive activities called "explorations"** that simulate a one-on-one conversation with a tutor, letting students learn by doing while getting feedback . It is a nonprofit project with **6,771 GitHub stars and 5,646 forks**, built by a community for the community [citation:14]. The platform includes free lessons on basic mathematics, with plans to expand to science and financial literacy, targeting learners who lack access to educational resources . **Trade-off:** It is focused on interactive explorations rather than full course commerce or video delivery, and runs on Google App Engine which may limit self-hosting flexibility.
**Best for:** Educators and organizations wanting interactive, conversation-style tutoring activities with a proven nonprofit-backed platform, accepting the App Engine deployment model.

### LiaScript
**Stack:** JavaScript / Markdown | **License:** BSD-3-Clause
LiaScript is an open-source interpreter that turns **static Markdown files into fully interactive learning experiences** rendered directly in the browser, even offline [citation:7]. Features include quizzes, cloze tests, surveys, **text-to-speech in multiple languages**, live code execution (JavaScript, Python via Pyodide, MicroPython), ASCII diagrams, PWA support for offline use, and export to PDF, SCORM, and IMS [citation:7]. Courses are plain Markdown files hosted anywhere (GitHub, etc.) and opened via a URL, with a LiveEditor for browser-based authoring [citation:7]. **Trade-off:** It is a course authoring and delivery interpreter rather than a full LMS with commerce, student management, or analytics.
**Best for:** Educators and NGOs wanting to create interactive, offline-capable courses using plain Markdown, particularly for low-bandwidth or multilingual contexts.

### VibeLMS
**Stack:** React / Node.js / PostgreSQL / Drizzle | **License:** Open Source
VibeLMS is a modern LMS with hierarchical course structure (Course → Chapter → Lesson), YouTube video integration, rich text content with TipTap editor, interactive questions and assignments, and **progress tracking for both authenticated and anonymous users** [citation:9]. It includes JWT-based authentication with HTTP-only cookies, role-based access control (Teachers/Students), public course preview without registration, and Docker containerization [citation:9]. **Trade-off:** It uses YouTube for video hosting rather than self-hosted HLS, and its feature set is narrower than Euron or LearnHouse.
**Best for:** Small teams wanting a straightforward open-source LMS with YouTube integration and anonymous user support, accepting a lighter feature set.

### Open edX
**Stack:** Python / Django | **License:** AGPL-3.0
Open edX is the open-source platform behind edX, one of the largest MOOC providers, with course authoring, video delivery, assessments, certificates, and a massive ecosystem of extensions [citation:13]. It is positioned for universities and large organizations wanting a proven, scalable platform for online courses. **Trade-off:** It is a heavy, complex deployment requiring significant infrastructure and DevOps expertise, and the feature set is oriented toward academic institutions rather than individual creators.
**Best for:** Universities and large institutions wanting a battle-tested MOOC platform, accepting the substantial operational overhead.

### Moodle
**Stack:** PHP / MySQL/PostgreSQL | **License:** GPL-3.0
Moodle is the most widely deployed open-source LMS globally, used by universities, schools, and corporate training programs. It provides course management, quizzes, assignments, forums, gradebooks, and a vast plugin ecosystem, with integrations for video conferencing and content delivery [citation:13]. **Trade-off:** The interface is dated compared to modern platforms, and the breadth of configuration options can be overwhelming for small teams.
**Best for:** Educational institutions and organizations wanting a proven, extensible LMS with a massive community and plugin ecosystem, accepting a dated UI and configuration complexity.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Course Commerce | Video | AI/Interactive | Self-Hosted | Best For |
|----------|---------|-------|-----------------|-------|----------------|-------------|----------|
| **Teachable** | Proprietary | Cloud | ✅ | ✅ | ❌ | ❌ | Creator course sales |
| **Thinkific** | Proprietary | Cloud | ✅ | ✅ | ❌ | ❌ | Customizable course storefront |
| **Euron Open LMS** | Open Source | TS/Node/Postgres | ✅ Stripe/Razorpay | ✅ HLS | ✅ AI grading | ✅ | Full self-hosted LMS + commerce |
| **LearnHouse** | AGPL-3.0 | Next.js/FastAPI | (Enterprise) | ✅ | ✅ Code execution | ✅ | Modern LMS + AI playgrounds |
| **Scibly** | AGPLv3 | Next.js/Postgres | (Enterprise) | (Check) | ✅ AI-native | ✅ | Document-to-course AI |
| **Oppia** | Apache-2.0 | Python/Angular | ❌ | ❌ | ✅ Interactive explorations | (App Engine) | Conversation-style tutoring |
| **LiaScript** | BSD-3 | Markdown/JS | ❌ | (Check) | ✅ Interactive Markdown | ✅ | Markdown courses + offline |
| **VibeLMS** | Open Source | React/Node/Postgres | ❌ | YouTube | ❌ | ✅ | Simple LMS + YouTube |
| **Open edX** | AGPL-3.0 | Python/Django | ❌ | ✅ | ❌ | ✅ | University MOOC platform |
| **Moodle** | GPL-3.0 | PHP/DB | (Plugins) | (Plugins) | (Plugins) | ✅ | Institutional LMS |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Online Tutoring or Course Delivery tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source.

**Note on the open-source ecosystem:** Online course delivery splits between **full LMS platforms with commerce** (Euron Open LMS with Stripe/Razorpay and verifiable certificates , LearnHouse with code execution and AI playgrounds [citation:11]), **AI-native platforms** (Scibly for document-to-course conversion [citation:3]), **interactive tutoring systems** (Oppia's conversation-style explorations ), and **lightweight Markdown-based authoring** (LiaScript [citation:7]). **Euron Open LMS** is the most complete open-source option for organizations wanting to sell courses with real payment processing and full administrative control, while **LearnHouse** offers the most modern authoring experience with AI and code execution. No open-source project replicates the full marketing automation bundle of Kajabi or the polished storefront of Teachable, but combinations of these platforms with dedicated marketing tools can cover most creator needs.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
