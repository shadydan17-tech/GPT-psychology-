# LAU Psychology AI

An advanced, AI that answer any questions about a person's mental issues or any issue that helps the user deal with their problems. This system utilizes a **4-Tier Architecture** to provide students and faculty with real-time academic guidance and office navigation through a stateful, human-like interface.

##  System Features
*   **Conversational Memory**: Utilizes `ConversationBufferMemory` to maintain dialogue context, allowing for natural follow-up questions and pronoun resolution.
*   **Stateful RAG (Retrieval-Augmented Generation)**: Links a high-performance vector database with the **Llama 3.1 8B** model to ensure answers are grounded in verified departmental data.
*   **High-Speed Inference**: Powered by **Groq**, delivering sub-second response times for campus users.
*   **Professional Persona**: Custom-tuned as a witty yet professional LAU Research Assistant, capable of handling everything from simple greetings to complex academic queries.

##  Technical Architecture
The system is built on a modular **4-Tier Design** to ensure scalability and reliability:
1.  **Presentation Tier**: Streamlit / Google Colab UI for user interaction.
2.  **API/Backend Tier**: Groq Cloud integration for high-performance LLM processing.
3.  **Logic Tier**: LangChain orchestration managing the `ConversationalRetrievalChain`, memory buffers, and retrieval logic.
4.  **Data Tier**: Persistent FAISS Vector Store using `all-MiniLM-L6-v2` embeddings to index departmental knowledge bases.

##  Tech Stack
*   **Language**: Python 3.10+
*   **Frameworks**: LangChain, LangChain-Community, LangChain-Groq
*   **Vector Search**: FAISS (Facebook AI Similarity Search)
*   **Embeddings**: HuggingFace Open-Source Models
*   **Model**: Meta Llama 3.1 8B via Groq

##  Installation & Usage
1. **Clone & Install**:
   ```bash
   git clone [https://github.com/](https://github.com/)[Your-Username]/lau-psych-ipms.git
   pip install langchain-groq langchain-community faiss-cpu langchain-huggingface
