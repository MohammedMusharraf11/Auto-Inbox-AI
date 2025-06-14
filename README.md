# 📬 Auto Inbox AI — Smart Email Workflow Automation with n8n & OpenAI

Auto Inbox AI is an intelligent inbox management system powered by **n8n** and **OpenAI**, designed to automate email classification and actions like marking, replying, and sending alerts — all without manual intervention.

Built for job seekers and professionals, this system classifies incoming emails (like job application results, referral offers, interview invites, etc.) and automatically:

- Sends relevant updates via Telegram
- Marks emails as read
- Replies with a polite rejection response (if applicable)

> ⚡ This workflow uses LLM-based classification with a custom set of job-related categories and makes your inbox act like an agent.

---

## 🧠 How It Works


![Workflow Screenshot](https://github.com/user-attachments/assets/d550c5c0-b89a-4697-a8bb-125a2b07d833)
1. **Gmail Trigger**: Checks for new incoming emails.
2. **Text Classifier (OpenAI GPT-4o-mini)**: Classifies the email into one of several predefined categories:
   - Shortlisted / Viewed
   - Referral Offered
   - Interview / Assessment Invite
   - Rejected
   - Spam / Irrelevant
   - Job Board Notification
3. **Conditional Actions**:
   - **Sends Telegram alerts** with contextual messages.
   - **Marks mails as read** when necessary.
   - **Sends an automatic reply** if the mail is a rejection (with a polite message).
   
---

## 📂 Files Included

- `Inbox_Manager.json`: The exported n8n workflow. You can import this directly into your n8n instance.
- `a41de676-bfc8-4b8b-989a-a7d5991cd50a.png`: Visual snapshot of the flow.

---

## 🚀 How to Use

1. Import the `Inbox_Manager.json` into your n8n editor.
2. Set up credentials:
   - Gmail OAuth2
   - Telegram Bot API
   - OpenAI API (GPT-4o or gpt-3.5-turbo works too)
3. Configure your custom Telegram chat ID and Gmail account.
4. Activate the workflow and let it manage your inbox!

---

## 🧰 Built With

- [n8n.io](https://n8n.io)
- OpenAI GPT (via LangChain Classifier Node)
- Gmail API
- Telegram Bot API

---

## 🙋‍♂️ About the Creator

Made by **Mohammed Musharraf**, a GenAI + Automation enthusiast exploring agentic AI for real-world productivity.

🔗 [LinkedIn](https://www.linkedin.com/in/mohammed-musharraf11/) | [GitHub](https://github.com/MohammedMusharraf11)

---

## 📜 License

MIT License
