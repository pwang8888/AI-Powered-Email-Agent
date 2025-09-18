# 📧 AI-Powered Email Agent

An intelligent automation system that **retrieves recipient information, generates personalized drafts with OpenAI, and sends professional emails automatically**.  
This project combines **n8n workflows, Pinecone vector search, and LLMs** to streamline communication at scale.

---

## ✨ Features
- 🔍 **Smart recipient lookup** using Pinecone vector database  
- 📝 **Context-aware draft generation** with OpenAI GPT models  
- 📬 **Automated delivery** via Gmail integration  
- 🎯 **Personalization rules**: names, tone, subject lines, and clear closing phrases  
- 📊 Supports multiple email types: reminders, follow-ups, offers, support, and more  

---

## 🛠️ Tech Stack
- **n8n** – workflow automation  
- **OpenAI GPT-4o** – natural language generation  
- **Pinecone** – vector database for recipient info retrieval  
- **Gmail API** – email sending integration  

---

## ⚙️ How It Works
1. **Data Ingestion**: Contact details and documents are embedded using OpenAI and stored in Pinecone:contentReference[oaicite:3]{index=3}.  
2. **Query Handling**: On receiving a chat/email request, the system retrieves the correct recipient address from Pinecone:contentReference[oaicite:4]{index=4}.  
3. **Draft Generation**: OpenAI creates a clear, concise, and professional email tailored to the recipient and context:contentReference[oaicite:5]{index=5}.  
4. **Delivery**: The draft is automatically sent through Gmail, reducing manual effort.  

---

## 🚀 Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/pwang8888/AI-Powered-Email-Agent
   cd AI-Powered-Email-Agent
