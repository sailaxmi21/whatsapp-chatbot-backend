# whatsapp-chatbot-backend
# WhatsApp Chatbot Backend

A **Spring Boot** backend for a WhatsApp-style chatbot.  
Supports multiple greetings, questions, and simple chatbot responses. Stores timestamped messages and replies.

---

## Features

- Accepts user messages via a **REST API** (`/webhook`)  
- Responds with predefined replies based on message content:
  - Greetings: `hi`, `hello`, `good morning`, `good night`
  - Questions: `how are you`, `what is your name`, `time`, `date`, `weather`
  - Gratitude: `thanks`, `thank you`
  - Others: `help`, `joke`, etc.
- Returns a structured **JSON response**:
  ```json
  {
      "user": "sai",
      "message": "hi",
      "reply": "Hi there! How can I help you?",
      "timestamp": "2026-04-07T15:37:14.5894484"
  }
