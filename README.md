# 🌊 AapdaSetu: The Disaster Management and Response System

> **AI-powered unified platform bridging the information-to-action gap for proactive disaster response.**

##### 1. Project Summary & Problem Statement
##### 2. Solution: AapdaSetu & Target Audience
##### 3. Core Features & MVP Architecture
##### 4. Realistic Impact and Usefulness
##### 5. Citizen Usage Guide
##### 6. Team Rakshak

---
### **1. Project Summary & Problem Statement**

AapdaSetu is designed to address the critical **information-to-action gap** in disaster management. Currently, crucial data exists in distributed fragments (weather forecasts, historical records, real-time ground reports), but lacks the synthesis needed for timely, actionable intelligence for authorities and citizens.

This inadequacy creates specific challenges:

* **Pre-Disaster Gap**: Authorities lack precise, hyperlocal, and context-aware early warnings necessary for effective preparation.
* **Post-Disaster Gap**: Authorities struggle to achieve a real-time, consolidated view of the ground reality. This directly hinders efficient resource allocation, as specific needs (food, connectivity status, etc.) are unknown.

---
### **2. Solution: AapdaSetu & Target Audience (Expanded)**

AapdaSetu ("Bridge of Disaster Relief") is a unified web platform that leverages AI to structure raw, complex input into intelligent output, facilitating **Smart Pre and Post Disaster Management**.

| Portal | Target User | Primary Role & Intelligence |
| :--- | :--- | :--- |
| **Citizen Portal** | Residents/Public | This portal is crucial for ensuring citizen safety and engagement. Users **receive personalized safety alerts** based on their location. They can **track alert status and updates**, which enhances transparency. Critically, citizens can **report their status and request help** directly through the platform. They also **get guidance from an AI Chatbot**, which assists them in navigating the crisis and categorizing the emergency for submission. |
| **Admin Portal** | Government Authorities/Officials | This portal serves as the command center for data-driven response coordination. Authorities **get AI-driven predictions & resource suggestions** to optimize the distribution of resources. They visualize the situation in real time using the **Live Interactive Map** and **assign and analyse response missions**. This allows them to **send targeted mass alerts to specific zones**, providing a real-time, consolidated view of the ground reality. |

---
### **3. Core Features & MVP Architecture**

The system's feasibility is rooted in its proven tech stack and event-driven architecture, ensuring stability and resilience under extreme load.

| Feature | Description | Mechanism |
| :--- | :--- | :--- |
| **Proactive AI Warnings** | Prediction of major disturbed areas based on historic data analysis with present conditions. | Uses **OpenWeather API** and **IMD Weather API** for data fusion. |
| **Human-in-the-Loop (HITL)** | For high-severity, wide-impact alerts, the system requires a final confirmation from a human operator before public broadcast. | Directly addresses the risk of **AI Automated Inaccurate Critical Alerts** that could cause mass panic. |
| **Realtime Management** | Authorities visualize the situation in real time with an interactive map, enabling data-driven decisions. | Implemented using **Google Map API** and **Supabase Realtime** for instant updates. |
| **Asynchronous AI Engine** | The **n8n** workflow orchestrates automated AI analysis by refining and summarizing raw data. | Utilizes **Google Gemini-boot** and the **Vision API** for image analysis and data structuring. |

**Technical Stack Highlights (MVP Focus)**  
The MVP is built using **Vanilla HTML, CSS, and JavaScript (Bootstrap 5)** to ensure a fast, browser-ready experience. The data layer uses **Supabase** (PostgreSQL) for its built-in **Realtime** feature, essential for instant alert synchronization.

---
### **4. Realistic Impact and Usefulness**

AapdaSetu ensures that government response shifts from reactive to proactive, leading to substantial societal and economic benefits.

| Impact Area | Benefit | Real-World Usefulness |
| :--- | :--- | :--- |
| **Social (Communities)** | Increases preparedness and drastically reduces loss of life. | Provides immediate safety alerts and targeted assistance, building resilient communities. |
| **Economic (Financial)** | Minimizes Financial Damage. | Early warnings protect critical infrastructure and property. |
| **Operational (Response)** | Optimize Resource Allocation. | Ensures limited resources (relief teams, aid, food) are allocated to the areas of greatest need, maximizing operational benefits. |

---
### **5. Citizen Usage Guide**

The Citizen Portal is designed for immediate safety and actionable intelligence, even for users with poor connectivity or low digital literacy.

**Receiving an Alert (Pre-Disaster/In-Crisis)**

1. **Login**: Resident logs in to the unified web platform.
2. **Personalized Alert**: As a logged-in resident, you instantly receive a **personalized safety alert** based on your location (auto-fetched via GPS API).
3. **Actionable Steps**: The alert card provides a brief description and a checklist of **AI-enhanced safety recommendations**.
4. **Track Status**: You can track the alert status and receive continuous updates.

**Requesting Help (During/Post-Disaster)**

1. **Access Help**: Use the portal to report your status and request help.
2. **Auto-Fetch Location**: Your precise location (latitude/longitude) is automatically fetched using the device's **GPS API**.
3. **Categorize Emergency**: Select the specific category of your emergency (e.g., medical, infrastructure, flood).
4. **AI Chatbot Guidance**: Get instant guidance from the **AI Chatbot**. For low-literacy users, a **Voice-Enabled Chatbot** feature can be incorporated for reporting in local languages.
5. **Submission**: Your verified report is instantly submitted to the Admin portal, where it is visualized on the Live Map for emergency response prioritization.

---
### **6. Team Rakshak**

| Role | Name |
| :--- | :--- |
| **Leader** | Mayank Aryan |
| **Member** | Ayush Kashyap |
| **Member** | Venkata Koushik |
| **Member** | Aditya Suman |
