# PulseAI 🤖✨
### Always there for you

PulseAI is your smart, personal AI assistant that remembers you.
Chat about anything, anytime. It learns from your conversations to give better, more human replies.

No limits. Just smart conversations 24/7.

## 🎥 Demo vedio

Watch PulseAI in action:

https://www.linkedin.com/posts/amber-shahid-684874350_ai-automation-n8n-activity-7499855665138642945-2SA3?utm_source=share&utm_medium=member_desktop&rcm=ACoAAFexdcQB64WadUaxFz6H3bGdWAAFG0bEMLw

---

## 🌟 Key Features

- **🧠 Smart Memory**
  Uses Simple Memory in n8n + Gemini to remember your past chats
- **⚡ Instant Replies**
  Powered by Google Gemini 2.5 Flash for fast, accurate answers
- **🔄 Always On**
  Available 24/7 for work, study, ideas, or just random chats
- **🎯 Personalized**
  The more you talk, the better it gets to know you
- **🔧 Built with n8n**
  Fully automated workflow, easy to extend and deploy

---

## 🏗️ Tech Stack

| Component | Technology |
| --- | --- |
| **AI Model** | Google Gemini 2.5 Flash |
| **Automation** | n8n |
| **Memory** | n8n Simple Memory |
| **Language** | Node.js / JavaScript |
| **Deployment** | Anywhere n8n runs |

---

## 🔄 How It Works

Here's the basic flow of PulseAI:

```mermaid
flowchart LR
A[User Message] --> B[n8n Webhook]
B --> C[Simple Memory]
C --> D[Gemini AI]
D --> E[Send Reply]
E --> F[Save to Memory]

