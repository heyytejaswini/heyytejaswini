<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0B1026&height=220&section=header&text=Tejaswini%20V&fontColor=7CBFE9&fontSize=60&animation=twinkling&desc=design%20%C3%97%20technology%20%C3%97%20curiosity&descAlignY=72&descSize=18" width="100%"/>

<a href="https://github.com/heyytejaswini/Starstamp">
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=18&duration=3200&pause=900&color=7CBFE9&center=true&vCenter=true&width=640&lines=BCA+student+%40+CHRIST+University%2C+Bengaluru;building+Starstamp%3A+letters+that+wait+for+the+right+moment;exploring+RAG%2C+agentic+AI+and+GPU+computing;I+care+how+things+work+%E2%80%94+and+how+they+feel" alt="typing intro"/>
</a>

<br><br>

<div align="center">

<a href="https://www.linkedin.com/in/heyytejaswini/"><img src="https://img.shields.io/badge/LinkedIn-7CBFE9?style=for-the-badge&logo=linkedin&logoColor=0B1026"/></a>
&nbsp;
<a href="mailto:heyytejaswini@gmail.com"><img src="https://img.shields.io/badge/heyytejaswini%40gmail.com-0B1026?style=for-the-badge&logo=gmail&logoColor=7CBFE9"/></a>

<sub>✦ open to collaborations, internships and interesting conversations ✦</sub>

</div>

</div>

---

## ✦ Hello, I'm Tejaswini

First-year **BCA student at CHRIST (Deemed to be University), Bengaluru**, working where **software, AI, research and design** meet.

I like understanding *how* something works, and also *how it feels to use it*: the structure of a website, how information gets discovered, how an AI system retrieves and communicates what it knows.

> *I like building things that work, and I care that they feel, flow and communicate.*

<table>
<tr>
<td width="50%" valign="top">

**🌐 Web & Digital Experience**
Full-stack development · UI/UX · information architecture · content structuring · interactive experiences

</td>
<td width="50%" valign="top">

**🤖 AI & Emerging Tech**
LLMs · RAG · agentic AI · intelligent information retrieval · robotics · GPU-accelerated computing

</td>
</tr>
</table>

---

## 🌠 Featured: Starstamp

<div align="center">

### *write a letter. seal it. let the sky decide when it opens.*

</div>

**Starstamp** is a web app for time-locked letters. You write a letter to your future self, choose the **date** it should open, and seal it in an envelope you design yourself: layout, seal colour, stamp, postmark and stamped words. The envelope then turns into a **star** and flies into your night sky. When the day arrives, the star opens and the letter is yours again, and you get an email to tell you it's ready (the email never contains the letter's text).

Next up: a shared sky where letters you choose to share become stars for everyone, with lights, live shooting stars and reply letters.

