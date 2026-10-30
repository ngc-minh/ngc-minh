<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=220&section=header&text=Hi%2C%20I'm%20Minh&fontSize=58&fontAlignY=36&animation=fadeIn&desc=AI%20Engineer%20%C2%B7%20Computer%20Vision%20%C2%B7%20LLM%20%C2%B7%20Edge%20AI&descSize=20&descAlignY=58" width="100%" />
</p>

<p align="center">
  <a href="https://github.com/ngc-minh">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&duration=3000&pause=900&color=0A66C2&center=true&vCenter=true&width=700&height=40&lines=Building+vision+systems+for+real+cameras;Detection+%C2%B7+Tracking+%C2%B7+Recognition;LLM+agents%2C+RAG+and+voice+AI;Edge+AI+on+Jetson+and+ESP32" alt="Typing animation" />
  </a>
</p>

<p align="center">
  Student at Hanoi University of Mining and Geology · Based in Hanoi, Vietnam 🇻🇳
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Focus-Computer%20Vision-0A66C2?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Also-LLM%20%26%20Agents-6F42C1?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Edge-Jetson%20%7C%20ESP32-2EA44F?style=for-the-badge" />
</p>

---

## 🧭 About me

I build practical AI systems that run on real cameras and real hardware, from detection and tracking models to the pipelines and dashboards around them. I also build chatbots, RAG systems and agent workflows with LLMs.

- 👁️ **Computer Vision** – object detection, segmentation and multi-object tracking (YOLO family, ByteTrack, ONNX deployment)
- 📹 **Video analytics** – multi-camera RTSP pipelines, people counting, license plate recognition, PPE and safety monitoring
- 🤖 **LLM & agents** – chatbots, RAG, multi-agent assistants, voice agents
- 🔌 **Edge & embedded** – NVIDIA Jetson, Raspberry Pi, ESP32

## 🛠️ Tech stack

What I use, and what I've actually built with it.

| Area | Tools | What I've done with them |
|---|---|---|
| 👁️ **Detection & tracking** | YOLOv8 · YOLO11 · ByteTrack · Ultralytics · Supervision | Tracked people and vehicles across several cameras at once; built restricted zones, line crossing counts, loitering alerts and crowd detection; crowd-density heatmaps with clustering of bounding boxes. |
| 🧑‍🤝‍🧑 **Recognition** | InsightFace (SCRFD, ArcFace) · FAISS · FER+ · fast-alpr | Face recognition for VIP / blacklist and classroom attendance, emotion and mask detection, uniform matching with ResNet18 embeddings, license plate detection and OCR with a watch list. |
| ⚡ **Inference & deployment** | ONNX · CUDA | One shared detector batching frames from every camera, models exported to ONNX, automatic fallback from GPU to CPU. |
| 📹 **Video pipeline** | RTSP · OpenCV · MediaMTX · WebRTC / HLS · DeepStream 7.1 | Read multi-channel streams from NVR and IP cameras with auto-reconnect, restream to browsers, snapshots and event clips. |
| 🧠 **Edge computing** | NVIDIA Jetson Orin NX · Docker Compose · Mosquitto (MQTT) | Headless production stack: camera → DeepStream → WebRTC and MQTT → backend and dashboard, plus a written guide to rebuild it from scratch. |
| 🔌 **Embedded & IoT** | ESP32 · ESP32-CAM · Arduino / C · Raspberry Pi | Periodic photo capture on ESP32-CAM, LED control over UART, and GPIO control with Raspberry Pi. |
| 💬 **LLM & RAG** | Gemini (OpenRouter) · ChromaDB · VLM | Document Q&A with source and page citations, order-taking through tool calls, multi-agent version with intent routing, image understanding for product questions. |
| 🤖 **Agents** | Claude · tool use · TikTokLive · Facebook Graph API | Shopper agents (search, cart, booking) and operations agents (revenue, stock, price proposals) with human approval before any write; a livestream agent that reads comments and answers from a product list. |
| 🎙️ **Voice AI** | LiveKit Agents · PhoWhisper · VieNeu-TTS · LMDeploy | Vietnamese real-time voice assistant: speech-to-text, GPU-optimized text-to-speech and an LLM for answers. |
| 🌐 **Backend & dashboards** | FastAPI · Flask · NiceGUI · Node / Express · PostgreSQL | REST APIs, event databases, on-premise monitoring dashboards and a sales admin backend. |
| 🖥️ **Frontend** | React · Vite · JavaScript · TypeScript | Admin web app for orders and products; chat widgets and landing pages. |
| 📊 **Data** | Python · Jupyter | Credit card fraud detection, churn prediction, time series forecasting, and scraping and analysing national exam scores. |
| 🧰 **Tooling** | Docker · uv · Git · Linux · Bash | Containerized deployment, reproducible Python environments, on-premise Linux servers. |

