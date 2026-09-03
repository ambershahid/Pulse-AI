<div align="center">

# 🔄 WORKFLOW FLOWCHART
### *PulseAI - Always there for you*

Complete n8n workflow breakdown with visual diagram

</div>

---

## 1. 📊 Full Workflow Diagram

```mermaid
flowchart TD
    A[👤 User Message] --> B[🌐 Webhook Node]
    B --> C[🔑 Extract User ID]
    C --> D[🧠 Simple Memory Node]
    D --> E[🤖 Gemini AI Agent]
    E --> F[💬 Generate Response]
    F --> G[📤 Respond to Webhook]
    G --> H[💾 Save to Memory]
    H --> I[✅ End]
    
    style A fill:#6366f1,stroke:#4f46e5,color:#fff
    style D fill:#10b981,stroke:#059669,color:#fff
    style E fill:#f59e0b,stroke:#d97706,color:#fff
    style G fill:#ec4899,stroke:#db2777,color:#fff