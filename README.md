<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=FC466B,3F5EFB&height=200&section=header&text=GenerativeAI-LLM&fontSize=70&fontColor=ffffff&animation=twinkling" width="100%" />

<img src="https://img.icons8.com/?id=M1bt3ZHCANRW&format=png&size=100" width="90" />

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=2500&pause=1000&color=FC466B&center=true&vCenter=true&width=700&height=50&lines=Language%20Model%20Question%20Generation;Transformers%20+%20FastAPI%20%28fork%20of%20lmqg%29" alt="Typing SVG" />

[![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)](#)
[![FastAPI](https://img.shields.io/badge/FastAPI-API-009688?style=for-the-badge&logo=fastapi&logoColor=white)](#)
[![Transformers](https://img.shields.io/badge/Transformers-FFD21E?style=for-the-badge)](#)
[![License](https://img.shields.io/github/license/AfnanSharif/GenerativeAI-LLM?style=for-the-badge&color=yellow)](LICENSE)

</div>

---

## 📖 Overview

**GenerativeAI-LLM** (package `lmqg`) generates questions (and question-answer pairs) from
text using pretrained language models via the HuggingFace inference API, with a FastAPI demo
(`app.py`) and a local variant (`app_local.py`).

## 🏗️ Project Layout

```
GenerativeAI-LLM/
├── lmqg/                  # Library — question generation models & inference
├── app.py                   # FastAPI demo (HuggingFace inference API)
├── app_local.py                # FastAPI demo (local model)
├── tests/
└── setup.py
```


## ⚡ Setup & Run

### 🪟 Windows / 🍎 macOS / 🐧 Linux
```bash
git clone https://github.com/AfnanSharif/GenerativeAI-LLM.git
cd GenerativeAI-LLM

python -m venv venv
# Windows: venv\Scripts\activate | macOS/Linux: source venv/bin/activate
pip install -e .

uvicorn app:app --reload --port 8000     # or: python app_local.py for the local-model variant
```

### 🐳 Docker (all platforms)
```bash
docker build -t generative-llm .
docker run -p 8000:8000 generative-llm
```

---

<div align="center">

**Created by [AfnanSharif](https://github.com/AfnanSharif)** · ⭐ star this repo if it helped you

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=FC466B,3F5EFB&height=80&section=footer" width="100%" />

</div>
