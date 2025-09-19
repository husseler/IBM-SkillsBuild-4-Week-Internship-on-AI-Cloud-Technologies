# IBM SkillsBuild 4-Week Internship on AI & Cloud Technologies

This repository documents the capstone project completed during the IBM SkillsBuild 4-Week Internship on AI & Cloud Technologies. This program is a collaborative initiative by the Edunet Foundation, AICTE, and IBM SkillsBuild.

The internship's primary goal is to provide hands-on experience in emerging technologies, enhancing employability and confidence by solving real-world challenges using the IBM SkillsBuild and IBM Cloud platforms.

📝 **Table of Contents**

- Intern Details
- About the Internship
- Project: Nutrition Agent — The Smartest AI Nutrition Assistant
- Problem Statement
- Solution Overview
- ⚙️ Technology Stack
- 🚀 Project Workflow
- 📊 Results
- 📁 Repository Contents

---

## 👨‍💻 Intern Details

**Name:** Harsh Suryavanshi  

**Institute:** Shri Govindram Seksaria Institute of Technology & Science, Indore — Information Technology

**Duration** 4Weeks (15th July 2025 to 7th August 2025)

---

## 📖 About the Internship

This 4-week program focused on practical skills in AI and Cloud Computing. The internship was structured with weekly virtual sessions, mentor guidance, and hands-on labs. The curriculum included orientation to IBM Cloud, core AI concepts, hands-on labs, and practical deployment on IBM Cloud services. Successful completion required active participation, completion of required courses on IBM SkillsBuild, and the submission of a final project presentation.

---

## 💡 Project: Nutrition Agent — The Smartest AI Nutrition Assistant

### Problem Statement (No. 8 — Nutrition Agent)
**The Challenge** — In an era where health awareness is growing, individuals increasingly seek personalized nutrition guidance. However, most existing tools provide generic diet plans, lack real-time adaptability, and fail to consider a person's holistic lifestyle, cultural preferences, allergies, and evolving health conditions. Furthermore, dieticians and nutritionists face limitations in scaling personalized consultations due to time and resource constraints.

Generative AI presents a groundbreaking opportunity to revolutionize this space by enabling an intelligent, interactive, and adaptive virtual nutrition assistant. By leveraging natural language processing (NLP), multimodal understanding, and large-scale dietary databases, an AI-powered assistant can generate dynamic meal plans, recommend smart food swaps, and explain nutritional choices — all tailored to the individual.

**This project aims to develop _“The Smartest AI Nutrition Assistant”_ that:**
- Understands user inputs via text, voice, or image (e.g., food photos, grocery labels).  
- Generates personalized meal plans based on health goals, medical conditions, fitness routines, and preferences.  
- Offers contextual explanations (e.g., “Why is this food better?”).  
- Adapts suggestions dynamically with continuous feedback.

By integrating health data, food databases, and LLM-powered reasoning, the solution bridges the gap between one-size-fits-all diet apps and in-person nutrition counselling — delivering an AI that thinks, learns, and cares like a real nutrition expert.

> **Mandatory:** Use of IBM Cloud Lite services and IBM Granity (watsonx agent) is required for this project.

---

## Solution Overview

An end-to-end, agent-driven system was created to accept multimodal inputs (text, voice, images), reason about nutrition and user constraints (allergies, cultural preferences, goals), and return adaptive meal plans plus short, human-friendly explanations. The agent combines:

- Multimodal preprocessing (OCR for labels, image-to-food detection, voice→text)  
- Nutrition knowledge base (food nutrition facts, portion mappings)  
- Agentic LLM reasoning (Granity / watsonx agent) to plan meals, make swaps, and explain choices  
- A lightweight backend/API and a simple frontend demo for real-time interactions

---

## ⚙️ Technology Stack

- **Cloud Platform:** IBM Cloud (Lite)  
- **Agent / LLM tooling:** IBM Granity / watsonx agent lab (watsonx.ai)  
- **NLP & multimodal:** Watson components + small CV/OCR models  
- **Language / Libraries:** Python (core), optional JavaScript for UI  
- **Storage:** IBM Cloud Object Storage (Lite)  
- **Other:** Small calculator utilities for macro computations; optional image recognition model

---

## 🚀 Project Workflow

1. **Collect inputs** — user profile (age, sex, weight, height, activity), preferences, allergies, goals; accept images/voice/text.  
2. **Preprocess** — normalize units, run OCR on labels, detect food items, map to nutrition DB.  
3. **Agent design** — craft instruction set and tool integrations in Granity to enforce nutrition rules and personalization.  
4. **Reasoning & generation** — agent composes meal plans (3 meals + snacks), estimates macros, suggests swaps and explains choices.  
5. **Deployment** — package and publish the agent as an online endpoint on IBM Cloud Lite.  
6. **Frontend/back-end** — simple backend (Flask/Node) forwards normalized queries to the agent; frontend demo allows multimodal input and feedback.  
7. **Iterate & evaluate** — gather user feedback and refine prompts, tools, and data mappings.

---

## 📊 Results

The deployed Nutrition Agent provides:
- Personalized meal plans honoring user constraints (allergies, preferences, goals).  
- Explanations for each recommendation and suggested substitutions.  
- A demonstration-ready API endpoint for real-time interactions (deployed on IBM Cloud Lite).

(If you run user tests, add numeric metrics here: user satisfaction, constraint-respect rate, response latency, etc.)

---

## 📁 Repository Contents

- `README.md` — Project overview and instructions (this file).  
---

## How to run (high-level)

1. Create an IBM Cloud Lite account and enable required services (Cloud Object Storage, watsonx / Granity).  
2. Upload sample datasets to Cloud Object Storage.  
3. Configure an agent in Granity / watsonx with instruction sets and tool hooks (nutrition DB, OCR).  
4. Deploy agent and obtain the REST endpoint + API key.  
5. Update `src/backend/app.py` with your endpoint and API key, run the backend.  
6. Start the frontend and test multimodal inputs; provide feedback to the agent.

---

## Acknowledgements & References

- IBM SkillsBuild, Edunet Foundation & AICTE  
- IBM watsonx / Granity documentation  
- IBM Cloud Object Storage docs  
- Public nutrition datasets and OCR/CV resources

---
## Cerificates 
![Certifications01](https://github.com/husseler/IBM-SkillsBuild-4-Week-Internship-on-AI-Cloud-Technologies/blob/main/Certifications/ICOC.png)

![Certifications02](certifications/JTC.png)

![Certifications03](certifications/GSWAI.png)




**Prepared by Harsh Suryavanshi — Nutrition Agent Project**
