# ragas-rag-evaluator
ragas for evaluating rag and llm efficiency

# RAG System with Ollama
This is a simple Retrieval-Augmented Generation (RAG) system that uses a local Ollama model to answer questions based on a provided PDF document.

# Prerequisites
Python: Install Python 3.10 or newer.

VS Code: Install Visual Studio Code with the Python and Jupyter extensions.

Ollama: Download and install the Ollama application from ollama.com.

# Setup Instructions
Add Ollama to your System Path:

Find the Ollama executable (e.g., C:\Program Files\Ollama).

Add this path to your system's PATH environment variables.

Restart your terminal after making this change.

# Download the Language Model:

Open your terminal and run the following command to download the llama2 model.

ollama pull llama2
Create a Virtual Environment:

In your project directory, create a virtual environment.

python -m venv venv
Activate the environment.

On Windows: .\venv\Scripts\activate

# Install Required Libraries:

With your virtual environment active, install the necessary packages.

pip install langchain-community pypdf chromadb
Place your PDF:

Place the PDF document you want to use in your project folder and name it your_document.pdf.

# Running the Project
Open the ragas.ipynb Jupyter Notebook in VS Code and run each cell in order.

Cell 1: Loads and chunks your PDF.

Cell 2: Creates the embeddings using Ollama and builds the ChromaDB vector store.

Cell 3: Initializes the RAG chain with the Ollama model.

Cell 4: Runs the query and prints the grounded response.

# You can modify the query variable in the last cell to ask a new question. 