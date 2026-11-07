<p align="center">
  <img src="./Rishi_Dulhani_Cyber_City_Banner.gif" width="100%" alt="Rishi Dulhani — cyber city engineering profile banner" />
</p>

<p align="center"><sub><a href="./Rishi_Dulhani_Cyber_City_Banner.png">View static high-resolution PNG version</a></sub></p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=17&duration=2400&pause=850&color=70F6F0&center=true&vCenter=true&width=1000&lines=PYTHON+BACKEND+%2F+DATABASES+%2F+SYSTEMS;LOCAL+DOCUMENT+INTELLIGENCE+%2F+APPLIED+ML;OFDM+%2F+CHANNEL+ESTIMATION+%2F+WIRELESS;GNSS+%2F+IMU+FUSION+%2F+EMBEDDED+SECURITY" alt="Engineering focus areas" />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/rishi-dulhani-397987360/"><img src="https://img.shields.io/badge/LINKEDIN-111827?style=for-the-badge&logo=linkedin&logoColor=70F6F0" alt="LinkedIn" /></a>
  <a href="mailto:rishidulhani7070@gmail.com"><img src="https://img.shields.io/badge/EMAIL-111827?style=for-the-badge&logo=gmail&logoColor=FF69C8" alt="Email" /></a>
  <a href="tel:+919096780763"><img src="https://img.shields.io/badge/CALL-111827?style=for-the-badge" alt="Call +91 90967 80763" /></a>
  <a href="https://github.com/Rishi-D70"><img src="https://img.shields.io/badge/GITHUB-111827?style=for-the-badge&logo=github&logoColor=FFFFFF" alt="GitHub" /></a>
</p>

<p align="center">
  <a href="#profile">PROFILE</a> &nbsp; / &nbsp;
  <a href="#selected-builds">SELECTED BUILDS</a> &nbsp; / &nbsp;
  <a href="#research--publications">RESEARCH</a> &nbsp; / &nbsp;
  <a href="#technical-stack">STACK</a> &nbsp; / &nbsp;
  <a href="#contact">CONTACT</a>
</p>

---

## `01 / PROFILE`

**I build systems that turn messy inputs into useful decisions.**

I'm a final-year **B.Tech Electronics & Telecommunication** student with a **Data Science minor** at D. Y. Patil School of Engineering and Management, Kolhapur (**8.60/10 CGPA**, graduating May 2027).

My work sits across three connected areas: **Python backend engineering**, **applied machine learning and local document intelligence**, and **wireless / embedded systems**. I've worked on transaction-safe Django applications, offline contract analysis, computer-vision classification, OFDM channel-estimation research, and an embedded GNSS spoofing-detection prototype.

I care about the engineering underneath the demo: data models, evaluation methodology, edge cases, latency, reproducibility, and whether a system behaves correctly outside the happy path.

<p align="center">
  <img src="https://img.shields.io/badge/BASE-KOLHAPUR%2C%20INDIA-101827?style=flat-square&labelColor=101827&color=1C3448" alt="Based in Kolhapur, India" />
  <img src="https://img.shields.io/badge/GRADUATION-MAY%202027-101827?style=flat-square&labelColor=101827&color=164B52" alt="Graduating May 2027" />
  <img src="https://img.shields.io/badge/FOCUS-BACKEND%20%7C%20APPLIED%20ML%20%7C%20EMBEDDED-101827?style=flat-square&labelColor=101827&color=4A2750" alt="Career focus" />
</p>

### Engineering lanes

