# 🚀 WhatsApp Chatbot Backend System

A scalable Spring Boot backend system that simulates a WhatsApp-style chatbot. It processes user messages, generates rule-based responses, and stores complete conversation history using a structured REST API architecture.

---

## 🎯 Project Overview

This project demonstrates backend system design using Spring Boot by building a chatbot service that handles incoming messages, processes intents, and returns structured responses. It focuses on REST API design, layered architecture, and database-driven conversation management.

---

## ⚙️ Key Features

### 💬 Chat Functionality

* Accepts user messages via `/webhook` API
* Generates rule-based responses for:

  * Greetings (hi, hello, good morning)
  * Basic queries (name, time, date, how are you)
  * Gratitude responses (thanks, thank you)
  * Fallback responses for unknown inputs

---

### 🧠 Chat Logic

* Simple rule-based intent detection
* Structured response generation
* Extensible design for AI/ML integration

---

### 🗄️ Data Persistence

* Stores complete conversation history
* Saves:

  * User message
  * Bot response
  * Timestamp
* Enables chat history retrieval and tracking

---

## 📡 API Example

### Request

```json id="api_req_01"
POST /webhook
{
  "user": "sai",
  "message": "hi"
}
```

### Response

```json id="api_res_01"
{
  "user": "sai",
  "message": "hi",
  "reply": "Hi there! How can I help you?",
  "timestamp": "2026-04-07T15:37:14"
}
```

---

## 🏗️ System Architecture

Client → REST API (/webhook) → Controller → Service (Chat Logic) → Repository → MySQL Database → JSON Response

---

## 🛠️ Tech Stack

* Java
* Spring Boot
* Spring MVC
* Spring Data JPA
* REST APIs
* MySQL
* Maven

---

## 📌 Architecture Style

* Layered architecture:

  * Controller → Request handling
  * Service → Business logic
  * Repository → Database operations
* Clean separation of concerns
* Scalable backend design

---

## 🚀 Why This Project Stands Out

* Real-world chatbot backend simulation
* Persistent conversation storage (not stateless APIs)
* Clean scalable Spring Boot architecture
* Easy to extend into:

  * AI chatbot (LLM integration)
  * WhatsApp Cloud API integration
  * Real-time messaging system

---

## 🔮 Future Improvements

* Integrate WhatsApp Cloud API (Meta)
* Add JWT authentication
* Implement WebSocket for real-time chat
* Add AI/LLM-based responses
* Dockerize for deployment

---

## 👨‍💻 Author

Sai Lakshmi
Java Backend Developer | Spring Boot | REST APIs
