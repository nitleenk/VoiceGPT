# VoiceGPT
Telegram Chatbot with GPT-3.5 Turbo and Voice Support

**1. Introduction**
This Python script sets up a Telegram chatbot that utilizes OpenAI's GPT-3.5 Turbo language model to respond to both text and voice messages. The chatbot integrates with the Telegram platform through the `python-telegram-bot` library and leverages the power of the `openai` library to interact with the GPT-3.5 Turbo API.

**2. API Key Setup**
Before running the script, you need to obtain two API keys:

- **Telegram API Token**: To get this token, create a new Telegram bot using the BotFather and replace `<YOUR TELEGRAM API>` with the token provided.
- **OpenAI GPT-3.5 Turbo API Key**: Sign up for the OpenAI API and acquire an API key. Replace `<YOUR API KEY>` with your actual key.

**3. Chatbot Functionality**
The chatbot operates with the following capabilities:

- **Text Messages**:
  - Users can send text messages to the chatbot.
  - The chatbot maintains a conversation history and sends it along with the user's message to GPT-3.5 Turbo for a response.
  - The bot replies to the user with the GPT-3.5 Turbo response.
  - The assistant's reply is appended to the conversation history for future interactions.

- **Voice Messages**:
  - Users can send voice messages to the chatbot.
  - The chatbot replies to the user, acknowledging receipt of the voice message.
  - The voice message is downloaded and transcribed using OpenAI's Whisper ASR model.
  - The transcribed text is sent to GPT-3.5 Turbo for a response.
  - The bot replies to the user with the GPT-3.5 Turbo response.
  - The assistant's reply is appended to the conversation history.

**4. Telegram Integration**
The script utilizes the `python-telegram-bot` library to integrate the chatbot with the Telegram platform. It sets up an Updater, Dispatcher, and adds MessageHandlers for text and voice messages.

**5. Dependencies**
The script requires the installation of `python-telegram-bot`, `openai`, and `moviepy` libraries.

