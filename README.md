# Smart Inspection & Monitoring System (OIML R-76)
### By Team CODIFY

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
Our solution is an advanced digital platform designed to transform the manual weighing-instrument evaluation process into a streamlined, automated, and AI-assisted digital workflow. Built for modern metrology, it enforces strict compliance with the **OIML R-76** standard while providing offline-first capabilities, intelligent anomaly detection, and tamper-proof report generation.

## 🎯 Core Solutions (Key Deliverables)
* **Profiling & Parameterization:** Captures essential data of instruments (Maps accuracy classes), automatically generates load steps, and rigorously tests the data.
* **OIML R-76 Obs Matrix:** A digital data entry form that meticulously checks and notes laboratory environmental conditions.
* **Field Inspection & Evidence:** 
  * **Geo-fence Mechanism:** Validates on-site evidence capture.
  * Geo-tagged inspection reports and live evidence capture.
* **Evidence Anomaly Detection:** Utilizes OCR-based comparison of captured field evidence against submitted documents to instantly detect mismatches, missing fields, and inconsistencies.

## 💻 Technical Approach & Architecture

### 1. Application Layer
* **Desktop Application:** Built with the Electron Framework (Windows / Linux / macOS).
* **Web Application:** Hosted securely (Vercel / Render).
* **Core Engine:** Offline-first architecture with **AES-256 Encrypted Local Storage** (SQLite).
* **RAG Assistant:** Powered by Ollama & ChromaDB for source-grounded R-76 knowledge guidance, contextual procedure support, and technical assistance.

### 2. Backend Services
* **REST API Layer:** Built on Node.js and Express.js, secured via JWT to handle application requests, authentication, and data processing.
* **OIML R-76 Rules Engine:** Dynamic rule configuration (JSON/YAML) for Maximum Permissible Error (MPE) calculations and compliance determination.
* **Business Logic & Media:** Handles data validation, test sequence processing, and document/photo uploads.
* **Data Storage:** MongoDB, Redis, and Amazon S3.

### 3. AI / ML Services
* **Nameplate OCR & Document Validation:** Extracts instrument details and compares them with manual entries to detect discrepancies.
* **Voice Input (Hands-Free):** Web Speech API / Whisper integration to convert speech to structured fields, dramatically improving lab workflow.
* **Measurement Anomaly Detection:** Hugging Face and Scikit-learn models detect unusual patterns and alert technicians for review via XAI (Explainable AI).

## 👥 Users & Inputs
The system supports distinct role-based access for the metrology workflow:
1. **Lab Technician:** Responsible for data entry (instrument details, environmental conditions like temp/humidity/pressure, test observations, and photographs).
2. **Metrology Evaluator:** Reviews anomalies and approves the final test observations.
3. **Administrator:** Handles comprehensive user and system management.

## 📊 Output, Integration & Verification
* **Generated Reports:** Exportable in PDF (Standard OIML R-76), DOCX (Editable), and JSON/XML (Machine Readable format).
* **Dashboard & History:** Complete test report management, fast search & retrieval, and role-based access controls.
* **Verify & Sharing:** 
  * Public verification links
  * Tamper-proof reports
  * Cryptographic QR codes
  * Digital Signatures

## 🚀 Impact & Benefits
* **Faster Reporting:** Automated calculations reduce manual processing time significantly.
* **Improved Accuracy:** Rule-based calculations completely eliminate manual human calculation errors.
* **Regulatory Transparency:** Makes test results, evaluations, and report history universally traceable.
* **Scalable Testing:** Seamlessly supports multiple instruments, unlimited users, and future rule versions.
* **Easy Data Access & Traceable Workflow:** Centralized storage maintains test history and audit records for better traceability.
* **Future-Ready Infrastructure:** Creates a solid foundation for analytics, AI-assisted testing, and digital laboratories.