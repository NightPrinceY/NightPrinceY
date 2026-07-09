<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=26&duration=2800&pause=1200&color=2E9EF7&center=true&vCenter=true&width=640&lines=Hi%2C+I'm+Yahya+Elnawasany+(NightPrince);AI+Engineer+%C2%B7+R%26D;I+build+Arabic+speech+%26+voice+AI+systems;TTS+%C2%B7+ASR+%C2%B7+RAG+%C2%B7+LLM+fine-tuning" alt="Typing SVG" />

<img align="right" src="https://komarev.com/ghpvc/?username=NightPrinceY&style=flat-square&color=2E9EF7" alt="Profile Views" />

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/yahya-alnwsany-8b8206238)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:yahyaalnwsany39@gmail.com)
[![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)](https://huggingface.co/NightPrince)
[![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=flat-square&logo=kaggle&logoColor=white)](https://www.kaggle.com/alnwsany)
[![Docker Hub](https://img.shields.io/badge/Docker%20Hub-2496ED?style=flat-square&logo=docker&logoColor=white)](https://hub.docker.com/u/nightprincey)
[![Portfolio](https://img.shields.io/badge/Portfolio-111111?style=flat-square&logo=vercel&logoColor=white)](https://nightprincey.github.io/Portfolio-App/)

</div>

AI Engineer (R&D) focused on **Arabic speech and language AI** — text-to-speech, speech recognition,
retrieval, and LLM fine-tuning — with a specialty in Modern Standard Arabic and Islamic-domain content,
where correctness and pronunciation matter more than almost anywhere else in NLP.

---

## 🎙️ Flagship: Fasih-TTS-V1

A Modern Standard Arabic (Fusha) text-to-speech model, fine-tuned from Coqui XTTS v2 — built to be
**provably correct**, not just fluent.

<img src="https://huggingface.co/NightPrince/Fasih-TTS-V1/resolve/main/assets/poster.png" alt="Fasih-TTS-V1" width="640"/>

- **1.3% CER** against Whisper-large-v3, matching the **1.8%** error floor of the original human
  recordings — the synthetic voice is as understandable as the actor it was trained on.
- **#1 for intelligibility** on [SILMA's open-source Arabic TTS benchmark](https://huggingface.co/spaces/silma-ai/opensource-arabic-tts-benchmark),
  scored independently by **two ASR judges** (Whisper-large-v3 + NVIDIA NeMo) plus UTMOS naturalness —
  every clip, transcript, and score published for anyone to check.
- Ships its own Arabic front-end: **normalize → number expansion → CATT diacritization → sacred-term
  lexicon → chunking** — bare undiacritized input still comes out with correct case endings (iʿrāb).
- **RTF ≈ 0.6**, streaming first-audio **≈ 675 ms**, 24 kHz output.

**[🤗 Model](https://huggingface.co/NightPrince/Fasih-TTS-V1)** ·
**[▶ Live demo](https://huggingface.co/spaces/NightPrince/Fasih-TTS)** ·
**[📝 Write-up](https://huggingface.co/blog/NightPrince/fasih-tts-blog)** ·
**[📊 Benchmark data](https://huggingface.co/datasets/NightPrince/Fasih-TTS-Benchmark)** ·
**[💻 Source](https://github.com/NightPrinceY/Fasih-TTS-V1)**

---

## 🕌 Islamic AI Systems

A connected stack for a religious-Q&A voice assistant — every layer tuned for Arabic and for getting
sensitive content *right*:

| Layer | What it does |
|---|---|
| 🗣️ **Speech out** | [Fasih-TTS-V1](https://github.com/NightPrinceY/Fasih-TTS-V1) — see above |
| 👂 **Speech in** | [Whisper-Arabic-finetuning](https://github.com/NightPrinceY/Whisper-Arabic-finetuning-official-scripts) (Quranic ASR, tashkeel-aware, **CER 0.69% / WER 3.28%**) · [alignment_quran_recitation](https://github.com/NightPrinceY/alignment_quran_recitation) (NeMo FastConformer + forced alignment for recitation checking) |
| 🔎 **Retrieval** | [Quran-Semantic-Retrieval](https://github.com/NightPrinceY/Quran-Semantic-Retrieval), [Hadith_Search](https://github.com/NightPrinceY/Hadith_Search), [Tafsir_Search](https://github.com/NightPrinceY/Tafsir_Search) — hybrid BM25 + FAISS + verse-anchor search across 7 classical Tafsir books |
| 🧠 **Reasoning / persona** | [Muslim-mode-finetuning](https://github.com/NightPrinceY/Muslim-mode-finetuning) (QLoRA on Karnak-6B — tool routing, scope, measured rulings) · [Qwen3-4b-islamic-finetuning](https://github.com/NightPrinceY/Qwen3-4b-islamic-finetuning) · [Mofaser-Dataset](https://github.com/NightPrinceY/Mofaser-Dataset) |
| ⚙️ **Local inference infra** | [qwen3-8b-local-server](https://github.com/NightPrinceY/qwen3-8b-local-server) — OpenAI-compatible vLLM server on 4×RTX 2080 Ti |

---

<details>
<summary><b>📁 More projects</b> (click to expand)</summary>

<br>

- **[FishAudioTTS-Server](https://github.com/NightPrinceY/FishAudioTTS-Server)** — Fish Audio S2-Pro TTS server with Arabic voice cloning
- **[Arabic-Transcriber-Pro](https://github.com/NightPrinceY/Arabic-Transcriber-Pro)** / **[-Live](https://github.com/NightPrinceY/Arabic-Transcriber-Live)** — Arabic transcription tooling
- **[Dual-Stage-Toxic-Moderation](https://github.com/NightPrinceY/Dual-Stage-Toxic-Moderation)** / **[peft-distilbert-toxic-classifier](https://github.com/NightPrinceY/peft-distilbert-toxic-classifier)** — content moderation classifiers
- **[Search_Paper_MCP](https://github.com/NightPrinceY/Search_Paper_MCP)** — MCP server for paper search
- **[-CodeGenBot-RAG-Assistant](https://github.com/NightPrinceY/-CodeGenBot-RAG-Assistant)** — retrieval-augmented code generation assistant
- **[Respiration-App](https://github.com/NightPrinceY/Respiration-App)** — respiration-rate measurement via ML
- **[Helmet-V8](https://github.com/NightPrinceY/Helmet-V8)** — real-time helmet detection with YOLOv8
- **[RosaryApp](https://github.com/NightPrinceY/RosaryApp)** — Flutter app
- **[ShakespeareQ-Generator](https://github.com/NightPrinceY/ShakespeareQ-Generator)** — Shakespearean-style text generation

</details>

---

## 🧠 Tech Stack

**Speech & Audio**
<p align="left">
  <img src="https://img.shields.io/badge/Coqui%20XTTS-2E9EF7?style=flat-square" />
  <img src="https://img.shields.io/badge/Whisper-412991?style=flat-square&logo=openai&logoColor=white" />
  <img src="https://img.shields.io/badge/NVIDIA%20NeMo-76B900?style=flat-square&logo=nvidia&logoColor=white" />
  <img src="https://img.shields.io/badge/torchaudio-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" />
</p>

**LLMs & NLP**
<p align="left">
  <img src="https://img.shields.io/badge/Transformers-FFD21E?style=flat-square&logo=huggingface&logoColor=black" />
  <img src="https://img.shields.io/badge/vLLM-4B0082?style=flat-square" />
  <img src="https://img.shields.io/badge/LoRA%2FQLoRA-8A2BE2?style=flat-square" />
  <img src="https://img.shields.io/badge/FAISS-0467DF?style=flat-square" />
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" />
</p>

**Languages & Infra**
<p align="left">
  <img src="https://skillicons.dev/icons?i=python,cpp,bash,sql,html,css,docker,azure,linux,vscode,git" alt="Stack" />
</p>

**Serving & MLOps**
<ul>
  <li>FastAPI streaming inference servers · Docker containerization</li>
  <li>Modal (serverless GPU deployment) · ONNX / TensorRT optimization</li>
  <li>Multi-GPU local inference (RTX 2080 Ti ×4, vLLM, Accelerate DDP)</li>
</ul>

**Certifications**
<ul>
  <li>DeepLearning.AI TensorFlow Developer Specialization</li>
  <li>Deep Learning Specialization</li>
  <li>Machine Learning Specialization</li>
</ul>

**Spoken Languages**
<p align="left">
  <img src="https://img.shields.io/badge/Arabic-Native-success?style=for-the-badge" />
  <img src="https://img.shields.io/badge/English-Fluent-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/German-Intermediate-lightgrey?style=for-the-badge" />
</p>

---

## 💼 Experience

- **AI Instructor**, iSchool — teaching Python and applied AI to young students
- **Coordinator**, AlMentor — organizing AI/tech education events and workshops
- **Ambassador**, Solve Hub — AI-for-good workshops and events
- **Deep Learning Engineer Intern** — NLP and computer vision model development & deployment

---

## 📊 GitHub Activity

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=NightPrinceY&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true" alt="GitHub Stats" height="165"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=NightPrinceY&layout=compact&hide_border=true&theme=tokyonight&langs_count=8&card_width=320" alt="Top Languages" height="165"/>
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=NightPrinceY&theme=tokyonight&hide_border=true" alt="GitHub Streak" />
</p>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/NightPrinceY/NightPrinceY/output/github-contribution-grid-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/NightPrinceY/NightPrinceY/output/github-contribution-grid-snake.svg" />
  <img alt="contribution snake" src="https://raw.githubusercontent.com/NightPrinceY/NightPrinceY/output/github-contribution-grid-snake.svg" />
</picture>

---

<div align="center">

💬 Building Arabic speech/voice AI or need help with one? Reach out on
**[LinkedIn](https://www.linkedin.com/in/yahya-alnwsany-8b8206238/)** or **[email](mailto:yahyaalnwsany39@gmail.com)**.

</div>
