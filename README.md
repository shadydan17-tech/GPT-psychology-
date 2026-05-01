# 🧠 Psychology Research Assistant (IPMS)

An AI-powered **Indoor Positioning Management System (IPMS)** logic layer designed for psychology research. This system utilizes **Retrieval-Augmented Generation (RAG)** to provide accurate, context-aware answers from a 70MB psychology dataset.

---

## 🚀 Features
*   **One-Shot Retrieval:** Uses `RetrievalQA` to eliminate infinite loops and iteration errors.
*   **High-Level Reasoning:** Powered by **Llama 3.3 70B** via Groq for research-grade synthesis.
*   **Cloud-Native:** Built to run in Google Colab with direct Google Drive integration for large vector databases.
*   **Efficient Search:** Uses FAISS and HuggingFace `all-MiniLM-L6-v2` embeddings.

---

## 🛠️ Tech Stack
*   **Language:** Python 3.10+
*   **LLM API:** Groq (Llama 3.3 70B / Llama 3.1 8B)
*   **Framework:** LangChain
*   **Vector Store:** FAISS
*   **Embeddings:** HuggingFace Transformers

---

## 📋 Prerequisites

Before running the project, ensure you have:
1.  **Groq API Key:** Obtain one from [console.groq.com](https://console.groq.com/).
2.  **Google Drive:** A folder named `psych_vector_db` containing your `index.faiss` and `index.pkl` files.
3.  **Environment:** Google Colab is recommended for the Drive mounting features.

---

## ⚙️ Setup & Installation

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/psychology-assistant-ipms.git](https://github.com/YOUR_USERNAME/psychology-assistant-ipms.git)
   cd psychology-assistant-ipms
