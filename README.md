📄🧠 Document-Based Q&A Chatbot using LangChain & Streamlit
This project demonstrates how to build an intelligent chatbot that can answer questions based on the contents of uploaded documents. It utilizes LangChain for document loading, vectorization, and querying, and Streamlit for the user interface.

🚀 Features
✅ Upload and process PDF, TXT, or DOCX documents

✅ Automatically chunk, embed, and store documents using vector databases

✅ Ask natural language questions and get accurate answers based on document context

✅ Clean and interactive Streamlit UI

✅ Powered by OpenAI and LangChain

📁 Project Structure
bash
Copy
Edit
├── app.py                  # Main Streamlit app
├── utils.py                # Helper functions for document loading & processing
├── requirements.txt        # Python dependencies
├── .env                    # Environment variables (e.g., OpenAI API key)
└── README.md               # Project documentation
🔧 Installation
Clone the repository

bash
Copy
Edit
git clone https://github.com/yourusername/document-qa-chatbot.git
cd document-qa-chatbot
Create a virtual environment (optional but recommended)

bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
Set your OpenAI API key
Create a .env file in the root directory and add your API key:

ini
Copy
Edit
OPENAI_API_KEY=your_openai_api_key
▶️ Run the App
bash
Copy
Edit
streamlit run app.py
The Streamlit app will open in your default web browser. Upload a document, ask questions, and get contextual answers!

🧠 How It Works
Upload Document
Supported formats: .pdf, .txt, .docx

Text Extraction & Chunking
Text is extracted and split into manageable chunks for embedding.

Embedding & Vector Store
Chunks are embedded using OpenAI Embeddings (or any other provider) and stored in a FAISS vector store.

Question Answering
The user’s question is embedded and compared with the vector store to find the most relevant chunks. LangChain then uses an LLM to generate a contextual answer.

🛠 Built With
LangChain

Streamlit

FAISS

Python-dotenv

📌 To Do
 Add support for more document types

 Improve UI/UX with advanced Streamlit widgets

 Integrate persistent vector store (e.g., ChromaDB, Pinecone)

📄 License
This project is licensed under the MIT License. See the LICENSE file for details.

🙌 Acknowledgements
Thanks to the LangChain and Streamlit communities for making cutting-edge AI accessible and easy to integrate.

