# Jarvis - Discord Bot

Welcome to Jarvis, a sophisticated, personality-driven Discord bot that emulates **'Jarvis'** from Iron Man.

## 🌟 Description

This bot uses Google Gemini to hold witty, in-character conversations. It's designed to be loyal to its creator, address users as 'Sir', and provide short, precise answers.

The bot remembers your conversation history on a **per-channel basis** and will only respond when triggered directly.

## 🚀 Features

* **Advanced AI Personality:** Powered by Google Gemini (`gemini-1.5-flash`) with a detailed system instruction to act exactly like Jarvis.
* **Channel-Specific Memory:** Jarvis remembers the context of your conversation in *each channel* separately.
* **Multiple Triggers:** You can talk to Jarvis by:
    1.  Mentioning him (`@Jarvis`)
    2.  Starting your message with his name (`jarvis ...`)
    3.  Replying to one of his messages.
* **Creator Recognition:** The bot is hard-coded to recognize its owner via the `BOT_OWNER_ID` and respond with special loyalty and permissions.
* **Moderation Tools:** Includes a native `timeout` command for server moderation.
* **Fun Commands:** Includes several 'fun' commands like `activate`, `leak`, and `ban_this_guy`.
* **Uptime Ready:** Includes a built-in Flask web server, making it easy to deploy on services like Replit that require a web server to stay alive.

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
(Note: Ensure your requirements.txt file contains all necessary libraries, such as discord.py, google-generativeai, Flask, and python-dotenv)

**###4. Configure Environment Variables**
This bot requires three secret keys. Create a .env file in the project's root directory:

DISCORD_TOKEN: Your Discord bot token.

GEMINI_API_KEY: Your API key from Google AI Studio.

BOT_OWNER_ID: (Crucial) Your personal Discord User ID. This is used for admin commands and special recognition.


**###5. Run the Bot**
Start the bot using the command:
python main.py

**💬 Usage**

**How to Talk to Jarvis (using gemini)**

Jarvis will only respond if you trigger him in one of these three ways:

Mention: @Jarvis Hello, how are you?

Name Prefix: jarvis, what's the weather today? (*important*: call him jarvis with lowercase j not upper!)

Reply: Simply reply to any of Jarvis's messages.

If you just mention him (@Jarvis) with no prompt, he will respond with "Yes sir?".

**Command Prefix**

**The prefix for all commands is "Jarvis " (important: note the space at the end, and the uppercase J).**

**⚙️ Available Commands**
Here are the custom commands built into the bot:

**Moderation:**
  
*Jarvis timeout <@member> <time> [reason]*

Times out a user for a specified duration.

This requires both you and the bot to have "Moderate Members" permissions.

Time format: 10s (10 seconds), 5m (5 minutes), 1h (1 hour), 2d (2 days).

Example: Jarvis timeout @Noam 10m being annoying

**Utility**

*Jarvis reset*

Clears Jarvis's conversation memory for the current channe

This command can only be used by the bot's creator (as defined in BOT_OWNER_ID).


**Fun**

*Jarvis activate <mode>*

Activates a special "mode" and sends a GIF.

Modes: freaky, ragebait

Special Mode: admin (Only usable by the bot's creator).

*Jarvis ban_this_guy*

A fun command that asks who to ban and then posts a "banning" message (does not actually ban anyone).

*Jarvis leak <name>*

A fun command that pretends to leak a user's info and sends a GIF.

you can play with him and add as much commands as you like! enjoy!
