1. Introduction

During natural disasters—whether cyclones, floods, landslides, or earthquakes—the time between receiving information and taking action is often too long.
Authorities rely on fragmented data from different sources, and citizens rarely receive personalized, verified, and actionable guidance.

AapdaSetu was built to directly solve this problem.

It provides:

An early-warning prediction model using AI

Hyperlocal citizen alerts

A real-time authority dashboard

AI-generated safety checklists

A verification pipeline to prevent misinformation

Dynamic handling of severe-load scenarios using event-driven systems

The system’s goal is simple:
Bridge information → into action → as fast as possible.

2. Motivation and Problem Background

Disaster management today faces several structural challenges:

Fragmented Information Sources

Weather APIs, ground reports, historical datasets, and sensor readings are not integrated into a single platform. This slows down response time.

Lack of Real-Time Visibility

Authorities lack a consolidated view of:

Affected areas

Severity levels

Resource needs

Citizen requests

This makes prioritization extremely difficult.

Misinformation Risks

Citizens often share unverified news.
Authorities struggle to broadcast accurate alerts quickly without verification.
Slow Two-Way Communication

Most disaster systems push alerts one-way.
Citizens have no simple way to:

Report issues

Ask for help

Provide location-based data

AapdaSetu creates a closed loop disaster management cycle with end-to-end visibility.

3. Core Solution

AapdaSetu is a two-portal, AI-integrated disaster ecosystem:

🟥 Admin Portal

Live dashboard

Risk detection

Trigger or simulate disasters

Review AI-generated intelligence

Approve or modify alerts

Broadcast public alerts

View impact heatmaps

Monitor incoming citizen reports

🟦 Citizen Portal

Receive hyperlocal alerts in real-time

View structured AI-generated safety checklists

Send reports (photos, text, location) to authorities

Access maps and risk zones

Chat with an AI assistant for guidance

The system uses:

Kafka for stream handling

OpenAI for intelligence

WebSockets for live updates

Supabase for database and authentication

n8n automation for pre-processing and heavy trigger flows

4. System Features
1. AI-Generated Disaster Intelligence

Every triggered event passes through an AI pipeline which produces:

Severity score

Expected impact radius

Recommended resources

Summary for citizens

Government-level brief

2. Two-Level Verification (Human-in-the-Loop)

Critical alerts require:

AI assessment

Human approval

This prevents false alarms and misinformation.

3. Real-Time WebSocket Communication

Citizens receive alerts instantly without refresh.

4. Map Overlay & Geo-Tagging

Mark affected zones

Indicate blocked roads

Pin user reports

5. SMS Alerts via Twilio

Citizens without smartphones can be notified.

6. Automated Safety Checklists

Before, during, and after a disaster.

5. Technical Architecture
5.1 High-Level Overview
┌─────────────────────────────────────────────┐
│                 Citizen Portal              │
│  - Alerts                                    │
│  - Checklists                                 │
│  - Reporting (images/text/location)           │
└─────────────────────────┬─────────────────────┘
                          │ WebSocket
                          ▼
    ┌─────────────────────────────────────────┐
    │          Backend (Node + Express)       │
    │  - REST APIs                             │
    │  - WebSockets                             │
    │  - Kafka Producers & Consumers            │
    └─────────────────────────┬─────────────────┘
                              │ Streams
                              ▼
                     ┌────────────────────┐
                     │ AI Processing Unit │
                     │ (OpenAI APIs)      │
                     └────────────────────┘
                              │
                              ▼
        ┌─────────────────────────────────────────┐
        │               Admin Portal              │
        │ - Live Dashboard                         │
        │ - HITL Verification                      │
        │ - Final Broadcast                        │
        └─────────────────────────────────────────┘

5.2 Technology Stack
Component	Technologies
Frontend	HTML, CSS, JavaScript, Bootstrap
Backend	Node.js, Express.js, Apache Kafka
AI	OpenAI ChatGPT-4o, Vision API
DB	Supabase (Auth + DB), MongoDB (Full Build)
Cloud Services	Twilio, OpenWeather,Google Maps
Automation	n8n workflows
Communication	WebSockets
6. Installation Guide
6.1 Prerequisites

Install or configure:

Supabase project

OpenAI API key

n8n automation instance

Google Maps API key

Node.js v18+

Modern browser (Chrome recommended)

6.2 Setup Instructions

Clone the project:

git clone <repo-url>
cd AapdaSetu


Update API keys inside:

/admin.html

/index.html

Run the HTML files directly by opening them in your browser.

7. Usage Documentation
7.1 Admin Portal

The Admin Dashboard enables disaster managers to:

Trigger disaster simulations

Generate AI risk intelligence

Approve alerts

Broadcast crisis notifications

Monitor live WebSocket activity

View citizen reports in real-time

Analyze heatmaps showing disaster spread

7.2 Citizen Portal

Citizens get:

Instant red/yellow alerts

Dynamic checklists

Map of affected regions

Real-time info panels

Simple reporting tools

7.3 Human-in-the-Loop Alert Verification

This process ensures no incorrect critical alert reaches the public.

Workflow:

Admin triggers event → AI analysis begins

AI generates severity, summary, checklist

Alert is PENDING

A modal appears: “Verification Required”

Admin clicks BROADCAST

Citizens receive instant live alert

8. Configuration Options

Environment variables:

SUPABASE_URL=
SUPABASE_ANON_KEY=
OPENAI_API_KEY=
N8N_WORKFLOW_URL=
GOOGLE_MAPS_KEY=
TWILIO_ACCOUNT_ID=
TWILIO_AUTH_KEY=

9. Known Issues and Common Fixes
Problem	Reason	Fix
Map not loading	Wrong API key	Verify Google Maps key
AI not responding	OpenAI quota exceeded	Check API usage
Alerts not updating	WebSocket issue	Restart server
10. Risk Assessment & Mitigation
AI Hallucination

Solved using HITL flow

Strict prompt templates

Server Overload

Kafka handles spikes

Async pipelines

Citizen Misuse

Verification of identity

Report validation pipeline

11. Future Enhancements

Drone-based image assessment

Automated relief supply chain AI planner

Multi-language chatbot

Full mobile app

Predictive climate modeling

12. Contributors
Role	Name
Team Lead	Mayank Aryan
Developer	Ayush Kashyap
Developer	Venkata Koushik
Developer	Aditya Suman
