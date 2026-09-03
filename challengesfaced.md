<div align="center">

# 🛠️ Challenges Faced
### *Building PulseAI - Always there for you*

</div>

---

Building PulseAI with n8n + Gemini + Memory was fun, but not easy.  
Here are the real problems I faced and how I solved them 👇

---

## 1. 🧠 Memory Management

**Challenge:**  
`n8n Simple Memory` was forgetting context after 2-3 messages. The bot felt dumb.

**What I tried:**
- Increased `sessionId` to make memory unique per user
- Added `Window Buffer Memory` to keep last 10 messages

**Solution:**  
Connected `Simple Memory` directly to `AI Agent` node and set `returnMessages: true`.  
Now PulseAI remembers the full conversation flow.

```json
"sessionId": "={{ $json.userId }}"

2.⚡ Gemini API Rate LimitsChallenge:
Gemini 2.5 Flash was giving 429 Too Many Requests during testing.What I tried:Added delays between requestsReduced max tokensSolution:
Added Wait node in n8n for 1 sec + enabled Retry on Fail in HTTP Request node.
Also added error handling to show user: "I'm thinking a bit longer..."

3.🔄 Workflow LoopingChallenge:
Webhook → AI → Memory → Reply loop was creating duplicate messages.What I tried:Debugged for 2 hours 😭Checked every node connectionSolution:
The issue was Respond to Webhook node firing twice.
Fixed by setting Respond: On Received instead of On Last Node

4. 🎯 Prompt EngineeringChallenge:
Gemini was giving robotic, long answers. Didn't feel like "Always there for you".What I tried:10+ different system promptsAdding examples in promptSolution:
Final System Prompt:

You are PulseAI. A friendly, smart AI assistant. 
Be helpful, brief, and personal. 
Remember what the user told you before.
Always be there for them.