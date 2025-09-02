🏦 Azure RAG Compliance Chatbot
A Retrieval-Augmented Generation (RAG) chatbot built with Azure AI Search and Azure OpenAI to provide verifiable, source-cited answers from private regulatory documents.

🎬 Live Demo

![Live Chatbot Demo](docs/ChatBot%20Demo.gif)


🎯 Problem Solved
Compliance officers in the BFSI sector face a significant challenge: manually searching thousands of pages of dense regulatory circulars. This manual process is slow, inefficient, and carries the risk of non-compliance due to human error.

This chatbot solves that problem by providing an intelligent, conversational interface to this private knowledge base. It uses the RAG pattern to ensure that all answers are grounded in the provided documents, delivering trustworthy and cited responses while preventing the AI from hallucinating.

✨ Key Features
✅ Natural Language Queries: Ask complex questions in plain English instead of using keywords.

✅ Source-Grounded Answers: The AI generates answers based only on the content of the uploaded regulatory documents.

✅ Verifiable Citations: Every answer includes references to the source document chunks, allowing for easy verification.

✅ Secure & Private: All data is processed within a private Azure environment, ensuring data confidentiality.

✅ Hybrid Search: Combines keyword search, vector search, and a semantic ranker for the highest possible accuracy.

✅ Serverless Architecture: Built entirely on managed Azure services for scalability and low maintenance.

🛠️ Tech Stack & Architecture
This project uses a modern, serverless architecture built entirely on Microsoft Azure.

```mermaid
flowchart LR
    U[User] --> W[Web Chat App\n(Flask / React)]
    W --> S[Azure Cognitive Search\n(Vector + Semantic Index)]
    S --> O[Azure OpenAI\n(Embeddings + LLM)]
    O --> W
    W -->|Answer with citations| U

    %% Data ingestion flow
    B[Azure Blob Storage\n(Regulatory PDFs)] --> D[Azure Document Intelligence\n(OCR + Parsing)]
    D --> S
    S -.->|Indexing reference| B
```



🚀 Future Improvements
➡ Display Citations: Modify the UI to show the specific source chunks retrieved for each answer.

➡ Add Chat History: Implement logic to send the conversation history with each new request, giving the chatbot memory.

➡ Deploy to Azure: Host the index.html file on Azure App Service or Azure Static Web Apps to make it publicly accessible.

➡ Streaming Responses: Update the JavaScript to handle streaming responses from the OpenAI API for a more responsive user experience.