`🚧 In Progress` · [Try it live](https://starstamp.vercel.app)

### The stack, in plain words

| Part | Tool | Its job in Starstamp |
|---|---|---|
| **Frontend** | Next.js · React · Tailwind | The sky, the writing desk, the star drawer |
| **Animation** | GSAP · SVG · Canvas | The door, the sealing sequence, the star flight, the twinkling sky |
| **Database** | Supabase Postgres | Letters, stars, envelope designs |
| **Auth** | Supabase Auth | Passwordless email-link sign-in |
| **Security** | Row Level Security | Decides who may read which letter and when |
| **Email** | Nodemailer · Vercel Cron | A daily job that emails writers when a letter is ready |
| **Hosting** | Vercel | The site and the scheduled job |

### The life of a letter

```mermaid
flowchart LR
    A["✍️ Write & seal<br/>text + date + envelope design"] --> B["🔒 Sealed<br/>envelope turns into a star in the sky"]
    B --> C{"The date arrives"}
    C --> D["📧 Daily job emails the writer<br/>(no letter text inside)"]
    C --> E["⭐ The star opens<br/>database allows the text to be read"]
    E --> F["🗑️ Keep it, or delete it<br/>(opened letters only)"]
```

### Design decisions I'm proud of

- **The browser is never trusted.** Anyone can open DevTools and tamper with what a page sends, so *"you can't read a sealed letter"* is enforced by the database itself with **Row Level Security (RLS)**, not by hiding things in the UI. The same goes for deleting: the database only allows it for your own letters that have already opened.
- **Lazy checking.** Nothing ticks in the background to unlock a letter. The database tests the date whenever someone asks to read it, so a letter can never open early.
- **Emails without secrets.** The unlock email only says a star is ready. The letter's text never leaves the database until its owner opens it.
- **Fast with many stars.** The sky draws glows from cached sprites instead of recalculating them every frame, which fixed lag once an account had hundreds of letters.
- **Complete deletion.** Deleting a letter removes its text, its star and everything linked to it in one step.

---

## ✦ Other Things I've Built

<table>
<tr>
<td width="50%" valign="top">

### ☕ Brew & Bloom Café
`HTML` `CSS` `JavaScript` `React` `Node.js` `Express` `MySQL` `MongoDB`

A full-stack café website concept about navigation, visual hierarchy and structured content: responsive design, interactive forms, database connectivity, and sustainability / SDG-linked content.
`🚧 In Progress`

</td>
<td width="50%" valign="top">

### 🌙 Lumé
`HTML` `CSS` `JavaScript` `Git`

A productivity and wellness app with Pomodoro focus sessions, task management and structured break activities, exploring external API integrations. Built around simplicity and user flow.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🎮 Unity 2D Shooter
`Unity` `2D game dev`

A functional 2D shooter. I worked on level design, gameplay mechanics, collision and physics, scoring, UI and playtesting, on top of an existing C# framework.

</td>
<td width="50%" valign="top">

### 🗑️ Automatic E-Dustbin
`Arduino UNO` `HC-SR04` `Servo`

A sensor-driven dustbin: ultrasonic detection triggers servo-controlled lid movement. A small project in hardware, logic and accessibility-minded design.

</td>
</tr>
</table>

<sub>Coursework also covers AngularJS, React, SQL/MySQL, MongoDB, Node.js and Express: controllers, data binding, event handling, forms and database integration.</sub>

---

## 🤖 AI × HPC

**Enterprise AI / HPC Bootcamp 2026**, Centre for AI, CHRIST (Deemed to be University): hands-on work with **NVIDIA H100** GPU-based AI workflows.

| Area | Exposure |
|---|---|
| GPU computing | NVIDIA H100 |
| AI frameworks | NVIDIA NeMo |
| Model adaptation | QLoRA / fine-tuning |
| Accelerated computing | RAPIDS |

`AI models → model adaptation → GPU infrastructure → accelerated workflows → practical applications`

### 🔬 Research interest

> **Evaluating RAG Systems for Reducing Hallucinations in Educational Question Answering**

- How does retrieval affect factual reliability?
- Why do LLMs hallucinate even on knowledge-based questions?
- How can external knowledge improve grounding?
- How should RAG systems be evaluated in educational settings?
- Where can agentic systems improve information retrieval?

---

## 🏛️ Experience

| Role | Where | When |
|---|---|---|
| **AI / HPC Intern & Peer Trainer** | Centre for AI, CHRIST University | 2026 – Present |
| **IT Support Intern** | Office of IT Services, CHRIST University | Jul 2026 – Present |
| **Management Intern** (Team Head) | Office of Admissions, CHRIST Central Campus | 185+ hrs of service across 1st and 2nd PUC |
| **Business Development Specialist Intern** | Younity | 2024 |

<details>
<summary><b>What I did in each role</b></summary>

<br>

**Centre for AI.** Worked with NeMo, QLoRA/fine-tuning and RAPIDS on H100s; took part in technical learning and knowledge-sharing; built an understanding of AI infrastructure and accelerated workflows.

**Office of IT Services.** Backend operations, technical documentation and institutional IT workflows; supported technology needs across the university.

**Office of Admissions.** Handled student and parent queries, assisted with admission processes, coordinated floor operations in high-footfall periods and led a team.

**Younity.** Client outreach and business-development calls; professional communication and stakeholder interaction.

</details>

---

## 📌 Digital Content & Design

<div align="center">

| `4.2M+` | `2M+` |
|:---:|:---:|
| Pinterest impressions | Audience reach |

</div>

Content work built on **visual communication, discoverability, trend analysis and digital storytelling**. Design tools: **Canva** (graphics, social, presentations) and **Figma** (basic UI, layout and interface structure).

### 🧠 Information, by design

```text
Research → Information → Structure → Design → Communication → Discovery
```

I'm drawn to academic websites, research communication and information-heavy interfaces, and I want to make complex information **clearer, more navigable and more human**.

---

## 🧩 Tech Stack

<p>
<img src="https://img.shields.io/badge/C-0B1026?style=flat-square&logo=c&logoColor=7CBFE9"/>
<img src="https://img.shields.io/badge/C++-0B1026?style=flat-square&logo=cplusplus&logoColor=7CBFE9"/>
<img src="https://img.shields.io/badge/JavaScript-0B1026?style=flat-square&logo=javascript&logoColor=7CBFE9"/>
<img src="https://img.shields.io/badge/React-0B1026?style=flat-square&logo=react&logoColor=7CBFE9"/>
<img src="https://img.shields.io/badge/Next.js-0B1026?style=flat-square&logo=nextdotjs&logoColor=7CBFE9"/>
<img src="https://img.shields.io/badge/Tailwind-0B1026?style=flat-square&logo=tailwindcss&logoColor=7CBFE9"/>
<img src="https://img.shields.io/badge/AngularJS-0B1026?style=flat-square&logo=angularjs&logoColor=7CBFE9"/>
<img src="https://img.shields.io/badge/Node.js-0B1026?style=flat-square&logo=nodedotjs&logoColor=7CBFE9"/>
<img src="https://img.shields.io/badge/Express-0B1026?style=flat-square&logo=express&logoColor=7CBFE9"/>
<img src="https://img.shields.io/badge/Supabase-0B1026?style=flat-square&logo=supabase&logoColor=7CBFE9"/>
<img src="https://img.shields.io/badge/PostgreSQL-0B1026?style=flat-square&logo=postgresql&logoColor=7CBFE9"/>
<img src="https://img.shields.io/badge/MySQL-0B1026?style=flat-square&logo=mysql&logoColor=7CBFE9"/>
<img src="https://img.shields.io/badge/MongoDB-0B1026?style=flat-square&logo=mongodb&logoColor=7CBFE9"/>
<img src="https://img.shields.io/badge/Vercel-0B1026?style=flat-square&logo=vercel&logoColor=7CBFE9"/>
<img src="https://img.shields.io/badge/Unity-0B1026?style=flat-square&logo=unity&logoColor=7CBFE9"/>
<img src="https://img.shields.io/badge/Git-0B1026?style=flat-square&logo=git&logoColor=7CBFE9"/>
<img src="https://img.shields.io/badge/Figma-0B1026?style=flat-square&logo=figma&logoColor=7CBFE9"/>
<img src="https://img.shields.io/badge/Canva-0B1026?style=flat-square&logo=canva&logoColor=7CBFE9"/>
<img src="https://img.shields.io/badge/LLMs-0B1026?style=flat-square&labelColor=0B1026&color=7CBFE9"/>
<img src="https://img.shields.io/badge/RAG-0B1026?style=flat-square&labelColor=0B1026&color=7CBFE9"/>
<img src="https://img.shields.io/badge/Agentic%20AI-0B1026?style=flat-square&labelColor=0B1026&color=7CBFE9"/>
<img src="https://img.shields.io/badge/NVIDIA%20NeMo-0B1026?style=flat-square&labelColor=0B1026&color=7CBFE9"/>
</p>

---

## 🧭 How I Work

**01 Understand** the problem, user and context → **02 Structure** it: *information → flow → interface → functionality* → **03 Build** something interactive → **04 Question** what works and why → **05 Improve** until it's clearer, more useful and more enjoyable.

---

## 🎓 Education, Certifications & Beyond

<details>
<summary><b>🎓 Education</b></summary>

<br>

- **BCA**, CHRIST (Deemed to be University), Bengaluru, 2026 – Present. Web & backend, C/C++, digital logic, databases, research writing, AI, DSA.
- **PUC (PCMC)**, Christ Junior College, Karnataka State Board, 2025
- **SSLC**, Madonna High School, Karnataka State Board, 2023: **96.96%**

</details>

<details>
<summary><b>📜 Certifications & learning</b></summary>

<br>

Harvard **CS50x** · Enterprise AI / HPC Bootcamp 2026 (Centre for AI, CHRIST) · NVIDIA H100 GPU-based AI training · NVIDIA NeMo · QLoRA / fine-tuning · RAPIDS · Data Artisan Bootcamp 2026 · Cadet Training Program

</details>

<details>
<summary><b>🎤 Events & engagement</b></summary>

<br>

**Emcee** at **IEEE ICONICA 2026** and the **SDG International Conference** (in association with Sophia University, Japan), plus AI, research and technology events: operations, hospitality, logistics and student engagement.

</details>

<details>
<summary><b>🪖 NCC · 🏅 Sports</b></summary>

<br>

**NCC B Certificate** (Christ Junior College, 2 years). Participated in IGC; 🥇 Gold Medal in Dance; represented 2/9 Coy NCC in Rifle Shooting at IGC Karnataka & Goa Directorate.
**Volleyball:** 🥇 District gold, state-level representation. **Throwball:** 🥇 District gold.

</details>

<details>
<summary><b>🌏 Languages</b></summary>

<br>

English (Professional) · Kannada, Hindi, Telugu (Fluent) · French (A1) · Mandarin Chinese (HSK 1)

</details>

<details>
<summary><b>🌱 Outside the terminal</b></summary>

<br>

Dancing · journaling · digital creation · game development · robotics · visual design · Pinterest curation

</details>

---

## 🎯 Where I'm Headed

I'm building a foundation across **software engineering, AI, research, design and information**, with the aim of making technology that's not only capable but **thoughtful, accessible and genuinely useful.**

---

<div align="center">

<table align="center">
<tr>
<td align="center" valign="top">
<img height="195" src="https://streak-stats.demolab.com/?user=heyytejaswini&hide_border=true&background=FFFFFF00&ring=7CBFE9&fire=7CBFE9&currStreakLabel=7CBFE9&sideLabels=8B949E&currStreakNum=8B949E&sideNums=8B949E&dates=8B949E"/>
</td>
<td align="center" valign="center">
<img height="195" src="https://github-readme-stats.vercel.app/api/top-langs/?username=heyytejaswini&layout=compact&langs_count=20&hide_border=true&title_color=7CBFE9&text_color=8B949E&bg_color=FFFFFF00"/>
</td>
</tr>
</table>

<br>

### 🩵 Let's connect
Web development · AI · research · design · emerging technology

<div align="center">

<a href="https://www.linkedin.com/in/heyytejaswini/"><img src="https://img.shields.io/badge/LinkedIn-7CBFE9?style=for-the-badge&logo=linkedin&logoColor=0B1026"/></a>
&nbsp;
<a href="mailto:heyytejaswini@gmail.com"><img src="https://img.shields.io/badge/heyytejaswini%40gmail.com-0B1026?style=for-the-badge&logo=gmail&logoColor=7CBFE9"/></a>

<sub>✦ open to collaborations, internships and interesting conversations ✦</sub>

</div>

<br>

<img src="https://capsule-render.vercel.app/api?type=waving&height=120&color=0B1026&section=footer&animation=twinkling" width="100%"/>

</div>

<!-- Made with curiosity, caffeine, and too many browser tabs. 🩵 -->
