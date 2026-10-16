# Invoice Agent Automation

## Overview
This project automates invoice processing using AI and workflow automation. It uses n8n to detect new invoice files, extract information from PDF documents, store the extracted data, and send an email notification.

## Workflow
1. **Invoice Detection:** Google Drive trigger detects a new file in the specified folder.
2. **File Download:** Downloads the invoice file from Google Drive.
3. **Text Extraction:** Extracts text from the PDF invoice.
4. **AI Information Extraction:** Google Gemini extracts invoice-related information, including vendor name, address, email, and payment method.
5. **Data Storage:** Saves the extracted information to Google Sheets.
6. **Email Generation:** Google Gemini drafts an invoice notification.
7. **Email Delivery:** Gmail sends the notification automatically.

## Technologies Used
- **n8n** — workflow automation
- **Google Drive** — invoice file storage and detection
- **Google Gemini** — AI-powered information extraction and email generation
- **Google Sheets** — structured data storage
- **Gmail** — automated email notifications

## Key Features
- Automated invoice file detection
- PDF text extraction
- AI-based invoice information processing
- Automatic spreadsheet updates
- AI-generated email notifications
- Integration between multiple Google services

## Project Status
Portfolio project. Google service credentials, folder IDs, spreadsheet IDs, and other required settings must be configured before running the workflow.

## Security Note
The workflow JSON shared in this repository is a sanitized export. Configure your own credentials and resource IDs before importing and running it. Do not upload API keys, passwords, or private customer invoice data.
