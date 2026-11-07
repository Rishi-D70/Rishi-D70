<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0b132b,50:1c2541,100:3a506b&height=200&section=header&text=Rishi%20Dulhani&fontSize=62&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Embedded%20Systems%20%7C%20Signal%20Processing%20%7C%20Applied%20ML&descAlignY=62&descSize=17" width="100%" alt="header"/>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=21&pause=1300&color=5BC0BE&center=true&vCenter=true&width=640&lines=Signals+lie.+I+build+things+that+catch+them.;GNSS+spoofing+detection+on+an+RC+car;CNN+vs+MMSE+in+OFDM%2C+tested+under+mismatch;Offline+AI+that+reads+contracts" alt="typing intro"/>
</p>

<p align="center">
  <a href="YOUR_LINKEDIN_URL"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:YOUR_EMAIL"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

---

## 👋 About me

Final-year B.Tech student in **Electronics and Telecommunication** with a **Data Science minor**, at DYPSEM, Kolhapur. CGPA 8.60.

I work where radio, hardware and machine learning overlap. A GPS fix, a wireless channel and a 60-page contract look nothing alike, but all three can be wrong in ways that are hard to notice. I like building the part that notices.

I've always been pulled toward defense technology, which is why my capstone is about catching fake GPS.

---

## 🛰️ Currently building: GPS spoofing detection

**GPS Spoofing Detection using Low-Cost GNSS and IMU Sensor Fusion**
Embedded Systems and GNSS Navigation Security. Built with a team of four (Vansh Limbad, Rajvardhan Mohite, Hrushiraj Yadav and me), guided by Dr. Aarti A. Chavan.

The idea: a fake GPS signal can show a believable position, but it can't fake how the vehicle is actually moving. So the detector checks if what GNSS claims matches what the motion sensor feels.

```mermaid
flowchart LR
    A["u-blox NEO-M9N<br/>GNSS fix"] --> B["Attacker ESP32<br/>edits data in transit"]
    B --> C["Detector ESP32-S3"]
    D["IMU<br/>motion reference"] --> C
    C --> E{"Does GNSS agree<br/>with real motion?"}
    E -->|Yes| F["Clean"]
    E -->|No| G["Spoof flagged<br/>by ML classifier"]
```

| | |
|---|---|
| **Detector** | ESP32-S3 with a NEO-M9N GNSS receiver and an IMU, logging to SD |
| **Attacker** | A second ESP32 sitting in the data path, started wirelessly from a laptop |
| **Test bench** | The whole block rides on an RC car in a box enclosure that fits most cars |
| **Attack scenarios** | Three, each with its own LED signature on the attacker |
| **Training data** | Attacks are injected with randomized values inside bounds taken from published spoofing research (TEXBAT), so the model learns the attack and doesn't memorize a formula |
| **Status** | In active build. Code and write-up will land here after the demo |

---

## 📡 Research: when learned channel estimators meet the real world

Co-authored with Dr. Sutar. **CNN vs MMSE channel estimation in OFDM under distribution mismatch.**

Neural estimators look great when test conditions match training. This paper asks what happens when they don't, and introduces two metrics to measure it:

- **Robustness Ratio**: how much of its performance an estimator keeps when conditions shift
- **Effective SNR Loss**: how many dB of signal quality the mismatch effectively costs

Manuscript in progress, aimed at Elsevier's *Physical Communication*.

---

## 🔧 Things I've shipped

| Project | What it does | Numbers |
|---|---|---|
| [**Project-IQ**](https://github.com/Rishi-D70/Project-IQ) | Reads contracts and policies fully offline and pulls out clauses, obligations, dates and parties. Nothing leaves your machine. | Qwen2.5-7B (4-bit) on llama.cpp with FAISS retrieval. **0.81 precision, 0.74 recall** on 50 CUAD contracts |
| [**Fly-High-Index**](https://github.com/Rishi-D70/Fly-High-Index) | Smart India Hackathon 2026 team project on a real-time airfare price index for India | Team build |
| **Hospital Management System** | Full backend built during my internship at Study Brainz | Django and PostgreSQL, 8 models, **24 pytest tests** |
| **Cattle Breed Classifier** | Image classifier for Indian cattle breeds | MobileNetV2, about 2,600 images, 10 breeds, **82% accuracy** |
| [**Simple_Py_Projects**](https://github.com/Rishi-D70/Simple_Py_Projects) | Small Python builds where I test ideas fast | |

---

## 🧰 Toolkit

**Embedded and signals**
![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=for-the-badge&logo=espressif&logoColor=white)
![GNSS](https://img.shields.io/badge/GNSS-1c2541?style=for-the-badge)
![Sensor Fusion](https://img.shields.io/badge/Sensor%20Fusion-3a506b?style=for-the-badge)
![OFDM](https://img.shields.io/badge/OFDM-0b132b?style=for-the-badge)

**ML and data**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![llama.cpp](https://img.shields.io/badge/llama.cpp-000000?style=for-the-badge)
![FAISS](https://img.shields.io/badge/FAISS-0467DF?style=for-the-badge)

**Backend**
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

---

## 🎤 Off the keyboard

- **Documentation Head** at the DYPSEM E-Cell, under E-Cell IIT Bombay
- **Model UN** delegate and chairperson. I've argued for Russia in DISEC and for Finland at UNODC
- Two-time paper presentation winner
- I collect vocabulary words, and I'm slowly dying my way through Elden Ring

---

## 📫 Let's talk

I'm looking for internships from January 2027 and fresher roles across Python, ML and data, and embedded or electronics. If you have a problem with a signal you can't trust, I'd like to hear about it.

<p align="center">
  <a href="YOUR_LINKEDIN_URL"><img src="https://img.shields.io/badge/Connect%20on%20LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:YOUR_EMAIL"><img src="https://img.shields.io/badge/Send%20an%20email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:3a506b,100:0b132b&height=110&section=footer" width="100%" alt="footer"/>
