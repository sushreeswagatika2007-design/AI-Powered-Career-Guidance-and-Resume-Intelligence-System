Run Command: python career_guidance_system.py (Optional: export GEMINI_API_KEY="your_key")
​Dataset: data/job_roles_dataset.csv (10 AI/Tech roles) + data/sample_candidate_resume.pdf.
​Workflow:
​1. Parse PDF/TXT resume (PyMuPDF), mask PII (emails/phones), and segment sections.
​2. Extract 80+ domain skills & keywords (NLTK lemmatization + regex).
​3. Rank top career roles via TF-IDF + Cosine Similarity (65% semantic + 35% skill overlap).
​4. Compare resume against any Job Description to find matched & missing skills.
​5. Run Gemini AI Mentor & Multi-Turn CLI Chatbot (truthful project rewrites + 4-week roadmap).
​Key Results:
​Top-1 Recommendation Accuracy: 100.0% (8/8)
​Top-3 Recommendation Accuracy: 100.0% (8/8)
​Mean Reciprocal Rank (MRR): 1.0000
