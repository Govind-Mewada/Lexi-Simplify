# Lexi-Simplify: Demystifying Legal Documents with AI

## Project Overview

**Lexi-Simplify** is a prototype web application built for the GenAI Exchange Hackathon. It addresses the significant societal problem of complex legal documents being inaccessible to the average person. Our solution leverages Google Cloud's generative AI to bridge this information gap, empowering individuals to understand critical documents like rental agreements, contracts, and terms of service without professional legal assistance.

## Features

This prototype demonstrates the following key functionalities:

* **Intelligent Summarization:** Paste or upload a legal document, and the AI generates a concise, jargon-free summary of its contents.

* **Conversational Q&A:** Ask specific questions about the document, and the AI provides clear, direct answers based on the text.

* **Multi-format Document Support:** Supports direct text input as well as file uploads for `.txt`, `.md`, `.html`, `.json`, `.pdf`, and `.docx` files.

* **Intuitive Drag-and-Drop:** Easily upload documents by simply dragging and dropping them into the designated area.

## Technologies Used

* **Frontend:** HTML, Tailwind CSS, JavaScript

* **AI Backend:** Google Cloud's **Gemini API** (`gemini-2.5-flash-preview-05-20`) for document understanding and text generation.

* **Hosting:** The single-file architecture makes it easy to deploy on any simple web server (e.g., GitHub Pages, Netlify, Vercel).

## Live Prototype

You can view the live, working prototype here:
[**https://govind-mewada.github.io/Lexi-Simplify/**](https://govind-mewada.github.io/Lexi-Simplify/)

## How It Works

The application operates as a single-page web app. When a user pastes text or uploads a file, a prompt is dynamically constructed in JavaScript. For file uploads, the document is read and sent to the Gemini API as `inlineData` within the API request. The Gemini API then processes the content and returns a simplified summary or a direct answer to the user's question. This approach ensures a seamless user experience while leveraging the full power of the multimodal model.

## Installation and Usage

To run this project locally, you only need to host the `index.html` file on a simple web server.

1. **Clone the repository:**


Frontend: HTML, Tailwind CSS, JavaScript

AI Backend: Google Cloud's Gemini API (gemini-2.5-flash-preview-05-20) for document understanding and text generation.

Hosting: The single-file architecture makes it easy to deploy on any simple web server (e.g., GitHub Pages, Netlify, Vercel).

Live Prototype
You can view the live, working prototype here:
https://govind-mewada.github.io/Lexi-Simplify/

How It Works
The application operates as a single-page web app. When a user pastes text or uploads a file, a prompt is dynamically constructed in JavaScript. For file uploads, the document is read and sent to the Gemini API as inlineData within the API request. The Gemini API then processes the content and returns a simplified summary or a direct answer to the user's question. This approach ensures a seamless user experience while leveraging the full power of the multimodal model.

Installation and Usage
To run this project locally, you only need to host the index.html file on a simple web server.

Clone the repository:

git clone [https://github.com/](https://github.com/)<your-username>/<your-repo-name>.git

Navigate to the project directory:

cd <your-repo-name>

Open index.html in your browser. For security, your browser may not allow local file access to the API. It is recommended to use a live server extension in your code editor or a simple local server like Python's http.server.

# Run a simple Python web server
python -m http.server

Then, open http://localhost:8000 in your browser.

Note: The application requires a valid API key for the Gemini API. The index.html file is configured to receive this from the Canvas runtime, but for local testing, you will need to insert your key.

Disclaimer
This tool is a hackathon prototype for demonstration purposes only. It is not a substitute for professional legal advice. The answers and summaries provided by the AI may not be entirely accurate or complete. Please consult with a qualified legal professional for any legal concerns.


Developed by Govind Mewada ❤️
