# AI-Powered Lead Generation System using n8n

An end-to-end automation workflow built with n8n that collects, enriches, and stores high-quality business leads using AI-powered query optimization, business data APIs, and automated website crawling.  
The final output is stored in Google Sheets for immediate use.

---

## Features

- AI-powered search query optimization  
- Automated business lead discovery  
- Website crawling for contact information  
- Email and social media link extraction  
- Duplicate lead removal  
- Clean, column-wise Google Sheets storage  
- Append-only storage for high reliability  
- Fully automated end-to-end workflow  

---

## Workflow Overview

1. User submits a business-related query using an n8n Form Trigger  
2. The query is optimized using an AI language model (Groq LLM)  
3. Business listings are fetched via a local business data API  
4. Business data is cleaned and normalized using custom JavaScript  
5. Each business website is crawled automatically  
6. Contact details (email and social links) are extracted  
7. Duplicate leads are removed  
8. Final leads are appended to Google Sheets  

---

## Tech Stack

- n8n – Workflow automation platform  
- Groq LLM (GPT-OSS-120B) – AI-based query optimization  
- RapidAPI (Local Business Data API) – Business listings  
- JavaScript – Data cleaning and extraction  
- Google Sheets API – Lead storage  
- HTTP Requests – Website crawling  

---

## Output Format (Google Sheets)

Each generated lead contains the following fields:

- name  
- phone  
- website  
- email  
- address  
- facebook  
- twitter  
- instagram  
- youtube  
- linkedin  
- blogspot  

Data is stored using Append Row mode to prevent workflow failures when some fields are missing.

---

## Repository Contents

- `lead generation.json` – n8n workflow export  
- Documentation files  
- README.md  

---

## How to Use

1. Import the workflow JSON into n8n  
2. Configure credentials:
   - Groq API  
   - RapidAPI  
   - Google Sheets OAuth  
3. Create a Google Sheet and add headers in Row 1  
4. Activate the workflow  
5. Submit a query using the form trigger  
6. Leads will be generated automatically in Google Sheets  

---

## Demo

A complete project walkthrough video can be added here.

---

## Author

Anjan Manohar  
Individual Project

---

## Notes

- Append-only storage is intentionally used to ensure reliability  
- Suitable for sales research, marketing analysis, and automation learning  

---

## License

This project is intended for educational and learning purposes.
