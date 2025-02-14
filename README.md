# Chat with Multiple PDFs - Streamlit App

## Overview
This is a Streamlit-based web application that allows users to upload multiple PDFs and ask questions based on the document content using AI-powered embeddings and retrieval.

<img width="1303" alt="image" src="https://github.com/user-attachments/assets/8edc96b6-ac1b-4d48-89f5-8fddf83207d4" />

## Features
- Upload multiple PDF files
- Extract text from PDFs
- Convert text into embeddings using Google's Gemini API
- Store embeddings in a FAISS vector database
- Retrieve relevant information and answer user queries

## Requirements
Ensure you have the following installed:

- Python 3.8+
- Streamlit
- PyPDF2
- LangChain
- FAISS
- Google Generative AI API
- dotenv

## Installation
1. Clone the repository:
   ```bash
   git clone <repo-url>
   cd <project-folder>
   ```
2. Create a virtual environment and activate it:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Create a `.env` file and add your Google API key:
   ```
   GOOGLE_API_KEY=your_api_key_here
   ```

## Usage
1. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```
2. Upload PDFs through the sidebar.
3. Enter your question in the text box.
4. View AI-generated responses based on your documents.

## Troubleshooting
- Ensure the `.env` file is properly configured.
- Check for typos in function names.
- Verify that required dependencies are installed.
- Run `print(os.getenv("GOOGLE_API_KEY"))` to confirm the API key is loading.

