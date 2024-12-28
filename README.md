# RAG_ Document _Q&A_ With_ Groq _&_ Open_ AI_ Embeddings
 This project implements a Retrieval-Augmented Generation (RAG) system using Groq's Llama3-8b model and OpenAI embeddings. The application provides a user-friendly interface powered by Streamlit to perform question-answering on a vectorized database of research papers. This tool leverages the capabilities of LangChain for document processing, embedding generation, and retrieval chains, alongside LangSmith tracing for monitoring and debugging.

# Features

## Core Functionality:

**1.** **Document Embedding:**

**-** Uses OpenAI's text-embedding-ada-002 model for generating vector embeddings.

**-** Processes PDF files located in the research_papers directory.

**-** Splits documents into manageable chunks using RecursiveCharacterTextSplitter for better retrieval performance.

**-** Stores embeddings in a FAISS vector database for efficient similarity search.

**2.** **Question-Answering System:**

**-** Employs Groq's Llama3-8b-8192 model for generating context-aware answers.

**-** Integrates LangChain's retrieval chain to fetch relevant documents and provide responses based on user queries.

**3.** **Streamlit-Based Interface:**

**-** Provides an intuitive web-based UI for:

**-** Generating embeddings.

**-** Submitting queries.

**-** Includes an expandable section to view retrieved document content and similarity context.

**4.** **LangSmith Tracing:**

**-** Tracing is enabled for better monitoring and debugging of the chain processes.

# Usage

**1.** Run the Streamlit application:

**-** streamlit run main.py

**2.** Open your web browser to the URL displayed in the terminal (typically http://localhost:8501).

**3.** Perform the following actions:

**-** **Document Embedding:** Click the "Document Embedding" button to generate the vector database from the PDFs in the research_papers folder.

**-** **Ask Questions:** Enter your query in the text input field to receive responses based on the embedded documents.

# Key Libraries and Tools Used

**1.** **Streamlit:** For creating the web-based interface.

**2.** **LangChain:** For building document chains, retrieval chains, and embeddings.

**3.** **Groq:** For utilizing the Llama3-8b model in generating responses.

**4.** **FAISS:** For efficient vector-based similarity searches.

**5.** **dotenv:** For managing sensitive environment variables.

**6.** **LangSmith Tracing:** To monitor the performance and flow of LangChain processes.

# Security Considerations

**-** The .env file containing sensitive API keys is excluded from this repository for security purposes. 
