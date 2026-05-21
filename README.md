# Azure Compliance Engine — Multimodal RAG Video Compliance Auditor

## Overview

Azure Compliance Engine is a multimodal RAG-based video compliance auditing system that analyzes video content against compliance policy documents and generates structured PASS, WARNING, or FAIL reports with evidence, timestamps, matched policy rules, severity levels, and recommendations.

The system uses Azure Video Indexer for transcript, OCR, keyword, timestamp, and metadata extraction; Azure AI Search for vector-based policy retrieval; Azure OpenAI for embeddings and reasoning; and LangGraph for orchestrating the compliance audit workflow.

## Problem Statement

Manual video compliance review is slow, inconsistent, and difficult to scale. Reviewers need to watch long videos, compare content against policy documents, identify violations, and prepare evidence-backed reports.

This project automates the compliance review workflow by extracting multimodal signals from videos, retrieving relevant policy rules, and generating explainable compliance decisions.

## Key Features

- Video URL or MP4 input support
- Temporary Azure Blob Storage upload workflow
- Transcript, OCR, keyword, timestamp, and metadata extraction
- Policy document retrieval using Azure AI Search
- RAG-based compliance reasoning using Azure OpenAI
- LangGraph-based workflow orchestration
- PASS, WARNING, and FAIL compliance classification
- Evidence-backed report generation
- Matched policy rules with severity levels
- Recommendations for remediation
- Observability support using LangSmith and Azure Application Insights

## Tech Stack

- Python
- FastAPI
- LangGraph
- Azure OpenAI
- Azure AI Search
- Azure Blob Storage
- Azure Video Indexer
- Azure Application Insights
- LangSmith
- RAG
- Vector Search

## System Architecture

```text
Video URL / MP4 Upload
        |
        v
FastAPI Backend
        |
        v
Azure Blob Temporary Storage
        |
        v
Azure Video Indexer
        |
        |-- Transcript
        |-- OCR
        |-- Keywords
        |-- Timestamps
        |-- Metadata
        |
        v
LangGraph Compliance Workflow
        |
        |-- Extract Video Evidence
        |-- Retrieve Relevant Policy Rules
        |-- Compare Evidence with Policies
        |-- Assign Severity
        |-- Generate Recommendations
        |
        v
Azure AI Search Vector Index
        |
        v
Azure OpenAI Reasoning
        |
        v
PASS / WARNING / FAIL Compliance Report