## 🚀 Featured work

Most of my recent work lives in private repositories, so here is a summary of what I've built (no client names or code shown).

### 👁️ Computer Vision & Video Analytics

| Project | What it does | Tech |
|---|---|---|
| **Smart camera platform** | Runs fully on-premise: multi-camera input (RTSP / webcam / video), object detection and tracking, restricted zones, line counting, loitering and crowd alerts with snapshots and clips, pushed to Telegram or webhooks. Web UI for configuration. | YOLO11, ByteTrack, FastAPI, CUDA |
| **Community security cameras** | Crowd detection, license plate recognition with a watch list, and fire alerts across multiple RTSP cameras. A single inference pass serves both people and vehicles. | YOLOv8, ByteTrack, fast-alpr (ONNX), NiceGUI |
| **Retail customer analytics** | VIP / blacklist face recognition, emotion and mask detection, and entry-exit counting, built as a modular pipeline with instant alerts. | InsightFace, FAISS, ONNX, ByteTrack |
| **Classroom vision** | Face-based attendance, uniform recognition and crowd-density heatmaps. One shared detector batches frames from all cameras. | YOLOv8, ArcFace, ResNet18, FastAPI |
| **PPE safety monitoring** | Detects missing protective equipment. Final project of the Samsung Innovation Campus ([public repo](https://github.com/ngc-minh/Safety_warning)). | Python, YOLO |

### 🔌 Edge & Video Infrastructure

| Project | What it does | Tech |
|---|---|---|
| **Edge vision on Jetson Orin NX** | End-to-end production stack: IP camera → DeepStream → WebRTC and MQTT → backend and dashboard, all containerized and headless. Includes a step-by-step guide to rebuild it from scratch. | DeepStream 7.1, MediaMTX, Mosquitto, FastAPI, Docker Compose |
| **Open-source VMS with 8 AI analyzers** | Video management system with recording, WebRTC / HLS viewing and AI analyzers plugged into a shared detector. Events flow through MQTT into a central event database and web app. | MediaMTX, MQTT, RTSP |

### 🤖 LLM, Agents & Full-stack

| Project | What it does | Tech |
|---|---|---|
| **RAG chatbots** | Document Q&A with source and page citations, plus order-taking through tool calls. Built as a multi-agent version with intent routing and a lean single-flow version. | ChromaDB, Gemini, OpenRouter, uv |
| **Commerce agents on Claude** | Shopper agents (search, cart, policies, booking) and operations agents (revenue, stock, pricing proposals) where every change needs human approval. Includes a livestream comment-reply agent. | Claude, tool use, Python |
| **Vietnamese voice agent** | Real-time voice assistant with Vietnamese speech-to-text, GPU-optimized text-to-speech and an LLM brain. | LiveKit Agents, PhoWhisper, LMDeploy, Gemini |
| **Sales admin dashboard** | Back-office web app for orders and products. | React, Vite, Node / Express, PostgreSQL |

### 📚 Public repositories

[Track & count objects (YOLOv8 + ByteTrack)](https://github.com/ngc-minh/Track-Count-Objects-using-YOLOv8-ByteTrack-Supervision) · [ESP32-CAM capture](https://github.com/ngc-minh/ESP32Cam_TakePhoto) · [ESP32 UART control](https://github.com/ngc-minh/ESP32_UART) · [Credit card fraud detection](https://github.com/ngc-minh/credit-card-fraud) · [Time series forecasting](https://github.com/ngc-minh/Time-Series-Forecasting-Model-Using-Python)

## 🐍 Contribution snake

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ngc-minh/ngc-minh/output/github-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ngc-minh/ngc-minh/output/github-snake.svg" />
    <img alt="Contribution snake animation" src="https://raw.githubusercontent.com/ngc-minh/ngc-minh/output/github-snake.svg" />
  </picture>
</p>

## 📫 Let's connect

<p>
  <a href="mailto:nguyenngocminha3@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://github.com/ngc-minh"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
</p>

<p align="center"><i>Open to internships and collaboration on computer vision and AI projects.</i></p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=120&section=footer" width="100%" />
</p>
