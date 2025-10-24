# Jarvis - Discord Bot

Welcome to Jarvis, a Discord bot powered by **Google Gemini**.

## 🌟 Description

This project provides a Discord bot that utilizes the AI capabilities of Google Gemini to interact with users, answer questions, and perform various tasks on your Discord server.

## 🚀 Features (Example - Please Update)

* **AI-Powered Conversation:** Chat with the bot using the advanced Gemini model.
* **Question Answering:** Get answers to questions on a wide range of topics.
* **Custom Commands:** (Please add specific commands you have created here)
* ... (Add more features)

## 🛠️ Installation and Setup

To run the bot locally, follow these steps:

### 1. Prerequisites

* [Python 3.8](https://www.python.org/downloads/) or newer
* A Discord account and a server where you have administrative permissions.
* A [Google Gemini API Key](https://aistudio.google.com/app/apikey).
* A [Discord Bot Token](https://discord.com/developers/applications).

### 2. Clone the Repository

Clone the repository to your local machine:
git clone [https://github.com/ofri09bs/Jarvis-Discord-bot.git](https://github.com/ofri09bs/Jarvis-Discord-bot.git)
cd Jarvis-Discord-bot

**### 3. Install Dependencies**
Install the required libraries using the requirements.txt file:
pip install -r requirements.txt
(Note: Ensure your requirements.txt file contains all necessary libraries, such as discord.py and google-generativeai)

**### 4. Configure Environment Variables**
The bot requires two secret keys to operate. It is highly recommended to store them as environment variables and not directly in the code.

DISCORD_TOKEN: Your Discord bot token.
GEMINI_API_KEY: Your API key from Google AI Studio.
It's recommended to create a .env file in the project's root directory (and add it to your .gitignore as you have already done) with the following content:

DISCORD_TOKEN=your_token_here
GEMINI_API_KEY=your_api_key_here
(You will need to ensure the code in main.py loads these variables, for example, using the dotenv library).

**### 5. Run the Bot**
Start the bot using the command:
python main.py
