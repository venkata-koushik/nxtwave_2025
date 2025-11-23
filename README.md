# 🌊 AapdaSetu: The Disaster Management and Response System

> **AI-powered unified platform bridging the information-to-action gap for proactive disaster response.**

## 1. Project Summary & Problem Statement
## 2. Solution: AapdaSetu & Target Audience
## 3. Core Features & MVP Architecture
## 4. Realistic Impact and Usefulness
## 5. Citizen Usage Guide
## 6. Team Rakshak

---

### **1. Project Summary & Problem Statement**

The core challenge AapdaSetu addresses is the **significant information-to-action gap** in disaster management.  
Currently, data exists in distributed fragments (weather forecasts, ground reports, historical records), but it's not synthesized into timely, actionable intelligence for authorities and citizens.

* **Pre-Disaster Gap**: There is a lack of precise, hyperlocal, and context-aware early warnings.  
* **Post-Disaster Gap**: Authorities struggle with a real-time, consolidated view of the ground reality and do not know how to prioritize resource allocation efficiently.

---

### **2. Solution: AapdaSetu & Target Audience**

AapdaSetu ("Bridge of Disaster Relief") is an AI-powered, unified web platform designed for smart Pre and Post Disaster Management.

| Portal | Target User | Primary Role |
| :--- | :--- | :--- |
| **Citizen Portal** | Residents/Public | Receive personalized safety alerts, track status, and request help. |
| **Admin Portal** | Government Authorities/Officials | Get AI-driven predictions & resource suggestions, analyze missions, and send targeted alerts. |

---

### **3. Core Features & MVP Architecture**

The system provides intelligent insight generation at the end of both the user and government process.

| Feature | Description | Mechanism |
| :--- | :--- | :--- |
| **Proactive AI Warnings** | Prediction of disaster through historic data analysis. | Hybrid Data Ingestion & Asynchronous AI Processing Engine. |
| **Human-in-the-Loop (HITL)** | For critical alerts, the system requires a human operator's final confirmation before broadcasting. | Prevents mass panic caused by AI-automated inaccurate critical alerts. |
| **Realtime Map & Resource Management** | Live Interactive Map for visualizing the situation and optimizing resource allocation. | Real-time Update on Active Map. |
| **Chatbot Guidance** | Citizens receive guidance from an AI Chatbot. | AI-powered Chatbot recommends the Help Response. |

**Technical Stack Highlights (MVP Focus)**  
The MVP uses **Vanilla HTML, CSS, and JavaScript** with **Bootstrap 5**, and relies on the **Supabase** backend (replacing custom Node.js) for high-speed **Authentication** and **Realtime** capabilities.  
**ChatGPT-4o** is integrated for data structuring and analysis.

---

### **4. Realistic Impact and Usefulness**

AapdaSetu ensures the shift from a reactive response to proactive mitigation, leading to significant benefits:

| Impact Area | Benefit | Real-World Usefulness |
| :--- | :--- | :--- |
| **Social** | Builds Resilient Communities. | Immediate Safety Alerts right where citizens are, drastically reducing loss of life. |
| **Economic** | Minimizes Financial Damage. | Early warnings and efficient response protect critical infrastructure and property. |
| **Operational** | Optimizes Resource Allocation. | Ensures limited resources like rescue teams and medical aid are allocated to the areas of greatest need. |

---

### **5. Citizen Usage Guide**

AapdaSetu is designed to provide immediate safety alerts and actionable instructions to citizens with minimal steps.

**Receiving an Alert (Pre-Disaster/In-Crisis)**

1. **Personalized Alert**: As a logged-in resident, you will instantly receive a **personalized safety alert** based on your location.  
2. **Actionable Steps**: The alert card provides a brief description and a checklist of **AI-enhanced safety recommendations** (e.g., "Charge Phones," "Secure Gas Valves").  
3. **Track Status**: You can track the status and updates of the active alert.

**Requesting Help (During/Post-Disaster)**

1. **Access Help**: Click the 'Report Status and Request Help' button on the portal.  
2. **Auto-Fetch Location**: The system automatically uses your device's **GPS API** to fetch your current location.  
3. **Categorize Emergency**: Select the category of your emergency (e.g., Flood, Medical, Infrastructure).  
4. **AI Chatbot Guidance**: Get guidance from the **AI-powered Chatbot**. The Chatbot processes your query and the current disaster context to provide a recommendation of the appropriate help response.  
5. **Submission**: Your report is submitted to the Admin portal, where it is instantly visualized on the Live Map for response coordination.

---

### **6. Team Rakshak**

| Role | Name |
| :--- | :--- |
| **Leader** | Mayank Aryan |
| **Member** | Ayush Kashyap |
| **Member** | Venkata Koushik |
| **Member** | Aditya Suman |
