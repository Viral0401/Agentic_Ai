Agentic AI Paper Reviewer
Overview
This repository contains an Agentic AI-driven research paper reviewing system, leveraging CrewAI to critically assess and refine research papers. The system extracts text from PDF research papers and generates structured, in-depth reviews with automated evaluation, mismatch detection, and refinement.

Key Features
PDF Parsing: Extracts text from research papers using PyMuPDF (fitz).

AI-Powered Review Generation: Creates structured critiques covering all major sections of the paper.

Automated Evaluation: Ensures review depth, specificity, and logical consistency.

Mismatch Flagging: Identifies inconsistencies in critiques and scores.

Final Review Refinement: Ensures professional tone, depth, and fair critique.

Structured Output: Provides a final review with a rating (1-10), acceptance decision (Strong Reject → Strong Accept), and confidence score (1-5).

How It Works
Extract: Parses research paper PDFs from the ICLR_2020_papers/ directory.

Generate Review: Uses an AI agent to create an initial structured review.

Evaluate: A separate AI agent assesses the review for depth, politeness, and consistency.

Flag Mismatches: Detects contradictions and ensures ratings align with critiques.

Refine Final Review: Incorporates feedback and produces a polished, expert-level review.

Save Output: Stores the final review as a text file in the ICLR_2020_LLM_reviews/ directory.

Installation & Setup
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/yourusername/agentic-ai-reviewer.git
cd agentic-ai-reviewer
2. Install Dependencies
Ensure Python 3.8+ is installed, then run:

bash
Copy
Edit
pip install crewai pymupdf openai
3. Prepare Input PDFs
Place research papers in the ICLR_2020_papers/ directory.

4. Run the Review System
bash
Copy
Edit
python review_pipeline.py
Output Format
Each paper receives a structured review saved as:
📄 ICLR_2020_LLM_reviews/paper_title_review.txt

Example Review Format:
yaml
Copy
Edit
Paper Title: Example Research Paper  
Field: AI & Machine Learning  

Review:  
[Critically analyzes all major sections, highlights strengths, weaknesses, and areas for improvement.]  

Rating: 7/10  
Decision: Strong Accept  
Confidence Score: 4/5  
Contributing
We welcome contributions! Feel free to submit PRs or open issues.

License
This project is licensed under the MIT License.

