# Daily Quote Bot
# 🤖 AI Motivation Telegram Bot (n8n Automation)

An automated Telegram bot built with **n8n** that delivers daily inspiration. This project integrates multiple APIs to provide a seamless user experience with interactive menus and visual content.

## 🚀 Features
- **Interactive Navigation:** Uses Telegram Reply Keyboards for easy user interaction.
- **Dynamic Content:** Fetches random quotes from the Quotable API.
- **Visual Aesthetics:** Integrates with Unsplash/Picsum API to deliver high-quality random images paired with quotes.
- **Clean UI:** Implemented custom formatting to optimize message presentation and branding.

## 🛠️ Tech Stack
- **Automation Tool:** [n8n.io](https://n8n.io/)
- **APIs:** Telegram Bot API, Quotable API, Picsum Photos.
- **Logic:** Conditional Switching, Binary Data Handling, REST API Integration.

## 📈 Workflow Logic
1. **Trigger:** User sends a command via Telegram (/start, /quote, /help).
2. **Switch:** The bot evaluates the command and routes to the appropriate path.
3. **Data Fetching:** Parallel requests to fetch a text quote and a random image.
4. **Processing:** Merging the quote text into the image caption.
5. **Delivery:** Sending the final visual message back to the user.

## 📂 How to Use
1. Download the `DailyQuoteBot.json` file from this repository.
2. Import the file into your **n8n** instance.
3. Configure your Telegram Credentials with your `Bot Token`.
4. Set the `Chat ID` in the Telegram nodes.
5. Execute and Enjoy!

## 🛠️ Step-by-Step Setup

### 1. Create Telegram Bot API Token
1. Open Telegram and search for **@BotFather**.
2. Send the command `/newbot` and follow the instructions to name your bot.
3. Copy the **API Token** provided (e.g., `123456789:ABCDefGh...`).
4. **Safety Note:** Never share this token publicly!

### 2. Resources Used
To make this bot work, I used the following public APIs:
- **Quotes API:** [Quotable API](https://api.quotable.io/random) - Used for fetching randomized inspirational quotes.
- **Image API:** [Picsum Photos](https://picsum.photos/) - Used for high-quality random background images.
- **Platform:** [n8n Cloud/Self-hosted](https://n8n.io/) - The brain that connects all services.

### 3. Detailed Workflow Configuration
- **Command Router:** A `Switch` node that filters incoming text commands like `/start` or `/quote`.
- **Image Fetcher:** An `HTTP Request` node set to `Response Format: File` to handle binary image data.
- **Content Delivery:** A `Telegram` node using the `Send Photo` operation to merge the image and the quote as a caption.
---
*This project is part of my journey in mastering **System Automation** and **Network Administration**. I am also currently working on Python-based projects like **AI Smart Cleaner** and exploring network topologies in **Cisco Packet Tracer**.*


### Workflow Preview
![Workflow Diagram](https://github.com/Faiz-Mubarok/n8n-work-harder/blob/main/WorkflowQuoteBot.jpg?raw=true)

### Bot Preview
![Bot Result](https://github.com/Faiz-Mubarok/n8n-work-harder/blob/main/Hasil%20Quote%20Bot.jpg?raw=true)
