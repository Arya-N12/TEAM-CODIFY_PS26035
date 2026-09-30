# Inspex - Smart Inspection & Monitoring System (OIML R-76)
### By Team CODIFY (158210)

[![YouTube Presentation](https://img.shields.io/badge/YouTube-Video_Presentation-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtu.be/AnqudR6177E?si=J5--I8Wi2eW79oS6)
[![Live Website Prototype](https://img.shields.io/badge/Website-Live_Prototype-0052FF?style=for-the-badge&logo=vercel&logoColor=white)](https://drishti360.onrender.com/)
[![Download APK](https://img.shields.io/badge/APK-Download_Prototype-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://drive.google.com/file/d/1QRNk6M1IF1ViZFZCOvNc_yqt1804pk-p/view?usp=sharing)

---

## 👥 Team CODIFY

| Name | Role / Contribution |
|------|--------------------|
| **Arya Pritam Nangude** | Backend Developer |
| **Gayatri Mukchand Karkhile** | Backend Developer |
| **Sakib Samir Tamboli** | AI/ML Developer |
| **Atreya Ashish Kshirsagar** | Frontend UI/UX & RAG Model Developer |
| **Jiya Irfan Shahadivan** | Android/Kotlin Developer |
| **Kapil Chandrashekhar Sorte** | Flutter Developer |

---

## 📌 Project Overview
Inspex is an advanced digital platform designed to transform the manual weighing-instrument evaluation process into a streamlined, automated, and AI-assisted digital workflow. Built for modern metrology, it enforces compliance with the **OIML R-76** standard while providing offline-first capabilities, intelligent anomaly detection, and tamper-proof report generation.

## 🎯 Core Solutions
* **Profiling & Parameterization:** Captures essential data of instruments (accuracy classes), automatically generates load steps, and rigorously tests the data.
* **OIML R-76 Obs Matrix:** Digital data entry form that checks and notes laboratory environmental conditions.
* **Field Inspection & Evidence:** 
  * Geo-fence mechanism to validate on-site evidence capture.
  * Geo-tagged inspection reports and live evidence capture.
* **Evidence Anomaly Detection:** OCR-based comparison of captured field evidence with submitted documents to immediately detect mismatches, missing fields, and inconsistencies.

## 💻 Technical Architecture
### Application Layer
* **Desktop Application:** Electron Framework (Windows / Linux / macOS)
* **Web Application:** React / Next.js (Hosted on Vercel/Render)
* **Core Engine:** Offline-first architecture with AES-256 Encrypted Local Storage (SQLite)
* **RAG Assistant:** Powered by Ollama & ChromaDB for source-grounded R-76 knowledge guidance, contextual procedure support, and technical assistance.

### Backend & Services
* **REST API Layer:** Built on Node.js and Express.js, secured via JWT.
* **OIML R-76 Rules Engine:** Dynamic rule configuration (JSON/YAML) for MPE calculations and compliance determination.
* **Database & Storage:** MongoDB, Redis, and Amazon S3.

### AI / ML Integrations
* **Nameplate OCR & Document Validation:** Extracts instrument details and detects manual entry discrepancies.
* **Voice Input (Hands-Free):** Web Speech API / Whisper integration to convert speech to structured fields, drastically improving lab workflow.
* **Measurement Anomaly Detection:** Hugging Face and Scikit-learn models used to detect unusual patterns and alert technicians for review via XAI (Explainable AI).

## 👥 Users & Workflows
1. **Lab Technician:** Responsible for data entry, capturing photographs (instrument readings), and recording environmental conditions (Temperature, Humidity, Pressure).
2. **Metrology Evaluator:** Reviews anomalies and approves the final test observations.
3. **Administrator:** Handles comprehensive user and system management.

## 📊 Output & Verification
* **Generated Reports:** Available in PDF (Standard OIML R-76), DOCX (Editable), and JSON/XML (Machine Readable).
* **Verify & Sharing:** 
  * Public verification links
  * Tamper-proof reports utilizing Cryptographic QR codes
  * Digital Signatures

## 🚀 Impact & Benefits
* **Faster Reporting:** Automated calculations reduce manual processing time.
* **Improved Accuracy:** Rule-based calculations completely eliminate manual human errors.
* **Regulatory Transparency:** Makes test results, evaluations, and report history universally traceable.
* **Scalable Testing:** Seamlessly supports multiple instruments, unlimited users, and future rule versions.