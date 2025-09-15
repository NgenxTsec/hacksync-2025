# Kurukshetra - AI-Powered Debate Platform

🏆 **HackSync 2025 Champions!**

Kurukshetra is an innovative debate platform that transforms how debates are conducted, judged, and experienced. Designed with fairness, intelligence, and engagement in mind, it leverages cutting-edge AI architectures to provide real-time feedback, automated judgments, and intelligent sparring capabilities.

---

## 🚀 Features

### 💡 1. The 5 Pandavas Judgment Framework

A panel of five specialized LLMs that collaborate to deliver balanced, multi-dimensional debate assessments:

* **Ethos (Credibility)**: Evaluates speaker trustworthiness using **DeBERTa-v3-small**
* **Pathos (Emotion)**: Detects emotional appeal with **DistilBERT Emotion Classifier**
* **Logos (Logic)**: Analyzes reasoning with **DistilBERT MNLI Classifier**
* **Facts (Truthfulness)**: Verifies claims with **Gemini 1.5 Flash**
* **Stoic (Objectivity)**: Provides rational, bias-free evaluation using a **GPT-2 fine-tuned model**

### 🌍 2. Borderless Debating

* Cross-lingual debate capabilities
* Participants can engage in their **preferred languages**
* HuggingFace embeddings + FAISS vector store for multilingual retrieval

### 🤖 3. AI Debate Sparring Partner

* Challenges participants with counterarguments
* Identifies logical flaws in reasoning
* Provides structured **constructive criticism**

### 📰 4. Integrated Fact Verification

* Real-time claim validation through **web search (SerpAPI)** + **vector DB knowledge retrieval**
* Ensures **argument integrity and truthfulness**

---

## 🏗️ Architecture

### Main Debate Platform Architecture

The core platform follows a sophisticated flow:

1. **Input Processing**: Flask API handles client applications via HTTP POST
2. **Input Validation**: Ensures data integrity and format compliance
3. **Process Type Detection**: Distinguishes between ongoing debates and new debate initialization
4. **Retrieval System**: 
   - Fine-tuned GPT-2 model for initial counterargument generation
   - Hybrid retrieval combining FAISS Vector DB and SerpAPI web search
   - Knowledge merging and deduplication
5. **Response Generation**: 
   - Conversational Retrieval Chain
   - Groq API with Mixtral 8x7b model
   - Response parsing for logical flaws and counterarguments
6. **Output Formatting**: JSON response formatting for client consumption

### AI Coach Architecture

The coaching system incorporates:

- **HuggingFace Embeddings** with all-MiniLM-L6-v2 model
- **FAISS Vector Store** for efficient document retrieval
- **Multi-Modal Analysis** supporting user input, topics, and speaker transcripts
- **The 5 Pandavas Framework** for comprehensive evaluation
- **Groq Mixtral-8x7b-32768** for advanced language processing


---

## 👥 Team

Kurukshetra was proudly built by our team Ngenx at **HackSync 2025**, pushing the boundaries of debate, AI, and fairness.
