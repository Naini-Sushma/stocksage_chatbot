# StockSage 📈

**Your professional, AI-powered stock market educator.**

StockSage is an interactive, beginner-friendly AI chatbot designed to educate users about the stock market. Built for the GENAI Internship, this project serves as a frontend web application that leverages advanced Large Language Models to break down complex financial questions into clear, confident answers.

## 🚀 Features

- **Educational Focus:** Strictly programmed to teach concepts, explain terminology, and provide historical context.
- **No Financial Advice:** Hardcoded to strictly refuse personalized investment advice or stock picks.
- **Rich Text Rendering:** Uses `marked.js` to format AI responses nicely with bold text and headers, and `DOMPurify` to ensure maximum security against XSS attacks.
- **Dynamic UI:** Features an auto-resizing input box, typing indicators, and clickable "Quick Start" suggestion chips (e.g., "What is an IPO?").
- **Clear Chat:** Easily wipe the conversation clean with a single click.

## 🏗️ Architecture

StockSage is built on a simple, serverless foundation:
1. **Frontend UI:** Built with HTML/CSS/JS, it handles the user interface and tracks the chat history in memory.
2. **Context Manager:** Since AI models forget past messages, the app compiles the entire conversation history and a strict System Prompt into every request.
3. **AI Integration:** The context payload is sent via asynchronous REST `fetch` calls to the **Groq API**, ensuring the UI never freezes while waiting for the AI response.

## 🛠️ Tech Stack

- **Frontend:** HTML5, CSS3, Vanilla JavaScript
- **AI Integration:** Groq API (REST integration)
- **Deployment:** Vercel

## ⚙️ How to Run Locally

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/Naini-Sushma/stocksage_chatbot.git

2. Open the project folder and start a local development server:
  npm install
  npm run dev
3. Open the provided localhost URL in your browser to start chatting!
 
⚠️ Disclaimer
StockSage is for educational purposes only and does not provide investment advice.

👨‍💻 Author
Built by Sushma Naini | Built for GENAI Internship | StockSage

