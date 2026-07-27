# 📰 NewsMind AI

**NewsMind AI** is a user-friendly news research application that enables users to analyze financial and stock market news effortlessly. Simply provide one or more news article URLs, and the application extracts, processes, and indexes the content using **LangChain**, **NVIDIA AI Embeddings**, and **FAISS**. Users can then ask natural language questions and receive context-aware answers along with the relevant source URLs.

## 📸 Screenshot

> Add your application screenshot here.

![NewsMind AI](Screenshot%202026-07-27%20161101.png)


##  Features

-  Load news article URLs or upload a text file containing multiple URLs.
-  Extract and process article content using **LangChain's UnstructuredURLLoader**.
-  Generate semantic embeddings using **NVIDIA AI Embeddings**.
-  Store and search embeddings efficiently with **FAISS Vector Store**.
-  Query the indexed articles using **ChatNVIDIA** to receive accurate, context-aware responses.
-  Display the source URLs used to generate each answer for transparency.

---

##  Project Structure

```text
NewsMind-AI/
│── main.py                  # Main Streamlit application
│── requirements.txt         # Project dependencies
│── faiss_store_openai.pkl   # Serialized FAISS vector database
│── .env                     # NVIDIA API Key configuration
└── README.md                # Project documentation
```

---

##  Tech Stack

- Python
- Streamlit
- LangChain
- ChatNVIDIA
- NVIDIA AI Endpoints
- NVIDIA Embeddings
- FAISS
- UnstructuredURLLoader



##  Environment Variables

Create a `.env` file in the project root and add:

```env
NVIDIA_API_KEY=your_nvidia_api_key
```


##  How It Works

1. Enter one or more news article URLs.
2. The application extracts the article content.
3. Text is split into smaller chunks.
4. NVIDIA AI Embeddings convert the text into vector representations.
5. FAISS indexes the vectors for fast semantic retrieval.
6. Ask questions in natural language.
7. ChatNVIDIA retrieves the most relevant information and generates an answer with source references.


##  Future Improvements

- Support PDF and document uploads
- Chat history and conversation memory
- Multiple LLM support
- Real-time news ingestion
- Advanced filtering and summarization
