<div align="center">

# 🔄 WORKFLOW FLOWCHART
### *PulseAI - Always there for you*

Actual n8n workflow used in PulseAI

</div>

---

## 1. 📊 Full Workflow Diagram

```mermaid
flowchart LR
    A[💬 Chat Trigger] --> B[🧠 Window Buffer Memory]
    B --> C[🤖 AI Agent]
    C --> D[⚡ Google Gemini 2.5 Flash]
    D --> E[💬 Chat Response]
    E --> F[💾 Save to Memory]
    F --> G[✅ End]
    
    style A fill:#6366f1,stroke:#4f46e5,color:#fff
    style B fill:#10b981,stroke:#059669,color:#fff
    style C fill:#f59e0b,stroke:#d97706,color:#fff
    style D fill:#ef4444,stroke:#dc2626,color:#fff
    style E fill:#ec4899,stroke:#db2777,color:#fff