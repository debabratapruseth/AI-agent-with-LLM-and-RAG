# 📄 Document Q&A Agent using OpenAI & RAG (Retrieval-Augmented Generation)

This project demonstrates how to build an intelligent Document-Reading AI Assistant using **OpenAI’s GPT-4**, **LangChain**, and **vector database (FAISS)**. The assistant can read and answer questions from various document formats including **PDFs, Word, Excel, HTML, JSON**, and more — all without needing to train a new model.

---

## 🧑‍🏫 Designed for Beginner Python and AI/ML Learners

This beginner-friendly project helps students and enthusiasts learn:

- How to load structured and unstructured documents using LangChain loaders  
- ✂How to split documents into context-aware chunks for retrieval  
- How to create embeddings using OpenAI’s `text-embedding-ada-002` model  
- How to store and retrieve chunks using FAISS (vector database)  
- How to use GPT-4 to generate grounded answers from retrieved chunks  
- Modular, commented Python code designed for self-paced learning

---

## 🧠 How It Works

1. **Document Ingestion**: Load a file (PDF, DOCX, XLSX, HTML, CSV, JSON) using the appropriate LangChain document loader.
2. **Text Chunking**: Split content into manageable pieces for the LLM using smart chunking strategies.
3. **Embedding**: Convert each chunk into vector form using OpenAI Embeddings.
4. **Storage**: Store vectors in FAISS for fast similarity search.
5. **Retrieval + QA**: On user query, the top matching chunks are passed to GPT-4 to answer questions with context.

---

## 📚 Educational Goals

This hands-on AI project will help you:

- Understand the **RAG (Retrieval-Augmented Generation)** workflow  
- Explore **chunking strategies** and their impact on accuracy  
- Practice with **vector stores**, similarity search, and LLM prompting  
- Learn how to **choose loaders** for different document formats  
- Develop real-world AI apps with Python, LangChain, and OpenAI APIs

---

## 🛠️ Technologies Used

- Python 3.x  
- OpenAI GPT-4 / GPT-3.5-turbo  
- LangChain (latest version)  
- FAISS (Facebook AI Similarity Search)  
- Various LangChain document loaders  
- Google Colab (for smooth notebook execution)

---

## 🚀 Getting Started

To try this project:

1. Clone the repository or open the notebook in Google Colab.  
2. Set your OpenAI API key securely as a secret or environment variable.  
3. Install dependencies with `pip install -r requirements.txt` or run the Colab setup cell.  
4. Upload any supported document (PDF, Word, etc.).  
5. Ask questions and explore your own document!

---

## 📂 Supported Document Formats

| File Type     | Recommended Loader                    |
|---------------|----------------------------------------|
| PDF           | `PyPDFLoader`, `PDFPlumberLoader`      |
| Word (DOCX)   | `UnstructuredWordDocumentLoader`       |
| Excel (XLSX)  | `UnstructuredExcelLoader`              |
| HTML          | `UnstructuredHTMLLoader`               |
| CSV           | `CSVLoader`, `PandasCSVLoader`         |
| JSON          | `JSONLoader`                           |
| Websites      | `WebBaseLoader`                        |

---

## 🔮 Future Improvements

- Add support for persistent vector DB saving/loading  
- Create a Streamlit UI for easier user interaction  
- Add summarization fallback when token limit is exceeded  
- Extend support to web scraping (live pages)  
- Enable file upload UI for Gradio apps  

---

## 🧩 Limitations & Notes

- FAISS is in-memory — use Pinecone or Qdrant for production-ready storage  
- Make sure to handle token limits with long documents by chunking wisely  
- This version does not include a frontend — interaction is via notebook only  

---

## 📄 License

This project is open-source under the **MIT License**.

---

👋 If you find this helpful, don't forget to ⭐ the repo and follow for more beginner-friendly AI projects!


