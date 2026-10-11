Zapier - This project automates scheduled domain-related email notifications using Zapier, Google Sheets, and Gmail. It sends emails based on the information given, updates the status in the spreadsheet, and maintains records of sent emails for verification. This reduces manual effort and improves the efficiency of domain management.
RAG n8n - RAG(X) is a Retrieval-Augmented Generation (RAG) chatbot built using n8n Cloud and Google Gemini. Its purpose is to answer user questions based on information retrieved from a provided PDF document rather than relying on general knowledge.

Workflow
PDF Upload: The user uploads a PDF through an n8n Form Trigger.
Text Extraction: The Extract From File node extracts text from the PDF.
Document Processing: The Default Data Loader prepares the extracted text for indexing.
Knowledge Storage: Gemini embeddings convert text into numerical representations, which are stored in a Simple Vector Store.
Question Answering: A Chat Trigger receives user questions, and an AI Agent retrieves relevant information from the vector store.
Response Generation: Google Gemini generates an answer based on the retrieved information.
Technology Used
n8n Cloud for workflow automation
Google Gemini for AI-generated responses and embeddings
Simple Vector Store for document retrieval
PDF documents as the knowledge source