<table>
  <tr>
    <td width="33%" valign="top">
      <strong>01 — Backend systems</strong><br /><br />
      Django, relational data modelling, PostgreSQL, SQL, transaction safety, query optimisation, and automated tests.<br /><br />
      <sub>Proof point: dashboard queries reduced from ~48 to 6; load time from ~1.4 s to ~450 ms.</sub>
    </td>
    <td width="33%" valign="top">
      <strong>02 — Applied ML & local AI</strong><br /><br />
      PyTorch, computer vision, document extraction, OCR, retrieval, local LLM inference, and model evaluation.<br /><br />
      <sub>Proof point: offline contract analysis evaluated on 50 CUAD documents.</sub>
    </td>
    <td width="33%" valign="top">
      <strong>03 — Wireless & embedded</strong><br /><br />
      OFDM, channel estimation, GNSS, IMU sensor fusion, ESP32-based prototyping, and navigation-security research.<br /><br />
      <sub>Proof point: residual CNN experiments across multiple channel profiles.</sub>
    </td>
  </tr>
</table>

---

## `02 / SELECTED BUILDS`

A selection of projects where I can show the problem, the implementation choices, and the result — not just the tech stack.

### `A` — ContractIQ / Project-IQ

**Offline contract intelligence | Local LLMs | Retrieval-augmented analysis**

<a href="https://github.com/Rishi-D70/Project-IQ"><img src="https://img.shields.io/badge/VIEW%20SOURCE-70F6F0?style=for-the-badge&logo=github&logoColor=08111F" alt="View Project-IQ source" /></a>
<a href="https://drive.google.com/file/d/1J2JIDNkhjIDVbTbfC3PK7gZ5QIXSfe9Z/view?usp=sharing"><img src="https://img.shields.io/badge/PROJECT%20DEMO-FF69C8?style=for-the-badge&logo=google-drive&logoColor=10111C" alt="Watch ContractIQ demo" /></a>

A local-first document intelligence prototype that analyses contracts and policies without sending documents to a cloud service. The repository is named **Project-IQ**; the application is presented as **ContractIQ**.

- **Ingestion:** PDF text extraction with `pdfplumber`, with Tesseract OCR as a fallback for scanned pages.
- **Retrieval and reasoning:** FAISS-based clause retrieval paired with a 4-bit **Qwen2.5-7B** model running locally through `llama.cpp`.
- **Analysis:** clause-aware question answering, extraction of parties / obligations / dates, and risk flags across eight categories with severity and source excerpts.
- **Privacy model:** document processing and inference run locally; contract content is not uploaded to a hosted LLM service.
- **Evaluation:** tested on 50 CUAD contracts across six clause types, reaching **0.81 precision** and **0.74 recall**. A 10-page NDA was analysed in approximately **45 seconds** on the test machine.

<sub>Stack: Python · pdfplumber · Tesseract OCR · FAISS · llama.cpp · Qwen2.5-7B · SQLite</sub>

---

### `B` — Hospital Management System

**Full-stack developer internship project | Study Brainz | Sep 2025 – Feb 2026**

Built the backend of a hospital management application using Django and PostgreSQL, with an emphasis on reliable booking workflows and efficient database access.

- Designed an **8-model relational schema** using foreign keys and composite indexes.
- Prevented conflicting appointment bookings through database constraints and atomic transactions.
- Optimised dashboard data access from approximately **48 queries to 6**.
- Reduced measured dashboard load time from approximately **1,400 ms to 450 ms**, tested against **5,000 records**.
- Added **24 pytest tests** covering booking conflicts, permissions, and prescription workflows.

<sub>Stack: Python · Django · PostgreSQL · SQL · pytest · Git</sub>

---

### `C` — OFDM Channel Estimation Under Channel Mismatch

**Wireless communications research | Python · NumPy · PyTorch**

Co-authored research investigating a practical weakness in learned channel estimators: strong in-distribution results can degrade when the propagation channel differs from the training distribution.

- Built a pilot-assisted OFDM simulation with **64 subcarriers** and **QPSK** modulation.
- Implemented **LS**, realistic **LMMSE**, and oracle-LMMSE baselines.
- Trained a **3-layer residual 1D CNN** on 20,000 generated channel samples.
- Compared narrow training (Rayleigh only) with diverse training across **Rayleigh, Rician, EPA, EVA, and ETU** channel profiles.
- At **20 dB on the ETU channel**, the diverse CNN reduced NMSE by **86.59%** and BER by **85.82%** relative to the LMMSE baseline, using **1,000 Monte Carlo runs per SNR point**.
- Developed two evaluation measures — **Robustness Ratio** and **Effective SNR Loss** — to quantify performance degradation under channel mismatch.

