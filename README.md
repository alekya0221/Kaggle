# Insurance Document Retrieval-Augmented Generation (RAG) System

## Overview

This project implements a Retrieval-Augmented Generation (RAG) system that extracts information from insurance policy PDFs, performs semantic search, re-ranks the results using a cross encoder, and generates natural language responses with GPT-3.5-turbo. The system is designed to help users quickly find relevant details from complex insurance documents.

## Features

- **PDF Extraction:** Extracts text and tables from policy documents using `pdfplumber`.
- **Semantic Search:** Utilizes OpenAI embeddings and ChromaDB for fast and accurate document retrieval.
- **Re-ranking:** Uses a cross encoder to refine search results.
- **Response Generation:** Generates user-friendly answers with citations using GPT-3.5-turbo.
- **Caching:** Implements a cache mechanism to speed up repeated queries.

## Prerequisites

- Python 3.7+
- Required libraries (install via pip):
  - pdfplumber
  - tiktoken
  - openai
  - chromadb
  - sentence-transformers
  - pandas

## Dependencies and Requirements
 - pdfplumber==0.6.0 
 - tiktoken==0.3.3 
 - openai==0.27.0 
 - chromadb==0.3.21 
 - sentence-transformers==2.2.2 
 - pandas==1.5.3 
 - numpy==1.23.5


Here we have listed all the necessary Python libraries and their exact versions required to run the project. This ensures that anyone setting up or deploying the project installs the correct dependencies, which helps maintain reproducibility and minimizes version-related issues.

*Note: You may need to adjust version numbers based on your development environment and compatibility requirements.*


## Configure API Keys

- Place your OpenAI API key in a text file (e.g., `OpenAI_API_Key.txt`) and update the file path in the code accordingly.

## Prepare PDF Data

- Store your insurance policy PDFs in a designated folder. Update the file path in the code to point to this folder.

## Documents Used in this Case Study

Here are the links to the documents used in this case study:

- [HDFC Life Easy Health - Policy Bond (Single Pay)](https://www.hdfclife.com/content/dam/hdfclifeinsurancecompany/customer-services/policy-documents-pdf/health-live/HDFC-Life-Easy-Health-101N110V03-Policy-Bond-Single-Pay.pdf)
- [HDFC Life Group Poorna Suraksha - Policy Document](https://www.hdfclife.com/content/dam/hdfclifeinsurancecompany/customer-services/policy-documents-pdf/group-others-live/HDFC-Life-Group-Poorna-Suraksha-101N137V02-Policy-Document.pdf)
- [HDFC Life Group Term Life - Customer Information Sheet](https://www.hdfclife.com/content/dam/hdfclifeinsurancecompany/customer-services/customer-information-sheet/group-others-live/HDFC-Life-Group-Term-Life-101N169V03-Customer-Information-Sheet.pdf)
- [HDFC Life Sampoorna Jeevan - Policy Document](https://www.hdfclife.com/content/dam/hdfclifeinsurancecompany/customer-services/policy-documents-pdf/savings-and-investment-withdrawn/HDFC-Life-Sampoorna-Jeevan-101N158V04-Policy-Document.pdf)
- [HDFC Life Sanchay Plus - Life Long Income Option - Policy Document](https://www.hdfclife.com/content/dam/hdfclifeinsurancecompany/customer-services/policy-documents-pdf/savings-and-investment-withdrawn/HDFC-Life-Sanchay-Plus-Life-Long-Income-Option-101N134V19-Policy-Document.pdf)
- [HDFC Life Smart Pension Plan - Policy Document (Online)](https://www.hdfclife.com/content/dam/hdfclifeinsurancecompany/customer-services/policy-documents-pdf/retirement-live/HDFC-Life-Smart-Pension-Plan-Policy-Document-Online.pdf)
- [HDFC Surgicare Plan - Policy Document](https://www.hdfclife.com/content/dam/hdfclifeinsurancecompany/customer-services/policy-documents-pdf/health-withdrawn/HDFC-Surgicare-Plan-101N043V01.pdf)


## Running the Project

### Execute the Notebook or Script
- Run the main notebook  or execute the Python script to start the pipeline.
- The system will extract text from PDFs, build embeddings, perform semantic search, and generate responses based on user queries.

### Interacting with the System
- When prompted, enter your insurance-related query.
- The system will output a detailed answer with relevant citations from the policy documents.

## Deployment

### Local Deployment
- Follow the setup instructions and run the project locally.

### Cloud Deployment
- The project can be deployed on cloud platforms (e.g., AWS, GCP) by containerizing the application with Docker.
- Ensure API keys and data paths are configured as environment variables.

## Troubleshooting

### Model Loading Issues
- If you encounter errors with model loading (e.g., CrossEncoder), verify that the model name is correct and that your environment has access to the Hugging Face repository.

### API Key Errors
- Ensure that the OpenAI API key is correctly placed and the file path is updated.

## Conclusion

This project demonstrates an end-to-end implementation of a Retrieval-Augmented Generation (RAG) system tailored for the insurance domain. By combining robust document extraction, semantic search, re-ranking, and advanced language models, the system provides accurate and



---

