<div align="center">

# 🔄 WORKFLOW FLOWCHART
### *PulseAI - Always there for you*

Vertical workflow for easy reading

</div>

---

## 1. 📊 Vertical Workflow Diagram

```mermaid
flowchart TD
    A[💬 Chat Trigger<br/>User sends message] 
    --> B[🧠 Window Buffer Memory<br/>Loads last 10 messages]
    --> C[🤖 AI Agent<br/>Combines Memory + Message]
    --> D[⚡ Google Gemini 2.5 Flash<br/>Generates Reply]
    --> E[💬 Chat Response<br/>Sends answer to user]
    --> F[💾 Save to Memory<br/>Stores new conversation]
    --> G[✅ End]

    style A fill:#6366f1,stroke:#4f46e5,color:#fff,stroke-width:2px
    style B fill:#10b981,stroke:#059669,color:#fff,stroke-width:2px
    style C fill:#f59e0b,stroke:#d97706,color:#fff,stroke-width:2px
    style D fill:#ef4444,stroke:#dc2626,color:#fff,stroke-width:2px
    style E fill:#ec4899,stroke:#db2777,color:#fff,stroke-width:2px
    style F fill:#8b5cf6,stroke:#7c3aed,color:#fff,stroke-width:2px
    style G fill:#6b7280,stroke:#4b5563,color:#fff,stroke-width:2px

Step 1: You → "I love Python"
Step 2: Memory → []
Step 3: Gemini → "That's awesome! Python is great 🔥"
Step 4: Memory → [You: I love Python] [AI: That's awesome!]

Step 5: You → "Which language do I like?"
Step 6: Memory → [You: I love Python] [AI: That's awesome!]
Step 7: Gemini → "You told me you love Python"