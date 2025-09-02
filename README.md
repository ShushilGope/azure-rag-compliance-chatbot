# 🏦 Azure RAG Compliance Chatbot

> A Retrieval-Augmented Generation (RAG) chatbot built with Azure AI Search and Azure OpenAI to provide verifiable, source-cited answers from private regulatory documents.

### 🎬 Live Demo

![Live Chatbot Demo](demo.gif)

---

## 🎯 Problem Solved

Compliance officers in the BFSI sector face a significant challenge: manually searching thousands of pages of dense regulatory circulars. This manual process is slow, inefficient, and carries the risk of non-compliance due to human error.

This chatbot solves that problem by providing an intelligent, conversational interface to this private knowledge base. It uses the RAG pattern to ensure that all answers are grounded in the provided documents, delivering trustworthy and cited responses while preventing the AI from hallucinating.

---

## ✨ Key Features

- ✅ **Natural Language Queries:** Ask complex questions in plain English instead of using keywords.
- ✅ **Source-Grounded Answers:** The AI generates answers based *only* on the content of the uploaded regulatory documents.
- ✅ **Verifiable Citations:** Every answer includes references to the source document chunks, allowing for easy verification.
- ✅ **Secure & Private:** All data is processed within a private Azure environment, ensuring data confidentiality.
- ✅ **Hybrid Search:** Combines keyword search, vector search, and a semantic ranker for the highest possible accuracy.
- ✅ **Serverless Architecture:** Built entirely on managed Azure services for scalability and low maintenance.

---

## 🛠️ Tech Stack & Architecture

This project uses a modern, serverless architecture built entirely on Microsoft Azure.

![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

<br/>

The application follows a classic Retrieval-Augmented Generation (RAG) architecture:
