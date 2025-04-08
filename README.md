# 🤖 Facebook AI Comment Automation Bot

> Automate your Facebook comment tasks with a powerful AI-enhanced bot designed to mimic human behavior and avoid detection — powered by Gemini AI & Selenium! 🌐💬

---

## 📌 Features

- 💡 **AI-generated comments** using Google Gemini
- 🧠 **Human-like typing & mouse movements**
- 📜 **Auto-logging** for every comment & bot activity
- 🌐 **Uses Chrome with profile support**
- 📊 **Smart delay patterns** to avoid detection
- 🔁 **Supports auto-refresh & comment limits**
- 🧪 Modular and easy to customize

---

## ⚙️ Requirements

- Python 3.10+
- Chrome Browser (installed at default location)
- Facebook account logged into Chrome profile

---

## 📦 Installation

1. **Clone the repository:**

```bash
git clone https://github.com/yourusername/facebook-ai-comment-bot.git
cd facebook-ai-comment-bot
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Set up environment variables in .env:

env
Copy
Edit
POST_URL=https://www.facebook.com/post_url_here
GEMINI_API_KEY=your_gemini_api_key_here
GEMINI_MODEL=gemini-pro
GEMINI_PROMPT=Write a natural and thoughtful comment about the post. Do not include emojis or any introductory phrases or additional text.
⚠️ Make sure your Facebook profile is logged in using the default Chrome profile or update CHROME_PROFILE in the config.

🚀 Usage
Run the bot using:

bash
Copy
Edit
python fb.py
It will:

Launch Chrome with your Facebook profile

Navigate to the specified Facebook post

Generate human-like comments using Gemini AI

Type, pause, scroll, and comment like a real user

🧑‍💻 How It Works
generate_comment() - Uses Gemini API to craft unique, meaningful replies

human_type() - Simulates realistic typing with occasional typos

human_mouse_jiggle() - Random mouse movements like a real user

random_scroll() / random_hover_or_click() - Simulates page engagement

post_comment() - Safely and randomly posts comments over intervals

📂 Logs
Logs are saved with timestamps in the logs/ directory:

bash
Copy
Edit
logs/facebook_comment_bot_YYYYMMDD_HHMMSS.log
Includes detailed status updates and errors.

🛠 Configuration
Edit values in the CONFIG dictionary in fb.py to adjust behavior:

python
Copy
Edit
'MAX_COMMENTS': 100,
'MAX_ITERATIONS': 10000,
'DELAYS': {
    'SHORT_MIN': 0.5,
    'SHORT_MAX': 2.0,
    'MEDIUM_MIN': 1,
    'MEDIUM_MAX': 3,
    'LONG_MIN': 5,
    'LONG_MAX': 20,
    'RELOAD_PAUSE': 180,
}
🧪 Dependencies
selenium

webdriver-manager

google.generativeai

python-dotenv

logging

Install them manually if needed:

bash
Copy
Edit
pip install selenium webdriver-manager python-dotenv google-generativeai
❗ Disclaimer
This project is for educational and research purposes only.

Use responsibly. Automating social platforms may violate their terms of service.

💬 Contact
Created with ❤️ by Daniyal Asghar
Feel free to reach out for improvements, ideas, or collaboration!
