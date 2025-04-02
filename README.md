# Agentic AI Paper Reviewer  

## Overview  
This repository contains an **Agentic AI-driven** research paper reviewing system, leveraging **CrewAI** to critically assess and refine research papers. The system extracts text from PDF research papers and generates structured, in-depth reviews with **automated evaluation, mismatch detection, and refinement**.  

## Key Features  
- 📄 **PDF Parsing**: Extracts text from research papers using `PyMuPDF (fitz)`.  
- 📝 **AI-Powered Review Generation**: Creates structured critiques covering all major sections of the paper.  
- 🧐 **Automated Evaluation**: Ensures review depth, specificity, and logical consistency.  
- ⚠️ **Mismatch Flagging**: Identifies inconsistencies in critiques and scores.  
- 🔍 **Final Review Refinement**: Ensures professional tone, depth, and fair critique.  
- 📌 **Structured Output**: Provides a final review with a **rating (1-10), acceptance decision (Strong Reject → Strong Accept), and confidence score (1-5)**.  

## How It Works  
1. **Extract**: Parses research paper PDFs from the `ICLR_2020_papers/` directory.  
2. **Generate Review**: Uses an AI agent to create an **initial structured review**.  
3. **Evaluate**: A separate AI agent **assesses the review** for depth, politeness, and consistency.  
4. **Flag Mismatches**: Detects contradictions and **ensures ratings align with critiques**.  
5. **Refine Final Review**: Incorporates feedback and produces a **polished, expert-level review**.  
6. **Save Output**: Stores the **final review** as a text file in the `ICLR_2020_LLM_reviews/` directory.  

## Installation & Setup  
### 1️⃣ Clone the Repository  
```bash
git clone https://github.com/yourusername/agentic-ai-reviewer.git
cd agentic-ai-reviewer
