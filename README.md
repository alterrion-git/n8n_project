# n8n Youtube transcript analyzer
- Description of n8n workflow (not being hosted anymore)
- Analysis of Youtube transcripts against scientific papers (limited scope/size for demo purposes)
- Used to analyze science-based lifting advice against the most relevant literature

**Flow:**

<img width="1062" height="601" alt="Snímek obrazovky 2025-10-28 144952" src="https://github.com/user-attachments/assets/f8ad4b73-d845-405b-8250-9c53a8e77179" />

1. Use a local webhook form with URL to trigger workflow
2. Get the transcript using Apify scraper
3. Extract keywords and search for scientific papers (Apify scraper), then get PDF (http request) and save to a vector database (Pinecone)
4. Analyze transcript against paper using AI agent with RAG
5. Combine results and save to a Google Sheets file

**Result:**

<img width="810" height="277" alt="image" src="https://github.com/user-attachments/assets/a642990f-b556-45b8-9a53-4db8ca811c35" />
