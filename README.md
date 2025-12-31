# bot_project_AI-agent-and-Gemini
🌉 Workflow Architecture
The workflow follows a linear logic path with a centralized "Brain" (AI Agent):

Telegram Trigger: Listens for incoming messages via the Telegram Bot API.

AI Agent (Core): Processes the input using a reasoning loop.

Google Gemini Chat Model: Provides the underlying LLM logic for text generation and understanding.

Simple Memory: Stores previous interactions (2 items total) to maintain conversation context and "remember" what was said.

Telegram Output: Sends the generated response back to the user.

🛠️ Components
Automation Platform: n8n

AI Model: Google Gemini (Generative AI)

Channel: Telegram Bot API

Memory Type: Simple Window Memory (Context retention)

🚀 Setup Instructions
1. Prerequisites
An n8n instance (Cloud or self-hosted).

A Telegram Bot Token (obtainable via @BotFather).

A Google AI API Key (obtainable via Google AI Studio).

2. Import the Workflow
Copy the workflow.json file from this repository.

In your n8n dashboard, click Add Workflow > Import from File.

Paste the JSON or upload the file.

3. Credential Configuration
You will need to set up credentials for the following nodes:

Telegram Trigger & Send Message: Add your Telegram Bot Token.

Google Gemini Chat Model: Add your Google AI API Key.

📝 Configuration Details
Memory: Currently configured for Simple Memory with a capacity of 2 items, ensuring the bot stays on track without losing the immediate context of the conversation.

Model: Uses the Google Gemini Chat Model for optimized performance and high-speed responses.
