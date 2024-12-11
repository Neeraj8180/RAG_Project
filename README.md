# Document Genie

**Document Genie** is a chatbot application built using the Retrieval-Augmented Generation (RAG) framework. It leverages Google's Generative AI model (Gemini-PRO) to provide contextually accurate answers based on the content of uploaded PDF documents.

## Features

- Upload multiple PDF files.
- Processes and breaks down documents into manageable chunks.
- Creates a searchable vector store using FAISS.
- Provides accurate answers to user queries based on document content.

---

## Prerequisites

1. **Python**: Ensure Python 3.8 or later is installed on your system.
2. **Google API Key**: Obtain a Google API key from [Makersuite](https://makersuite.google.com/app/apikey).
3. **Libraries**: Install the required Python libraries as outlined below.

---

## Setup Instructions

### 1. Clone the Repository

```bash
git clone <https://github.com/Neeraj8180/RAG_Project>
cd <RAG-Project>
```

### 2. Install Required Python Libraries

Install the dependencies listed in the code:

```bash
pip install streamlit PyPDF2 langchain langchain-google-genai google-generativeai faiss-cpu
```

### 3. Obtain a Google API Key

- Visit [Makersuite](https://makersuite.google.com/app/apikey) to generate your API key.
- Keep the API key ready to input during runtime.

### 4. Run the Application

Start the Streamlit app:

```bash
streamlit run app.py
```

---

## Usage Instructions

### Step 1: Start the Application

Run the Streamlit app using the above command. The app will open in your default web browser.

### Step 2: Enter Your API Key

- Input your Google API key in the field provided on the main page.

### Step 3: Upload PDF Files

- Use the sidebar to upload one or more PDF files.
- Click the "Submit & Process" button to process the documents.
- Wait for the "Done" message indicating the documents have been processed successfully.

### Step 4: Ask Questions

- Enter your question in the "Ask a Question from the PDF Files" text box.
- The chatbot will provide an accurate response based on the content of the uploaded PDFs.

---

## How It Works

1. **Document Parsing**:
   - Extracts text from uploaded PDF files using `PyPDF2`.
2. **Chunking**:
   - Splits the text into manageable chunks using `RecursiveCharacterTextSplitter` from LangChain.
3. **Vector Store**:
   - Creates a FAISS vector store with embeddings generated using Google's Generative AI.
4. **Question-Answering**:
   - Handles user queries with the context retrieved from the vector store and generates detailed responses.

---

## Troubleshooting

### Common Issues

1. **Missing Dependencies**: Ensure all libraries are installed using the `pip install` command.
2. **Invalid API Key**: Double-check your API key and ensure it's correctly entered.
3. **Processing Errors**:
   - Ensure the uploaded PDFs are not corrupted.
   - Ensure sufficient system memory is available.

### Logs

- Check the Streamlit app logs in the terminal for detailed error messages.

---

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new feature branch.
3. Commit your changes.
4. Open a pull request.

---

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

## Acknowledgments

- [Streamlit](https://streamlit.io/)
- [LangChain](https://langchain.com/)
- [Google Generative AI](https://makersuite.google.com/)

---

### Contact

For questions or feedback, please open an issue on the GitHub repository.

email : neerajkumarjha8180\@gmail.com
