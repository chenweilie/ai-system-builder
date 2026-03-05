# Applied AI Systems Portfolio

> **Vision · LLM · Hardware Integration** — Real-world AI pipelines built end-to-end by [@chenweilie](https://github.com/chenweilie)

---

## About

This portfolio showcases applied AI engineering across three domains:
- **Computer Vision** → detection, alerting, real-time inference
- **LLM Automation** → content pipelines, API orchestration, multi-model workflows
- **Vision → LLM → Hardware** → full-stack systems bridging software AI with physical devices

Each project follows a consistent engineering pattern: **Problem → Architecture → Implementation → Result**.

---

## Projects

### 1. Delivery Vision Alert
**Repo:** [vision-delivery-alert](https://github.com/chenweilie/vision-delivery-alert)

| | |
|---|---|
| **Problem** | Property owners miss package deliveries; no smart alerting without expensive subscriptions |
| **Architecture** | Camera feed → YOLOv8 object detection → event filter → LLM notification composer → push alert |
| **Tech Stack** | Python, YOLOv8, OpenCV, OpenAI API |
| **Result** | Real-time delivery detection with natural-language alert messages, zero cloud subscription |

```
[Camera] → [YOLOv8 Detector] → [Event Filter]
                                       ↓
                              [LLM Message Composer]
                                       ↓
                              [Push Notification]
```

---

### 2. LLM Content Automation (petinsure-autopublish)
**Repo:** [petinsure-autopublish](https://github.com/chenweilie/petinsure-autopublish)

| | |
|---|---|
| **Problem** | Content teams spend hours writing SEO articles; manual publishing is slow and inconsistent |
| **Architecture** | Topic scheduler → LLM content generator → SEO formatter → CMS auto-publish API |
| **Tech Stack** | Python, OpenAI/Claude API, WordPress REST API |
| **Result** | Fully automated end-to-end content pipeline; reduces publishing time from hours to minutes |

```
[Topic Scheduler] → [LLM Generator] → [SEO Formatter]
                                              ↓
                                   [CMS Auto-Publish API]
```

---

### 3. LLM Workflow Agent
**Repo:** [llm-workflow-agent-demo](https://github.com/chenweilie/llm-workflow-agent-demo)

| | |
|---|---|
| **Problem** | Complex multi-step tasks require chaining multiple LLM calls with state management |
| **Architecture** | Task decomposer → parallel LLM agents → result aggregator → structured output |
| **Tech Stack** | Python, LangChain / direct API, OpenAI |
| **Result** | Modular agent framework with reusable workflow nodes; demonstrates production-grade LLM orchestration |

---

### 4. AI API Integration Demo
**Repo:** [ai-api-integration-demo](https://github.com/chenweilie/ai-api-integration-demo)

| | |
|---|---|
| **Problem** | Developers need a reference implementation for integrating multiple AI APIs reliably |
| **Architecture** | Unified API client → multi-provider adapter (OpenAI, Gemini, Claude) → response normalizer |
| **Tech Stack** | Python, REST APIs, async I/O |
| **Result** | Drop-in adapter pattern enabling provider-agnostic AI integration |

---

### 5. Vision → LLM → Hardware (esp32hid-keyboard)
**Repo:** [esp32hid-keyboard](https://github.com/chenweilie/esp32hid-keyboard)

| | |
|---|---|
| **Problem** | Air-gapped/restricted environments cannot run standard clipboard or keyboard automation |
| **Architecture** | AI workflow output → LLM text formatter → ESP32 BLE HID → physical keyboard injection |
| **Tech Stack** | Kotlin/Android, ESP32, BLE HID, LLM APIs |
| **Result** | Physical HID device that receives AI-generated text and types it into any target device via Bluetooth |

```
[AI Output / LLM Response]
          ↓
[Android App — BLE Commander]
          ↓
[ESP32 BLE HID Keyboard]
          ↓
[Target Device — any OS, air-gapped]
```

---

### 6. AI Portfolio Casebook
**Repo:** [ai-portfolio-casebook](https://github.com/chenweilie/ai-portfolio-casebook)

Deep-dive case studies for each project above: design decisions, tradeoffs, performance benchmarks, and lessons learned.

---

## Architecture Overview

```
┌─────────────────────────────────────────────────────┐
│              Applied AI Systems Stack                │
├───────────────┬─────────────────┬───────────────────┤
│  Vision Layer │   LLM Layer     │  Hardware Layer   │
│  YOLOv8       │  OpenAI/Claude  │  ESP32 BLE HID    │
│  OpenCV       │  LangChain      │  Android BLE      │
│  Camera feeds │  Agent chains   │  Physical devices │
└───────────────┴─────────────────┴───────────────────┘
         ↓               ↓                ↓
    Real-time        Automated        Cross-device
    alerting         pipelines        AI injection
```

---

## Skills Demonstrated

| Skill | Projects |
|---|---|
| Computer Vision (YOLOv8) | vision-delivery-alert |
| LLM API Orchestration | llm-workflow-agent-demo, ai-api-integration-demo |
| End-to-End Automation | petinsure-autopublish |
| Hardware + AI Integration | esp32hid-keyboard |
| Multi-provider AI Adapters | ai-api-integration-demo |
| Agent / Workflow Design | llm-workflow-agent-demo |

---

## Contact

- GitHub: [@chenweilie](https://github.com/chenweilie)
- Open to: AI Engineer / ML Engineer / Backend Engineer roles

---

*Portfolio maintained and updated regularly. Screenshots, demo GIFs, and architecture diagrams are in each project's `/docs` folder.*
