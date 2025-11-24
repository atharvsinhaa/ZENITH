<h1 align="center">🌿 ZENITH — AI Powered Mental Health & Wellbeing Platform</h1>

<p align="center">
  <img src="https://media.giphy.com/media/3o7aD2saalBwwftBIY/giphy.gif" width="200" />
</p>

<p align="center">
  <strong>ZENITH is an India-first AI mental wellness ecosystem designed to help users reach their emotional, psychological, and personal peak — their “zenith”.</strong>
</p>

---

# 🌱 **What is ZENITH?**
ZENITH is a technology-driven mental-health & wellbeing platform designed to solve the growing challenges around emotional wellness in India. It blends:

- AI  
- Community  
- Education  
- Therapy  
- Behavioural science  

ZENITH aims to bridge the **awareness gap**, reduce **stigma**, and make mental wellbeing **affordable**, **private**, and **accessible**.

---

# 🌟 **Why ZENITH?**
India has the world’s largest youth population — yet millions face:

- Limited access to mental-health professionals  
- High stigma around seeking help  
- Rising anxiety & depression  
- Expensive therapy  
- Lack of counsellors outside urban cities  

❗ **ZENITH solves this using AI + community support + verified educational content + accessible therapy options.**

<p align="center">
  <img src="https://media.giphy.com/media/xUA7bdpLxQhsSQdyog/giphy.gif" width="350" />
</p>

---

# 🧩 **Core Modules of ZENITH**

## 🧠 1. AI Early Detection System
Uses AI + behavioural indicators to identify early emotional risk patterns.

### Analyzes:
- Mood fluctuations  
- Emotion cues  
- Journal-based reflections  
- Stress triggers  
- Lifestyle indicators  
- Tone & sentiment through NLP  

⚠️ *Not diagnostic — assists by raising awareness and providing guidance.*

---

## 💬 2. AI Mental Health Companion

A 24×7 conversational wellness partner.

### Capabilities:
- Emotional check-ins  
- CBT-inspired reframing  
- Mindfulness + grounding  
- Guided reflections  
- Habit-building suggestions  
- Conversation support during distress  

<p align="center">
  <img src="https://media.giphy.com/media/l3q2XhfQ8oCkm1Ts4/giphy.gif" width="250"/>
</p>

---

## 📚 3. Awareness & Education Hub

A learning center designed for mental-health literacy across India.

### Includes:
- Scientific articles  
- Regional language versions  
- Mental health myths vs facts  
- Bite-sized learning videos  
- Stress-management guides for students & professionals  
- Daily wellness practices  

---

## 🧑‍🤝‍🧑 4. Community Platform

A safe, anonymous, moderated online forum.

### Users can:
- Share feelings & thoughts  
- Discuss challenges  
- Ask for guidance  
- Join support groups  
- Participate in events  
- Engage with peers  

### Safety:
- AI moderation  
- Human review  
- Toxicity filters  
- Anonymous posting enabled  

---

## 👩‍⚕️ 5. Therapy Access Marketplace

A marketplace to connect users with verified mental-health professionals.

### Features:
- Book certified therapists  
- Choose by:
  - Language  
  - Price  
  - Specialization  
  - Experience  
- Online/offline sessions  
- Secure chat/video  
- Student support pricing  

---

# 🏛️ **System Architecture (Detailed + Visual)**

Below are all four architectural diagrams included in your design:

---

# 🔷 **1. UML Diagram**

```mermaid
classDiagram
    class User {
      +id: String
      +name: String
      +email: String
      +role: String
      +login()
    }
    class AuthService {
      +login()
      +logout()
      +verifyToken()
    }
    class ChatSession {
      +sessionId
      +startTime
      +endTime
      +messages[]
    }
    class AIEngine {
      +analyzeMessage()
      +detectEmotion()
      +generateResponse()
    }
    class Therapist {
      +therapistId
      +specialization
      +availableSlots[]
      +bookSlot()
    }
    User --> ChatSession : creates
    ChatSession --> AIEngine : uses
    User --> Therapist : books
    AuthService --> User : authenticates
