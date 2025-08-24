
# Artful Curator Bot Prototype

This is a prototype chatbot built in **Dialogflow ES** to demonstrate feasibility for the **ProductOps assignment**.  
It focuses on improving user experience for museum/gallery visitors by answering questions about upcoming exhibits, hours, and locations.

---

## 📌 Features
- **5 Intents**
  1. `Find_Upcoming_Exhibit` → answers “What’s new?” or “Upcoming exhibitions?”
  2. `Exhibit_Hours` → provides exhibit-specific hours (with **slot filling** if no exhibit is given).
  3. `Exhibit_Location` → tells which hall an exhibit is located in.
  4. `Default Fallback (Clarify)` → handles unrecognized input with clarifying questions.
  5. `Escalate_To_Staff` → offers escalation to a human if needed.

- **1 Entity**
  - `@exhibit_name` → supports exhibit names and synonyms (`Abstract Visions`, `Celestial Forms`, `Modern Landscapes`).

- **Slot Filling**
  - If a user asks for hours without specifying the exhibit, the bot prompts:  
    *“Which exhibit are you asking about?”*

- **Fallback Handling**
  - Tiered strategy: clarify first, then escalate to staff.

---

## 🛠 Setup Instructions
1. Download this repository or clone it:
   ```bash
   git clone https://github.com/<your-username>/artful-curator-bot-prototype.git
