# VisionQA

## 🎯 Introduction
The VisionQA Application leverages LLM models to automate BDD test case generation and execution. It also provides project summaries and context-aware chat support to simplify the process of writing and executing BDD tests.

---

## 🎥 Demo 
📹 **Video Demo:** https://drive.google.com/file/d/1aYgrzA8HfzB8GE7Ex6YE-cmqOHhkR4eL/view?usp=sharing 

<br/>

 **AI Agent Demo:** https://drive.google.com/file/d/1w-KR0klxA5wT5HJPcOfuat1NQxZbnW1Q/view?usp=sharing 

### Ai Agent
#### <i>Our AI agent combines techniques from Adaptive RAG, Corrective RAG, and Self-RAG to enhance retrieval accuracy and reliability. It dynamically routes queries, falls back to web search when needed, and self-corrects responses to reduce hallucinations and improve answer quality.The agent also stores history in state using checkpointer memory for context retention.</i>

---

## ⚙️ What It Does
- **User Onboarding:** Upload Confluence and JIRA URLs to extract data.
- **Project Summary:** Generates a comprehensive summary from contextual data.
- **Context-Aware Chat:** Provides project-related answers and insights.
- **BDD Test Case Generation:** Creates test cases based on contextual data.
- **Syntax Validation:** Validates BDD syntax with advanced LLM models.
- **Step Definition Generation:** Generates precise and executable step definitions.
- **Test Execution:** Runs tests and generates reports using Allure.
- **Reporting:** Provides a shareable URL for the generated reports.

---

## 🏃 How to Run

### Run the Backend
```bash
cd code/src/backend
pip install -r requirements.txt
uvicorn main:app --reload
```

### Run the Frontend
```bash
cd code/src/frontend/visionqa
npm install
npm start
```

### Start the LLM Model
```bash
cd code/src/model/
pip install -r requirements.txt
cd agent/
langgraph dev
```

---

## 🏗️ Tech Stack
- **Frontend:** React, Tailwind CSS
- **Backend:** FastAPI
- **Database:** Pinecone Vector DB
- **LLM:** Langchain, LLaMA, deepseek-r1-distill-llama-70b, deepseek-r1-distill-qwen-32b, Chat Groq API
- **Sentence Transformer:** sentence-transformers/all-mpnet-base-v2
- **Image Processing:** Salesforce BLIP, OCR
- **Testing and Reporting:** Behave, Allure
