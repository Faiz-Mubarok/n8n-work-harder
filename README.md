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

---
*This project is part of my journey in mastering **System Automation** and **Network Administration**. I am also currently working on Python-based projects like **AI Smart Cleaner** and exploring network topologies in **Cisco Packet Tracer**.*


### Workflow Preview
![Workflow Diagram](https://github.com/Faiz-Mubarok/n8n-work-harder/blob/main/WorkflowQuoteBot.jpg?raw=true)

### Bot Preview
![Bot Result](https://github.com/Faiz-Mubarok/n8n-work-harder/blob/main/Hasil%20Quote%20Bot.jpg?raw=true)
