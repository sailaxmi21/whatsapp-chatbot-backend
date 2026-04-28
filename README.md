🚀 WhatsApp Chatbot Backend

A scalable Spring Boot backend that simulates a WhatsApp-style chatbot system with REST APIs, message handling, and structured conversation storage.

🎯 Key Highlights

Built a REST-based chatbot system using Spring Boot
Handles user messages and generates intelligent rule-based responses
Stores complete conversation history with timestamps
Designed with a clean layered architecture (Controller → Service → Repository)
Ready for extension into real-time chat systems or AI-powered bots

⚙️ Features

💬 Chat Functionality
Accepts user messages via /webhook
Generates responses for:
Greetings (hi, hello, good morning, etc.)
Queries (how are you, name, time, date, weather)
Gratitude (thanks, thank you)
General fallback responses

🧠 Response System

Rule-based intent detection
Structured JSON response format
🗄️ Data Persistence

Stores:
User messages
Bot replies
Timestamp of each interaction
Enables conversation tracking

📡 API Response Format
{
  "user": "sai",
  "message": "hi",
  "reply": "Hi there! How can I help you?",
  "timestamp": "2026-04-07T15:37:14"
}
🏗️ Tech Stack
Java
Spring Boot
Spring MVC
Spring Data JPA
REST APIs
MYSQL
📐 System Design

Client → REST API (/webhook)
       → Controller Layer
       → Service Layer (Chat Logic)
       → Repository Layer
       → Database (Message Storage)
       → Response JSON
       
🔥 What Makes This Project Stand Out

Clean backend architecture following industry standards
Conversation history tracking (not just stateless responses)
Extensible design for AI/ML or WhatsApp Cloud API integration
Ready for scaling into real-time chatbot systems
🚀 Future Improvements

Integrate WhatsApp Cloud API (Meta)
Add AI-based responses using LLMs
Implement WebSocket for real-time messaging
Add authentication & user sessions
Dockerize for deployment

👨‍💻 Author
Built by SaiLakshmi

Java Backend Developer | Spring Boot | REST APIs
