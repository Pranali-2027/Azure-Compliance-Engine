# 🎥 RAG-Based Multimodal Video Compliance Auditor using LangGraph

An enterprise-grade Generative AI system that automatically audits YouTube advertisements, influencer marketing videos, and promotional content against regulatory and compliance policies using Retrieval-Augmented Generation (RAG), LangGraph orchestration, vector search, and Large Language Models.

The platform analyzes video content, retrieves relevant compliance rules from policy documents, detects potential violations, and generates structured audit reports with evidence-backed recommendations.

---

## 🚀 Business Problem

Brands and regulatory teams review thousands of advertisements, influencer campaigns, and promotional videos every day.

Manual compliance review is:

* Time-consuming
* Expensive
* Difficult to scale
* Prone to human errors

This project automates the compliance auditing process using AI, helping organizations identify misleading claims, missing disclosures, and policy violations before publishing content.

---

## 🏗️ System Architecture

![Architecture](assets/architecture.png)

### End-to-End Workflow

1. User submits a YouTube video URL.
2. FastAPI receives the audit request.
3. LangGraph orchestrates the complete workflow.
4. Video content is processed to extract:

   * Transcript
   * OCR Text
   * Metadata
   * Timestamps
5. Compliance policy documents are indexed using embeddings.
6. RAG retrieves the most relevant compliance rules.
7. GPT-4o evaluates video content against policy guidelines.
8. Violations are classified by category and severity.
9. A structured compliance report is generated.
10. LangSmith and Application Insights provide observability and monitoring.

---

## 📸 Project Demonstration

### API Request

The user submits a YouTube video URL through the FastAPI endpoint.

![API Request](assets/api-request.png)

---

### Compliance Audit Result

The system generates a structured compliance report highlighting detected violations and recommendations.

![Compliance Result](assets/compliance-result.png)

---

## 📊 Sample Audit Output

```json
{
  "status": "FAIL",
  "final_report": "The video violates multiple compliance rules.",
  "compliance_results": [
    {
      "category": "Claim Validation",
      "severity": "CRITICAL"
    },
    {
      "category": "Endorsement Disclosure",
      "severity": "CRITICAL"
    }
  ]
}
```

---

## ⚙️ Technology Stack

### Backend

* Python
* FastAPI
* Uvicorn

### Generative AI

* GPT-4o
* LangChain
* LangGraph
* Prompt Engineering

### Retrieval Layer

* RAG (Retrieval-Augmented Generation)
* Embeddings
* Vector Search
* Azure AI Search (Architecture Ready)

### Video Intelligence

* Transcript Extraction
* OCR Processing
* Metadata Analysis
* Azure Video Indexer (Architecture Ready)

### Observability

* LangSmith
* Azure Application Insights

### Cloud Services

* Azure Blob Storage (Architecture Ready)
* Azure OpenAI (Architecture Ready)

---

## 🚀 Key Features

* Automated Video Compliance Auditing
* RAG-Based Policy Retrieval
* LangGraph Workflow Orchestration
* OCR and Transcript Processing
* Vector Similarity Search
* Structured JSON Output
* Severity-Based Violation Classification
* Enterprise Monitoring & Observability
* Scalable AI System Design

---

## 🧠 Core AI Concepts Demonstrated

* Retrieval-Augmented Generation (RAG)
* Embeddings
* Vector Databases
* Semantic Search
* Prompt Engineering
* Structured Output Generation
* Hallucination Reduction
* Workflow Orchestration
* LLM Evaluation
* AI Observability

---

## 📈 Future Enhancements

* React Frontend Dashboard
* Multi-Language Compliance Auditing
* Real-Time Video Monitoring
* Human-in-the-Loop Review System
* Batch Video Processing
* Full Azure Cloud Deployment
* Compliance Analytics Dashboard

---

## 🎯 Skills Demonstrated

* Generative AI Engineering
* Enterprise AI Architecture
* FastAPI Development
* LangGraph Workflows
* Retrieval Systems
* Vector Databases
* AI System Design
* Observability & Monitoring
* API Development
* Cloud-Native AI Design

---

## 👩‍💻 Author

### Pranali Dayanand Misal

B.Tech – Electronics & Telecommunication Engineering
Vishwakarma Institute of Information Technology (VIIT), Pune

Aspiring AI Engineer | Generative AI Engineer | Machine Learning Enthusiast

GitHub: https://github.com/Pranali-2027