<sub>Status: co-authored manuscript under review at Elsevier's *Physical Communication*.</sub>

---

### `D` — GNSS Spoofing Detection with Low-Cost GNSS + IMU Fusion

**Embedded systems capstone | Navigation security | In progress**

A low-cost defensive prototype designed to identify suspicious GNSS navigation data by checking whether reported satellite-derived movement is consistent with independent inertial measurements.

```mermaid
flowchart LR
    A[ u-blox NEO-M9N ] -->|GNSS navigation data| C[ ESP32-S3 detector ]
    B[ MPU9250 IMU ] -->|Motion reference| C
    C --> D[ Consistency checks ]
    D --> E{Motion agrees?}
    E -->|Yes| F[Nominal navigation]
    E -->|No| G[Flag for spoofing review]
    C --> H[Telemetry and data logging]
```

- **Receiver:** u-blox NEO-M9N; UART1 configured at 115200 baud with UBX-only output at 5 Hz, including NAV-PVT, NAV-SAT, and MON-RF message streams.
- **Compute and sensing:** ESP32-S3 development board with an MPU9250 9-axis inertial sensor.
- **Data path:** UART-based receiver integration, GNSS / IMU data acquisition, and local logging for analysis.
- **Validation concept:** three controlled test scenarios on an RC-car platform, comparing GNSS-derived motion with inertial movement estimates.
- **Research objective:** build a labelled GNSS–IMU dataset and evaluate whether a lightweight detector can identify navigation inconsistencies on-device.

<sub>Status: hardware and receiver bring-up are underway; live validation and model performance are not yet claimed.</sub>

---

### `E` — Cattle Breed Classification

**Computer vision | PyTorch | Django inference**

- Fine-tuned **MobileNetV2** on approximately **2,600 images across 10 cattle breeds**.
- Used a stratified **70 / 15 / 15** train-validation-test split, weighted loss, and data augmentation.
- Reached **82% accuracy** and **0.80 macro-F1** on the reported evaluation split.
- Used **Grad-CAM** checks to inspect model attention and served predictions through a Django inference endpoint.

<sub>Stack: Python · PyTorch · MobileNetV2 · scikit-learn · Grad-CAM · Django</sub>

---

### `F` — Fly-High-Index

**Smart India Hackathon 2026 | Team project**

A team-built Smart India Hackathon project exploring a **real-time airfare price index for India**.

<a href="https://github.com/Rishi-D70/Fly-High-Index"><img src="https://img.shields.io/badge/VIEW%20PROJECT-70F6F0?style=for-the-badge&logo=github&logoColor=08111F" alt="View Fly-High-Index" /></a>

<sub>Repository: Fly-High-Index</sub>

### More code

