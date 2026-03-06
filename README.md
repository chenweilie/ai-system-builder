# ai-system-builder

AI-powered systems portfolio that connects computer vision models, LLM automation workflows, and hardware integration APIs to solve real operational problems across multiple domains.

This project demonstrates how AI can be integrated into practical end-to-end operational systems rather than used as isolated model demos.

## Problem

Many real-world operational workflows still rely on manual monitoring, repetitive tasks, or disconnected tools that lack AI automation.

Example scenario:
- Teams need to monitor physical events, automate content pipelines, or control hardware remotely
- Manual processes are slow, error-prone, and do not scale
- No unified AI-to-action pipeline exists that connects perception, reasoning, and execution

The goal of this portfolio is to demonstrate how AI can automate these workflows end-to-end across three engineering domains.

## Solution Overview

This portfolio connects AI models with automation logic and execution actions across Vision, LLM, and Hardware systems.

High-level workflow:
```
Input Source (Camera / API / Structured Data)
       ↓
AI Processing (Vision / LLM / OCR)
       ↓
Decision Logic (Classification / Extraction / Reasoning)
       ↓
Automation Trigger (Event pipeline / Webhook / BLE)
       ↓
System Action (Notification / API call / Hardware)
```

Each project follows a consistent engineering pattern: **Problem → Architecture → Implementation → Result**.

## Architecture

**Computer Vision Domain**
- camera / image input
- object detection (YOLOv8)
- event classification
- real-time alert pipeline

**LLM Automation Domain**
- structured data input
- LLM reasoning and content generation
- multi-model orchestration
- automated publishing workflow

**Vision → LLM → Hardware Domain**
- screen / OCR input
- AI command generation
- BLE transmission layer
- physical HID hardware execution

**Architecture Diagram:**
```
Input
  ↓
AI Model
  ↓
Decision Logic
  ↓
Automation Trigger
  ↓
Action / Notification
```

## Projects

### 1. Delivery Vision Alert
**Repo:** [vision-delivery-alert](https://github.com/chenweilie/vision-delivery-alert)

| | |
|---|---|
| **Problem** | Property owners miss package deliveries with no smart alerting |
| **Architecture** | Camera feed → YOLOv8 detection → event filter → LLM alert composer → push notification |
| **Tech Stack** | Python, YOLOv8, OpenCV, OpenAI API |
| **Result** | Real-time delivery detection with natural-language alerts, < 15s latency |

### 2. ESP32 BLE HID Keyboard
**Repo:** [esp32hid-keyboard](https://github.com/chenweilie/esp32hid-keyboard)

| | |
|---|---|
| **Problem** | No way to automate keyboard input into air-gapped or network-restricted hardware |
| **Architecture** | Android Vision/LLM → BLE GATT → ESP32 → USB HID keystroke injection |
| **Tech Stack** | Android/Kotlin, ESP32 C, BLE, Gemini Vision API |
| **Result** | AI-driven physical keyboard emulation for UEFI, KVM, and restricted servers |

### 3. ClipReader TTS Automation
**Repo:** [ClipReader](https://github.com/chenweilie/ClipReader)

| | |
|---|---|
| **Problem** | Manual reading of AI responses on mobile requires too many taps |
| **Architecture** | Clipboard monitor → Azure TTS → audio playback → Doubao ASR → automated UI response |
| **Tech Stack** | Android/Kotlin, Azure TTS, Doubao ASR, Accessibility Service |
| **Result** | Hands-free AI chatbot consumption pipeline on Android |

## Tech Stack

**AI / ML**
- LLM APIs (OpenAI, Gemini)
- Computer vision (YOLOv8, OpenCV)
- TTS / ASR (Azure, Doubao)

**Backend**
- Python, Node.js, Kotlin
- REST API services
- Workflow automation scripts

**Automation**
- Event trigger pipelines
- BLE GATT protocol
- Accessibility Service automation

**Infrastructure**
- Android / ESP32 edge execution
- Cloudflare / edge services
- GitHub Actions (CI/CD)

## Example Use Cases

This architecture can support:
- Physical logistics monitoring and alerting
- Air-gapped hardware automation
- Mobile AI productivity workflows
- IT operations automation
- Computer vision event pipelines

## Results

Example performance metrics:
- Event detection to action latency: < 15 seconds
- Automated workflows replacing manual monitoring
- Cross-layer AI pipelines from perception to hardware action
- Demonstrated systems across 3 engineering domains

This portfolio demonstrates how AI can drive practical operational efficiency across vision, language, and hardware systems.

## Repository Structure

```
ai-system-builder/
└── README.md           # Portfolio index

Linked repositories:
├── vision-delivery-alert
├── esp32hid-keyboard
└── ClipReader
```

## Future Improvements

Possible extensions:
- Multi-input sensor fusion
- Unified dashboard for all system monitoring
- Additional automation trigger types
- Cross-project orchestration layer
- Real-time system health monitoring

## Author

William Chen  
Applied AI Engineer | AI Integration | Automation Systems

**LinkedIn:** https://linkedin.com/in/william-chen-98264938  
**GitHub:** https://github.com/chenweilie
