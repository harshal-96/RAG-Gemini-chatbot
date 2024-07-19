# Gemini RAG App Project

## Overview

The Gemini RAG App is a web application that enables users to interact with PDF documents through a question-answering interface powered by Google's Generative AI (Gemini). Users can upload multiple PDF files, and the app processes these files to allow natural language queries about their contents.

## Features

- **PDF Text Extraction**: Extracts text from uploaded PDF documents.
- **Text Chunking**: Splits extracted text into manageable chunks for processing.
- **Vector Store Creation**: Generates embeddings from text chunks and stores them in a FAISS index.
- **Question Answering**: Utilizes Google's Generative AI to answer user queries based on the content of the PDFs.
- **Streamlit Interface**: Provides a user-friendly interface for uploading PDFs and asking questions.

## Setup and Installation

1. **Clone the Repository**:
    ```sh
    git clone <repository-url>
    cd <repository-directory>
    ```

2. **Install Dependencies**:
    ```sh
    pip install -r requirements.txt
    ```

3. **Configure API Key**:
    - Create a `.env` file in the project directory.
    - Add your Google API key to the `.env` file:
      ```env
      GOOGLE_API_KEY=your_google_api_key
      ```

## How to Use

1. **Start the Application**:
    ```sh
    streamlit run app.py
    ```

2. **Upload PDF Files**:
    - Use the sidebar to upload one or more PDF files.
    - Click on "Submit & Process" to process the uploaded files.

3. **Ask Questions**:
    - Enter a question in the text input field at the top of the main page.
    - The app will display the answer based on the contents of the uploaded PDFs.

## Project Structure

- `app.py`: Main application script.
- `requirements.txt`: Lists all the dependencies required for the project.
- `.env`: Environment file containing the Google API key (not included in the repository).

## Dependencies

- `streamlit`: For creating the web interface.
- `PyPDF2`: For extracting text from PDF files.
- `langchain` and `langchain-google-genai`: For managing text processing and interaction with Google's Generative AI.
- `faiss-cpu`: For creating and managing the vector store.
- `python-dotenv`: For loading environment variables from the `.env` file.

## Acknowledgements

This project uses the following technologies and libraries:
- Streamlit
- PyPDF2
- Langchain
- FAISS
- Google's Generative AI

## Contact

For any inquiries or support, please contact Harshal Dhandrut at harshal.dhandrut@gmail.com.
