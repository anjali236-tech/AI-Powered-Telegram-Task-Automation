# AI-Powered-Telegram-Task-Automation

# AI-Powered Telegram Chatbot & Task Automation

An AI-powered Telegram chatbot and task management automation system built using **Activepieces**, integrating OpenRouter, Groq, and ClickUp. The system supports text and voice interactions, provides conversational responses and information, and automates task creation through AI-driven workflows.

## 🚀 Project Overview

This project combines conversational AI with workflow automation to create an intelligent Telegram chatbot. Users can ask general questions, receive information, interact through voice messages, or create tasks using natural language.

Using LLM-based processing, API integrations, and conditional workflows, the system interprets user inputs, validates task information, and automates task creation in ClickUp.

## ✨ Key Features

- **AI-Powered Chatbot:** Handles general conversations, answers questions, and provides relevant information.
- **Text & Voice Interaction:** Supports both text messages and voice-based inputs.
- **Voice-to-Text Transcription:** Converts voice messages into text using Groq's speech-to-text API.
- **AI-Based Intent Classification:** Distinguishes between general queries and task creation requests.
- **Structured Data Extraction:** Extracts task details using LLM-based processing and JSON.
- **Task Validation:** Validates five mandatory attributes: task name, description, status, priority, and assignee.
- **Automated Task Creation:** Creates tasks directly in ClickUp through API integration.
- **Conditional Routing:** Directs requests to appropriate processing branches based on message type and intent.
- **Error Handling:** Handles invalid inputs, incomplete requests, and workflow failures through validation and fallback responses.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Activepieces | Workflow automation and orchestration |
| Telegram Bot API | Chatbot interface |
| OpenRouter | LLM integration and natural language processing |
| Groq API | Audio transcription |
| ClickUp API | Task management and creation |
| JSON | Structured data extraction and exchange |
| HTTP Requests | API communication |

## ⚙️ Workflow Architecture

The workflow is divided into multiple processing paths based on the type of user input.

### 1. Text Processing

1. Receives text messages through Telegram.
2. Uses OpenRouter to understand user intent.
3. Handles general questions and conversational interactions.
4. Extracts task details when a task creation request is identified.
5. Converts AI responses into structured JSON.
6. Validates required task attributes.
7. Uses conditional routing to create ClickUp tasks or request missing information.
8. Sends responses and task confirmations through Telegram.

### 2. Voice Processing

1. Receives voice messages through Telegram.
2. Retrieves audio files using HTTP requests.
3. Processes audio using Groq's speech-to-text API.
4. Converts speech into text.
5. Passes the transcribed content to OpenRouter for interpretation.
6. Generates and sends an appropriate response through Telegram.

### 3. Error Handling & Validation

- Validates required task fields before task creation.
- Identifies missing information and requests clarification.
- Uses conditional routing to prevent incomplete task requests from proceeding.
- Handles invalid or unsupported inputs through fallback responses.
- Incorporates error-handling mechanisms to manage workflow execution failures.

## 📸 Workflow Screenshots

### Complete Automation Workflow
<img width="3200" height="2582" alt="Telegram Automation Bot Main" src="https://github.com/user-attachments/assets/1bf73e63-89e0-45b5-89b8-98e8f1781552" />


### Text Processing Branch
![Text Processing](screenshots/text_processing.png)

### Voice Processing Branch
![Voice Processing](screenshots/voice_processing.png)

### ClickUp Task Creation
![ClickUp Task](screenshots/clickup_task_created.png)

## 🔄 Sample Interaction Scenarios

| User Input | Expected Behaviour |
|---|---|
| Hello | Generates a conversational response |
| General question | Provides relevant information |
| Voice message | Transcribes and processes speech |
| Complete task request | Validates details and creates a ClickUp task |
| Incomplete task request | Identifies missing fields and requests information |
| Invalid or unsupported input | Provides an appropriate fallback response |

## 🔧 Setup & Configuration

### Requirements
- Activepieces account or self-hosted instance
- Telegram Bot API token
- OpenRouter API key
- Groq API key
- ClickUp account and API connection

### Basic Setup
1. Create a Telegram bot using BotFather.
2. Configure API connections in Activepieces.
3. Set up OpenRouter and Groq integrations.
4. Connect your ClickUp workspace.
5. Import or recreate the workflow in Activepieces.
6. Configure routing conditions and field mappings.
7. Test the workflow with text and voice inputs.

**Security Note:** Store API keys, bot tokens, and credentials securely within Activepieces. Never commit sensitive credentials to GitHub.

## 🎯 Project Objective

To demonstrate the integration of conversational AI, speech recognition, API communication, and workflow automation in building an intelligent chatbot that combines information assistance with automated task management.

## 👩‍💻 Developed By

**Anjali Muralidharan**

B.Sc. Information Technology

[GitHub Profile](https://github.com/anjali236-tech)
