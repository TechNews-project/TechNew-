# TechNews

## Run the website and Telegram contact endpoint

The contact form sends messages through the Node.js server. Keep the Telegram bot token on the server; never put it in `JS/script.js` or another browser-loaded file.

1. Revoke the previously shared bot token with BotFather and create a replacement.
2. Copy `.env.example` to `.env` and set `BOT_TOKEN` to the replacement token and `CHAT_ID` to the destination chat ID.
3. Install dependencies with `npm install`.
4. Start the site with `npm start` and open `http://localhost:3000/contact-page.html`.

The `.env` file is excluded from git. Configure the same environment variables in your hosting provider when deploying; static-only hosting cannot run the `/api/contact` endpoint.
