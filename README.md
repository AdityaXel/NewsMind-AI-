NewsMind AIis a user-friendly news research tool designed for effortless information retrieval. Users can input article URLs and ask questions to receive relevant insights from the stock market and financial domain.

<img width="1272" height="700" alt="Screenshot 2026-07-27 161101" src="https://github.com/user-attachments/assets/54eb8415-7018-457f-975b-7f16aab41cd1" />

Features:
1.Load URLs or upload text files containing URLs to fetch article content.
2.Process article content through LangChain's UnstructuredURLLoader.
3.Construct embedding vectors using NVIDIA AI Embeddings and leverage FAISS, a powerful similarity search library, to enable swift and effective retrieval of relevant information.
4.Interact with NVIDIA-hosted Large Language Models (LLMs) using ChatNVIDIA by submitting queries and receiving accurate answers along with source URLs.

Project Structure:
main.py: The main Streamlit application script.
requirements.txt: A list of required Python packages for the project.
faiss_store_openai.pkl: A pickle file to store the FAISS index.
.env: Configuration file for storing your ChatNvidia API key.
