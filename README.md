<h1 align="center">🌿 ZENITH — AI Powered Mental Health & Wellbeing Platform</h1>

<p align="center">
  <img src="https://media.giphy.com/media/qgQUggAC3Pfv687qPC/giphy.gif" width="200" />
</p>

<p align="center">
  <strong>ZENITH is an India-first AI mental wellness ecosystem designed to help users reach their emotional, psychological, and personal peak — their “zenith”.</strong>
</p>

---

# 🌱 What is ZENITH?
ZENITH is a technology-driven mental-health & wellbeing platform designed to solve the growing challenges around emotional wellness in India. It blends:

- AI  
- Community  
- Education  
- Therapy  
- Behavioural science  

ZENITH aims to bridge the awareness gap, reduce stigma, and make mental wellbeing affordable, private, and accessible.

---

# 🌟 Why ZENITH?
India has the world’s largest youth population — yet millions face:

- Limited access to mental-health professionals  
- High stigma  
- Rising anxiety & depression  
- Expensive therapy  
- Lack of counsellors outside urban cities  

**ZENITH solves this using AI + community support + verified education + accessible therapy options.**

<p align="center">
  <img src="https://media.giphy.com/media/xUA7bdpLxQhsSQdyog/giphy.gif" width="350" />
</p>

---

# 🧩 Core Modules of ZENITH

## 🧠 1. AI Early Detection System
Uses AI + behavioural indicators to identify early emotional-risk patterns.

### Analyzes:
- Mood fluctuations  
- Emotion cues  
- Journal reflections  
- Stress triggers  
- Lifestyle indicators  
- Tone & sentiment  

⚠️ *Not diagnostic — assists with awareness.*

---

## 💬 2. AI Mental Health Companion
A 24×7 conversational wellbeing partner.

### Capabilities:
- Emotional check-ins  
- CBT-inspired reframing  
- Mindfulness exercises  
- Guided reflections  
- Journaling support  

<p align="center">
  <img src="https://media.giphy.com/media/l3q2XhfQ8oCkm1Ts4/giphy.gif" width="250"/>
</p>

---

## 📚 3. Awareness & Education Hub
A scalable mental-health literacy center.

### Includes:
- Science-backed articles  
- Regional language content  
- Wellness videos  
- Stress-management guides  

---

## 🧑‍🤝‍🧑 4. Community Platform
A safe, anonymous, moderated social space.

### Users can:
- Share thoughts  
- Ask questions  
- Join support groups  
- Participate in events  

Safety:
- AI moderation  
- Human review  
- Anonymized posting  

---

## 👩‍⚕️ 5. Therapy Access Marketplace
Connects users with verified professionals.

### Features:
- Book certified therapists  
- Multilingual support  
- Specialization & price filters  
- Secure online/offline sessions  

---

# 🏛️ System Architecture (All Diagrams Included)

---

# 🔷 1. UML Diagram

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
