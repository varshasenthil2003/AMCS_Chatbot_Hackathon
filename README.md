# Document-Based Chatbot with Cohere

This project is a chatbot designed to answer user queries based on uploaded PDF documents. The chatbot utilizes Cohere's NLP capabilities for semantic search and conversational AI.

## Features

- **Document Upload and Indexing**: Upload PDF documents to create a searchable index.
- **Semantic Search**: Retrieve relevant document snippets for user queries using Cohere embeddings.
- **AI-Powered Conversations**: Generate context-aware responses to user queries.
- **Interactive Web Interface**: Engage with the chatbot and upload documents directly from the browser.

## Project Structure

```
├── app.py               # Main Flask application
├── test.py              # Script to test Cohere API models 
├── requirements.txt     # Python dependencies
├── .env                 # Environment variables (API key) 
├── templates/           
│   └── index.html       # Frontend template 
├── documents/           # Folder for uploaded PDF documents
└── README.md            # Project documentation
```

## Prerequisites

1. Python 3.7 or later.
2. A Cohere API key.
3. Dependencies listed in `requirements.txt`.

## Installation

1. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Set up the `.env` file: Create a `.env` file in the project root directory with the following content:
   ```
   COHERE_API_KEY='Replace with your actual API key'  
   ```

## Usage

1. Start the Flask application:
   ```bash
   python app.py
   ```

2. Open the application in your browser:
   ```
   http://127.0.0.1:5000
   ```

3. Upload PDF documents in the "Upload Your PDF Files" section.

4. Interact with the chatbot by entering queries in the input field.

## Frontend Template

The web interface is defined in `templates/index.html`. It features:

- **Upload Section**: Allows users to upload PDF files.
- **Chatbox**: Displays user and chatbot messages in a conversational format.
- **Responsive Design**: Adjusts for desktop and mobile devices using Bootstrap.

## Dependencies

Install all required Python libraries with:
```bash
pip install -r requirements.txt
```

Key dependencies:
- Flask
- pdfplumber
- Cohere
- transformers
- torch
- python-dotenv

## Future Enhancements

- Add support for formats like DOCX and TXT.
- Implement user authentication for secure access.
- Optimize the embedding and search process for large datasets.
