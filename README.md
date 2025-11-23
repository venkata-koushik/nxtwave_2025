# 🌊 AapdaSetu: The Disaster Management and Response System

> **AI-powered unified platform bridging the information-to-action gap for proactive disaster response.** [cite: 4, 17]

![Status](https://img.shields.io/badge/Status-MVP%20Complete-brightgreen)
[cite_start]![Theme](https://imgles.io/badge/Theme-AI%20for%20Societal%20Good-red) [cite: 2]
[cite_start]![Team](https://img.shields.io/badge/Team-Rakshak-darkviolet) [cite: 9]
[![Demo](https://img.shields.io/badge/Demo-Watch%20Video-ff69b4)]([INSERT_DEMO_VIDEO_LINK_HERE])

---

## 🎯 The Core Problem: The Information-to-Action Gap

[cite_start]Currently, data in disaster management exists in distributed fragments (weather forecasts, ground reports, historical records), but it is not synthesized into **timely, actionable intelligence** for authorities and citizens[cite: 5].

This results in two major challenges:

* [cite_start]**Pre-Disaster**: Lack of precise, hyperlocal, and context-aware early warnings[cite: 6].
* [cite_start]**Post-Disaster**: Authorities struggle to obtain a real-time, consolidated view of ground reality, making it impossible to prioritize resource allocation efficiently[cite: 7, 8]. [cite_start]They often don't know which specific area needs food or where connectivity is down[cite: 8].

---

## 💡 AapdaSetu: Our AI Solution

[cite_start]AapdaSetu ("Bridge of Disaster Relief") is a unified web platform that uses AI to transform raw, fragmented data into structured, intelligent insights for disaster mitigation and response[cite: 17, 23].

### [cite_start]**Target Audience & Portals** [cite: 17]

The system provides two distinct, customized portals:

| Portal | Target User | Key Functionality |
| :--- | :--- | :--- |
| [cite_start]**Citizen Portal** [cite: 26] | Residents/Public | [cite_start]Receive **personalized safety alerts**, track alert status, report their status, and get guidance from an **AI Chatbot**[cite: 27, 28, 29, 30]. |
| [cite_start]**Admin Portal** [cite: 31] | Government Authorities/Officials | [cite_start]Access **AI-driven predictions**, view the **Live Interactive Map**, assign response missions, and send **targeted mass alerts** to specific zones[cite: 32, 33, 34, 35]. |

---

## 🚀 Key Features & MVP Architecture

[cite_start]The MVP (Minimum Viable Product) is built on a high-speed, scalable architecture designed specifically for crisis-level stability[cite: 63].

### **Core AI-Driven Features**

1.  [cite_start]**Proactive AI Warnings**: Prediction of disasters through historic data analysis combined with real-time conditions[cite: 20, 24].
2.  [cite_start]**Data-Driven Resource Allocation**: AI provides suggestions for resource deployment (relief teams, aid, food) and response prioritization[cite: 21, 32, 36].
3.  [cite_start]**Human-in-the-Loop (HITL)**: For high-severity, wide-impact alerts, the system requires a final confirmation from a human operator before broadcasting to the public[cite: 73]. [cite_start]This mitigates the critical risk of **AI Automated Inaccurate Critical Alerts** that could cause mass panic[cite: 72].
4.  [cite_start]**Asynchronous AI Processing**: An **n8n** automation workflow leverages **ChatGPT4-o** and the Vision API for rapid data extraction, summarization, and structuring of raw reports[cite: 42, 51].

### **Technical Stack Highlights (MVP Focus)**

To ensure a fast, resilient, and simple MVP deployment, we utilized the following core stack:

| Component | Technology | Role in MVP |
| :--- | :--- | :--- |
| **Frontend** | Vanilla JS, Bootstrap 5 | [cite_start]Lightweight, instant-loading interface[cite: 39]. |
| **Backend/DB** | **Supabase** (Replacing custom Node/MongoDB for MVP) | [cite_start]Provides highly available **Database, Authentication, and Realtime WebSockets** for instant alert synchronization[cite: 41, 49]. |
| **AI/Automation** | **n8n, ChatGPT4-o, Vision API** | [cite_start]The "Brain" for intelligent insight generation and automated analysis[cite: 42, 51]. |
| **Alerts** | **Twilio API** | [cite_start]Sends alerts directly through messaging[cite: 44, 46]. |

---

## 🌎 Realistic Impact and Usefulness

AapdaSetu directly addresses the societal need for resilience and efficient crisis response.

### **Impact on Citizens (Social Benefit)**
* **Faster, Targeted Assistance**: Citizens get help faster by reporting issues directly and receiving guidance from the AI Chatbot[cite: 81, 30].
* **Reduced Loss**: Early warnings and personalized safety steps reduce personal and property loss.

### **Impact on Government (Economic & Operational Benefit)**
* **Proactive Mitigation**: Allows the shift from a reactive response to proactive mitigation using AI-driven insights.
* **Optimized Resource Allocation**: Ensures limited resources (like rescue teams and medical aid) are allocated to the areas of greatest need, minimizing financial damage and maximizing operational benefit.
* **Increased Accountability**: A transparent, data-driven system increases public trust.

---

## Team Rakshak


| **Leader** | Mayank Aryan  |

| **Member** | Ayush Kashyap |

| **Member** | Venkata Koushik  |

| **Member** | Aditya Suman  |

| Column 1 | Column 2 | Column 3 |

|----------|----------|----------|

| Row 1    | Data     | Value    |

| Row 2    | Data     | Value    |

| Row 3    | Data     | Value    |