- [Simple_Py_Projects](https://github.com/Rishi-D70/Simple_Py_Projects) — smaller Python experiments and practice builds.
- [All repositories](https://github.com/Rishi-D70?tab=repositories) — source code and ongoing work.

---

## `03 / EXPERIENCE`

| Role | Organisation | What I worked on |
|---|---|---|
| **Full-Stack Developer Intern** · Sep 2025 – Feb 2026 | **Study Brainz** · Remote | Django backend, PostgreSQL schema design, transaction-safe appointment workflows, dashboard query optimisation, pytest coverage, and a Django-served computer-vision classifier. |
| **Electrical Engineering Intern** · May 2023 – Jun 2023 | **Yadav Electrical Works** · Kolhapur | Assisted with residential / commercial wiring and distribution boards; prepared single-line diagrams and wiring layouts; supported load calculations, cable sizing, BOQs, and electrical testing. |

The electrical internship gave me practical exposure to site execution, switchgear termination, MCB / RCCB selection, earthing, continuity testing, insulation-resistance testing, and site safety procedures.

---

## `04 / RESEARCH & PUBLICATIONS`

| Work | Contribution / recognition |
|---|---|
| **Synergy of OFDMA and NOMA in Modern Wireless Communication** · Apr 2025 | Published research paper, **MAT-Journals**. |
| **OFDM Channel Estimation Under Channel Mismatch** · 2026 | Co-authored manuscript under review at **Elsevier Physical Communication**. |
| **Drone Detection: Differentiating Spy UAVs from Birds** · Mar 2025 | **1st Place**, National Paper Presentation, **IMPULSE 2K25**. |
| **Research Paper Award** · TKIET Tech Fest 2025 | Best Research Paper Award. |

**Other recognition:** 7+ first-place finishes at national-level technical paper presentations, covering wireless communications, defence technology, and applied engineering topics.

---

## `05 / TECHNICAL STACK`

The badges below reflect tools and technologies used across my projects, internship, coursework, and research — not a claim of equal depth in every tool.

**Languages & backend**

<p>
  <img src="https://img.shields.io/badge/Python-111827?style=for-the-badge&logo=python&logoColor=70F6F0" alt="Python" />
  <img src="https://img.shields.io/badge/Django-111827?style=for-the-badge&logo=django&logoColor=70F6F0" alt="Django" />
  <img src="https://img.shields.io/badge/SQL-111827?style=for-the-badge&logo=postgresql&logoColor=70F6F0" alt="SQL" />
  <img src="https://img.shields.io/badge/PostgreSQL-111827?style=for-the-badge&logo=postgresql&logoColor=70F6F0" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/MySQL-111827?style=for-the-badge&logo=mysql&logoColor=70F6F0" alt="MySQL" />
  <img src="https://img.shields.io/badge/SQLite-111827?style=for-the-badge&logo=sqlite&logoColor=70F6F0" alt="SQLite" />
  <img src="https://img.shields.io/badge/pytest-111827?style=for-the-badge&logo=pytest&logoColor=70F6F0" alt="pytest" />
</p>

**Machine learning & document intelligence**

<p>
  <img src="https://img.shields.io/badge/PyTorch-111827?style=for-the-badge&logo=pytorch&logoColor=FF69C8" alt="PyTorch" />
  <img src="https://img.shields.io/badge/scikit--learn-111827?style=for-the-badge&logo=scikitlearn&logoColor=FF69C8" alt="scikit-learn" />
  <img src="https://img.shields.io/badge/NumPy-111827?style=for-the-badge&logo=numpy&logoColor=FF69C8" alt="NumPy" />
  <img src="https://img.shields.io/badge/Pandas-111827?style=for-the-badge&logo=pandas&logoColor=FF69C8" alt="Pandas" />
  <img src="https://img.shields.io/badge/FAISS-111827?style=for-the-badge" alt="FAISS" />
  <img src="https://img.shields.io/badge/llama.cpp-111827?style=for-the-badge" alt="llama.cpp" />
  <img src="https://img.shields.io/badge/Tesseract_OCR-111827?style=for-the-badge&logo=google&logoColor=FF69C8" alt="Tesseract OCR" />
</p>

**Embedded, electronics & communications**

<p>
  <img src="https://img.shields.io/badge/Embedded_C-111827?style=for-the-badge&logo=c&logoColor=70F6F0" alt="Embedded C" />
  <img src="https://img.shields.io/badge/C++-111827?style=for-the-badge&logo=cplusplus&logoColor=70F6F0" alt="C++" />
  <img src="https://img.shields.io/badge/ESP32-111827?style=for-the-badge&logo=espressif&logoColor=70F6F0" alt="ESP32" />
  <img src="https://img.shields.io/badge/GNSS-111827?style=for-the-badge&logoColor=70F6F0" alt="GNSS" />
  <img src="https://img.shields.io/badge/OFDM%20%2F%20NOMA-111827?style=for-the-badge&logoColor=70F6F0" alt="OFDM and NOMA" />
  <img src="https://img.shields.io/badge/IMU%20Sensor%20Fusion-111827?style=for-the-badge&logoColor=70F6F0" alt="IMU sensor fusion" />
  <img src="https://img.shields.io/badge/Software--Defined%20Radio-111827?style=for-the-badge&logoColor=70F6F0" alt="Software-defined radio" />
</p>

**Tools & engineering practice**

<p>
  <img src="https://img.shields.io/badge/Git-111827?style=for-the-badge&logo=git&logoColor=FFFFFF" alt="Git" />
  <img src="https://img.shields.io/badge/Linux-111827?style=for-the-badge&logo=linux&logoColor=FFFFFF" alt="Linux" />
  <img src="https://img.shields.io/badge/Jupyter-111827?style=for-the-badge&logo=jupyter&logoColor=FFFFFF" alt="Jupyter" />
  <img src="https://img.shields.io/badge/AutoCAD-111827?style=for-the-badge&logo=autodesk&logoColor=FFFFFF" alt="AutoCAD" />
</p>

---

## `06 / EDUCATION & LEADERSHIP`

**D. Y. Patil School of Engineering and Management — Kolhapur**  
B.Tech, Electronics & Telecommunication · Minor in Data Science · **8.60 / 10 CGPA**  
Jun 2024 – May 2027

**Dr. Bapuji Salokhe Institute of Engineering & Technology — Kolhapur**  
Diploma in Electrical Engineering · **77%**  
Jun 2021 – May 2024

**Leadership and communication**

- **Documentation Head**, DYPSEM E-Cell — contributed to documentation and student entrepreneurship activities.
- **Model United Nations** — participated as a delegate and chairperson, developing research, structured argumentation, and public-speaking skills.

---

## `07 / OUTSIDE THE BUILD LOG`

I collect interesting vocabulary, enjoy a good technical rabbit hole, and spend a questionable amount of time trying to make progress in **Elden Ring**. Model UN and paper presentations keep the communication side of engineering active; building and breaking prototypes keeps the technical side honest.

---

## `08 / CONTACT`

Open to **2027 graduate opportunities and internships** in Python backend development, applied ML / document intelligence, and embedded or wireless systems.

<p align="center">
  <a href="https://www.linkedin.com/in/rishi-dulhani-397987360/"><img src="https://img.shields.io/badge/CONNECT_ON_LINKEDIN-70F6F0?style=for-the-badge&logo=linkedin&logoColor=08111F" alt="Connect on LinkedIn" /></a>
  <a href="mailto:rishidulhani7070@gmail.com"><img src="https://img.shields.io/badge/EMAIL_ME-FF69C8?style=for-the-badge&logo=gmail&logoColor=10111C" alt="Email Rishi" /></a>
  <a href="tel:+919096780763"><img src="https://img.shields.io/badge/CALL_%2B91_90967_80763-70F6F0?style=for-the-badge" alt="Call +91 90967 80763" /></a>
</p>

<p align="center">
  Direct: <a href="tel:+919096780763">+91 90967 80763</a> &nbsp; | &nbsp; <a href="mailto:rishidulhani7070@gmail.com">rishidulhani7070@gmail.com</a> &nbsp; | &nbsp; <a href="https://www.linkedin.com/in/rishi-dulhani-397987360/">LinkedIn</a>
</p>

<p align="center">
  <sub><strong>RISHI DULHANI</strong> &nbsp; // &nbsp; Electronics × Software × Intelligence</sub><br />
  <sub>Build it. Measure it. Break it. Make it better.</sub>
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:070B18,50:15243A,100:341A45&height=4&section=footer" width="100%" alt="Neon footer divider" />
</p>

