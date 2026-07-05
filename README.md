# AI Grammar Correction Automation Workflow

An AI-powered grammar correction workflow built with n8n, Google Drive, and Google Gemini. The workflow automatically monitors a Google Drive folder, extracts text from newly uploaded PDF files, corrects grammar and writing mistakes using AI, and saves the corrected version back to Google Drive.

📌 Project Overview

This workflow automates the grammar correction process for PDF documents. Whenever a new PDF is uploaded to a specific Google Drive folder, the workflow is triggered automatically. The document is downloaded, its text is extracted, sent to an AI Agent for grammar correction, and the corrected text is saved as a new file in Google Drive.

This project demonstrates how AI can be integrated with cloud storage and workflow automation to reduce manual editing and improve document quality.

🚀 Features
📂 Automatically monitors a Google Drive folder.
📄 Downloads newly uploaded PDF files.
🔍 Extracts text from PDF documents.
🤖 Uses Google Gemini AI for grammar correction.
✍️ Corrects:
Grammar mistakes
Spelling mistakes
Punctuation
Sentence structure
Capitalization
📝 Preserves the original meaning of the content.
☁️ Saves the corrected document back to Google Drive.
⚡ Fully automated with no manual intervention.
🛠️ Tech Stack

Technology	Purpose
n8n	Workflow Automation
Google Drive	File Storage & Trigger
Google Gemini	AI Language Model
Extract From File Node	PDF Text Extraction
Google Drive Create File	Save Corrected Document
📂 Workflow Architecture
Google Drive Trigger
        │
        ▼
Download PDF File
        │
        ▼
Extract Text From PDF
        │
        ▼
Google Gemini AI Agent
        │
        ▼
Create Corrected Text File
        │
        ▼
Google Drive

# Workflow visual
![image alt](https://github.com/n8n-workflows-projects/AI-grammer-checker/blob/e1b357beb030a4b485371706dec9b124df5f7ef4/Screenshot%202026-07-05%20121523.png)

🔄 Workflow Explanation
1. Google Drive Trigger
Watches a specific folder.
Detects newly uploaded PDF files.
Starts the workflow automatically.
2. Download File
Downloads the uploaded PDF.
Converts it into binary format.
Makes the file available for processing.
3. Extract From PDF
Reads the binary PDF.
Extracts readable text.
Passes the extracted content to the AI Agent.
4. AI Grammar Correction Agent

The AI Agent reviews the extracted text and performs:

Grammar correction
Spelling correction
Punctuation fixes
Sentence restructuring
Capitalization correction
Readability improvements

The AI keeps the original meaning unchanged while improving the overall quality of the writing.

5. Create Corrected File

The corrected text is converted into a new text document.

The workflow saves the corrected version to Google Drive without modifying the original file.

🤖 AI Agent Responsibilities

The AI Agent acts as a professional English grammar assistant.

Its responsibilities include:

Correct grammar mistakes
Correct spelling errors
Improve punctuation
Improve sentence clarity
Maintain the author's original meaning
Produce natural and professional English
Avoid adding or removing information
📁 Input

Supported File Type:

PDF (.pdf)

Example:

Student_Assignment.pdf
📁 Output

Generated File:

Student_Assignment_Corrected.txt

The corrected file contains:

Improved grammar
Correct spelling
Better readability
Professional sentence structure
📷 Workflow Screenshot

Add your workflow screenshot here.

images/workflow.png
📋 Prerequisites

Before running this workflow, make sure you have:

n8n installed
Google Drive account
Google Drive OAuth credentials
Google Gemini API credentials
A Google Drive folder for monitoring
PDF documents for testing
⚙️ Setup Instructions
Import the workflow into n8n.
Connect your Google Drive credentials.
Connect your Google Gemini credentials.
Select the Google Drive folder to monitor.
Activate the workflow.
Upload a PDF to the monitored folder.
Wait for the workflow to process the document.
View the corrected file in Google Drive.
📈 Use Cases
Student assignment correction
Resume grammar improvement
Research paper proofreading
Business document editing
Email draft correction
Content writing assistance
Educational institutions
Documentation review
🎯 Learning Outcomes

This project demonstrates how to:

Build an AI-powered automation workflow in n8n.
Integrate Google Drive with workflow automation.
Process PDF documents automatically.
Use AI for language correction.
Handle binary files and extracted text.
Create end-to-end document processing pipelines.
🔮 Future Enhancements
Support Microsoft Word (.docx) files.
Generate corrected PDF files instead of text files.
Highlight grammar changes.
Send email notifications after processing.
Store correction history in Google Sheets.
Support multiple languages.
Add plagiarism detection.
Generate downloadable correction reports.
👨‍💻 Author

Bhoomini Gokam

AI Automation Enthusiast | n8n Workflow Developer | AI Agent Builder

⭐ If you found this project useful

If this workflow helped you or inspired your own automation projects, consider giving the repository a ⭐ on GitHub. It helps others discover the project and supports future improvements.
