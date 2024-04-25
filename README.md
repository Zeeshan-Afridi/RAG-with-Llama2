# RAG-with-Llama2

## This app is a RAG based Q&A system on PDF Documents 

This notebook demonstrates the use of the Llama Index library to create a Q&A system for a PDF document. The notebook utilizes the following libraries:

- `llama_index`: A library for building and querying large-scale text indexes using OpenAI's LLMs.
- `SimpleDirectoryReader`: A class for reading documents from a directory.
- `HuggingFaceLLM`: A class for using Hugging Face LLMs with Llama Index.
- `LangchainEmbedding`: A class for using LangChain embeddings with Llama Index.
- `ServiceContext`: A class for configuring the execution context for Llama Index.
- `VectorStoreIndex`: A class for creating a vector-based index from documents.
- `query_engine`: A class for querying the index and retrieving answers.

## Usage

1. **Import Libraries**: The notebook begins by importing the necessary libraries.
2. **Install Dependencies**: The notebook then installs the required dependencies using `!pip` commands.
3. **Load Documents**: The `SimpleDirectoryReader` class is used to load the PDF document into a list of documents.
4. **Configure Prompts**: The notebook defines the system prompt and query wrapper prompt for the Q&A system.
5. **Authenticate with Hugging Face**: The notebook uses the `huggingface-cli` to authenticate with Hugging Face.
6. **Initialize LLM and Embedding Model**: The notebook initializes the HuggingFaceLLM and LangchainEmbedding objects.
7. **Create Service Context**: The notebook creates a ServiceContext object to configure the execution context for Llama Index.
8. **Build Index**: The notebook uses the `VectorStoreIndex` class to build an index from the documents and the configured service context.
9. **Create Query Engine**: The notebook creates a `query_engine` object for querying the index.
10. **Query Index**: The notebook demonstrates querying the index with a sample question.
11. **Print Response**: The notebook prints the answer retrieved from the index.
