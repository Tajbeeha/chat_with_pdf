Project Overview :
The Chat with PDF project allows users to upload PDF documents, extract and process their content, and then interact with the extracted data through a conversational interface. Users can ask questions related to the uploaded PDFs, and the application will retrieve relevant information and generate accurate responses using Google Generative AI.

Project Features :
PDF Text Extraction: Extracts text content from uploaded PDF files.
Text Chunking: Splits the extracted text into manageable chunks for efficient processing.
Embeddings Creation: Converts text chunks into vector embeddings for similarity search.
FAISS Vector Store: Uses FAISS to store embeddings and perform similarity searches.
Conversational Q&A: Allows users to ask questions and receive contextually accurate answers based on the PDF content.

Packages Used :
streamlit: For creating the interactive user interface.
PyPDF2: For extracting text from PDF files.
langchain.text_splitter.RecursiveCharacterTextSplitter: For splitting text into chunks.
os: For interacting with the operating system.
langchain_google_genai.GoogleGenerativeAIEmbeddings: For generating text embeddings using Google's generative AI model.
google.generativeai: For configuring and using Google’s generative AI models.
langchain.vectorstores.FAISS: For creating and managing the FAISS vector store to store embeddings.
langchain.chains.question_answering.load_qa_chain: For setting up the question-answering chain.
langchain.prompts.PromptTemplate: For defining the prompt structure for generating answers.
dotenv: For loading environment variables securely from a .env file.

Step-by-Step Process
1. Environment Setup
* Install the required Python packages:
             pip install streamlit PyPDF2 langchain google-generativeai faiss-cpu dotenv
  
2. Add API Key to .env
* Create a .env file in the root directory of the project.
* Add your Google API key in the following format:
* GOOGLE_API_KEY=your_api_key_here
* This key is used to authenticate and interact with Google’s generative AI services.
  
3. PDF Text Extraction
4. Text Chunking
5. Embedding Creation
6. Vector Store Creation
7. Question Retrieval
8. Answer Generation
9. User Interaction through Streamlit UI

Running the Application :
* Make sure all dependencies are installed.
* Set up your Google API key in the .env file.
* Run the application with the following command:
              streamlit run app.py
* Open the URL provided by Streamlit in your web browser to interact with the application.
  
Example Usage :
Upload PDF Files: Users can upload one or more PDF files via the file uploader in the Streamlit app.
Ask Questions: After the PDF files are processed, users can ask questions related to the content of the PDFs.
Get Responses: The application retrieves the relevant context and generates a detailed answer using the Google Generative AI model.

Conclusion :
This project showcases how to combine document processing, text retrieval, and generative AI to create a powerful conversational assistant for PDFs. The use of FAISS for similarity search and Google Generative AI for response generation ensures accurate and context-aware answers to user queries.
