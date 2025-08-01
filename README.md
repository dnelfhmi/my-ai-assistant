---
title: career_conversation
app_file: app.py
sdk: gradio
sdk_version: 5.34.2
---

# 🤖 AI Career Conversation Assistant

An intelligent chatbot that represents **Muhammad Daniel Fahmi** for career-related conversations, powered by OpenAI GPT-4o-mini and deployed on Hugging Face Spaces.

## 🚀 Live Demo

**Try it now:** [https://huggingface.co/spaces/dnelfhmi/career_conversation](https://huggingface.co/spaces/dnelfhmi/career_conversation)

## ✨ Features

- 💬 **Interactive Career Conversations** - Ask about skills, experience, and background
- 📧 **Contact Collection** - Automatically captures interested prospects' contact details
- 🔔 **Real-time Notifications** - Pushover integration for instant alerts on new conversations
- 📄 **Comprehensive Profile** - Loads data from LinkedIn PDF, CV, and personal summary
- 🛠️ **Smart Tool Calling** - Records unknown questions and user details automatically

## 🏗️ Architecture

- **Frontend:** Gradio ChatInterface
- **AI Model:** OpenAI GPT-4o-mini
- **Document Processing:** PyPDF for LinkedIn profile extraction
- **Notifications:** Pushover API
- **Deployment:** Hugging Face Spaces

## 🔧 Tech Stack

- **Python 3.12+**
- **OpenAI API** - Language model and tool calling
- **Gradio** - Web interface framework
- **PyPDF** - PDF text extraction
- **Pushover** - Push notifications
- **uv** - Package management

## 📁 Project Structure

```
├── app.py                 # Main application
├── development.ipynb      # Development & experimentation
├── pyproject.toml        # Project dependencies
├── me/
│   ├── linkedin.pdf      # LinkedIn profile
│   ├── summary.txt       # Personal summary
│   └── cv.md            # CV/Resume
└── README.md
```

## 🚀 Quick Start

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd my-ai-assistant
   ```

2. **Install dependencies**
   ```bash
   uv sync
   ```

3. **Set up environment variables**
   ```bash
   # Create .env file
   OPENAI_API_KEY=your_openai_api_key
   PUSHOVER_TOKEN=your_pushover_token
   PUSHOVER_USER=your_pushover_user
   ```

4. **Run the application**
   ```bash
   python app.py
   ```

## 🔨 Development

The project includes a comprehensive Jupyter notebook (`development.ipynb`) for experimentation and testing new features.

## 🔮 Potential Improvements

### High Priority
- **🛡️ OpenAI SDK Integration** - Migrate from manual API calls to official OpenAI SDK for simplified code, better error handling, and automatic retries
- **🧠 Agentic Patterns** - Implement Evaluator-Optimizer pattern for self-improving conversations and response quality assessment
- **📊 Conversation Analytics** - Add metrics tracking for conversation quality, user satisfaction, and engagement patterns

### Medium Priority
- **🔄 Multi-turn Context Management** - Enhanced memory for longer, more coherent conversations
- **🎯 Intent Classification** - Categorize user queries for more targeted responses
- **🌐 Multi-language Support** - Expand beyond English for international reach

### Lower Priority
- **🔍 RAG Implementation** - Retrieval-Augmented Generation for more accurate and up-to-date information
- **💾 SQL Database Integration** - Store common Q&A pairs for faster responses and reduced API costs
- **📈 Advanced Analytics Dashboard** - Comprehensive insights into user interactions and conversation patterns

## 🤝 Contributing

Feel free to submit issues and pull requests to improve the assistant's capabilities!

## 📄 License

This project is open source and available under the MIT License.