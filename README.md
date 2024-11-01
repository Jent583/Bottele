## Telegram Message-Sending Protocol

This application utilizes the Telegram Bot API to send messages to users or groups via a Telegram bot. Below is an overview of how the protocol works:

1. **Bot Creation**: To use this application, you need to create a Telegram bot. You can do this by chatting with the [BotFather](https://t.me/botfather) on Telegram. The BotFather will provide you with a unique bot token, which you must keep secure.

2. **API Endpoint**: The application sends HTTP POST requests to the Telegram Bot API endpoint to send messages:
   - **Endpoint**: `https://api.telegram.org/bot<YOUR_BOT_TOKEN>/sendMessage`
   - Replace `<YOUR_BOT_TOKEN>` with the token provided by BotFather.

3. **Request Parameters**: When sending a message, the following parameters are included in the request body:
   - `chat_id`: The unique identifier for the target chat(Get ChatID via @username_to_id_bot).
   - `text`: The message text to be sent.

4. **Response Handling**: Upon sending a message, the application receives a response from the Telegram API. If the message is sent successfully, a success status is returned. If there is an error (e.g., invalid chat ID), an error message will be returned.

5. **Security**: Ensure that your bot token is kept confidential and not exposed in public repositories or client-side code.

By following these steps, users can easily send messages to any Telegram user or group using this application.

# Telegram Message Sender

A simple web application to send messages via Telegram bot.

## Getting Started

1. Clone the repository.
2. Run `npm install` to install dependencies.
3. Start the server using `node server.js`.
4. Open `index.html` in a browser to use the app.

For Try

Bot token: 7625866705:AAGpBt1ELY3WI9dyyWCXfHY58FZogZZTC6U

Start Bot:
useforsample_bot
## License

This project is licensed under the MIT License.
