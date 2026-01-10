# Mini-AutoAid-AI-SMS-BDC-Demo
 Mini-AutoAid is a demo-level AI-powered Business Development Center (BDC) system designed to showcase the core intelligence loop used in modern automotive dealership communication platforms.

                ┌─────────────────────┐
                │  Dealership CRM     │
                │ (Sales & Customer)  │
                └────────┬────────────┘
                         │ CRM Sync
                         ▼
┌──────────────┐    ┌─────────────┐     ┌───────────────────┐
│Inbound Calls │    │Outbound Calls│     SMS/MMS Messaging  │
│  (Twilio,   │<-->|  Dialer AI  │<---> │  Service Layer    │
│  Plivo, etc)│    │  Orchestrator│     │(Normalization &   │
└─────┬────────┘    └─────┬───────┘     │  Metadata Mgmt)   │
      │                  │               └─────┬───────────┘
      ▼                  ▼                     │
┌───────────────┐  ┌───────────────┐          │
│Speech-to-Text │  │Conversation    │          │
│   (STT)       │  │State Manager   │<---------┘
└─────┬─────────┘  └─────┬─────────┘
      │                │
      ▼                ▼
┌─────────────────────────────┐
│ LLM / AI Agent (RAG-enabled)│
│ - Retrieval Augmented Gen   │
│ - Knowledge from CRM        │
└─────┬───────────────────────┘
      │
      ▼
┌───────────────┐
│Text-to-Speech │
│(TTS)          │
└───────────────┘
      │
      ▼
┌───────────────┐
│Human Escalation│
│(Agent Dashboard)│
└────────────────┘

