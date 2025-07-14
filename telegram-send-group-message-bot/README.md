Telegram Send Group Message Bot
----------------------
## 🚀 Telegram Send Group Message Bot
## 💡 Quick Overview
This single-file Node.js script automates a Telegram user account. It joins public or private groups and drops scheduled text or photo messages without any complicated logic. The whole flow is visible at a glance so newcomers grasp it in minutes.

## 🌟 Main Uses
📢 Broadcast marketing promos and seasonal deals to multiple groups.
📰 Mirror news posts across channels or relay announcements.
💬 Funnel customer questions into a help chat and send canned answers back.

## 🔧 Requirements and Setup
You only need Node.js, the tdlib binary, an API ID, an API Hash, and two folder paths for session and database, all stored in a dotenv file. No extra build step is required.

## 🛠️ Configuration and Customization
Everything important sits near the top of the file as clear constants. Edit the interval values, flip the changeProfile flag, or point to different text files and you are done. Because the logic is plain JavaScript you can ask ChatGPT to rewrite or extend any function instantly.

## 📈 Real Examples in Action
• Place https://t.me/somePublicGroup inside groups.txt and write Check out our latest promo inside messageToSend.txt. Run node bot.js and the sentence appears once each hour in that group.
• Add a line like photo.jpg followed by three consecutive minus signs then Summer sale starts now in messageToSend.txt. The image uploads with the caption whenever the timer fires.
• Drop a private invite link of the form +AbCdEfGhIjKlMn into groups.txt. The bot imports the invite, joins, and forwards posts right away.
• List many invite links in the same file; the sender moves through them in round-robin fashion to respect Telegram rate limits.
• Write a dozen catchy sentences in messageToSend.txt; a random one is chosen each time to keep content fresh.
• Fill a folder with avatar photos, set changeProfile to true, and the bot picks a new picture before every message.
• Clone the folder, point fresh environment variables at another Telegram account, launch both copies, and you have a small fleet running in parallel.

## 🤝 Smooth Integration
The script exports nothing global, so you can wrap it in a larger Node.js application with a standard require or import call. All source code is present and readable, which makes merging, debugging, or extending completely painless.

Find this code on https://fepo.codes

## Earn 75% on every sale you make with FEPO CODES
Compatible with both FEPO Membership and standalone sales scripts.
https://affi.fepo.codes

Do you need help ?
support@fepo.codes

Do you need developers?
https://discord.fepo.codes
https://tg.fepo.codes
