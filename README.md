
![WhatsApp Image 2024-07-10 at 11 28 58_48cf7c4b](https://github.com/SatyajeetPatra-11/AUDIRE_Document_Analysis/assets/117520211/8b50df96-e77a-4091-b67c-24846077feae)

"AUDIRE : COHORT OF DATA (Document Analysis) " : This is a Streamlit application that allows users to upload PDF files and interact with a conversational AI assistant to ask questions about the content of the uploaded documents. 

## Features

  1. **Streamlit Application**:
    - The application is built using the Streamlit framework, which provides a user-friendly interface for interacting with the AI assistant.
    - It includes functionality for file uploading, chat history management, and the display of the conversational interface.
  2. **Conversation Management**:
    - The conversation_chat() function handles the interaction between the user and the AI assistant, processing the user's query and generating a response.
    - The conversation history is stored in the Streamlit session state, allowing the application to maintain context across multiple user interactions.
  3. **LangChain Integration**:
    - The create_conversational_chain() function sets up the LangChain components, including the LLaMa language model, the conversation memory, and the conversational retrieval chain.
    - The conversational retrieval chain combines the language model and a vector store (FAISS) to provide relevant responses based on the uploaded PDF content.
  4. **PDF Processing**:
    - The application supports the upload of multiple PDF files.
    - The text content of the uploaded PDFs is extracted and split into smaller chunks using the PyPDFLoader and RecursiveCharacterTextSplitter from LangChain.
    - The text chunks are then embedded using the HuggingFace Embeddings model and stored in the FAISS vector store.
  5. **FAISS Vector Store**:
    - FAISS (Facebook AI Similarity Search) is a high-performance vector indexing and search library that enables efficient similarity-based retrieval.
    - In this project, FAISS is used to index the text embeddings of the PDF content, allowing the conversational retrieval chain to quickly find the most relevant information to answer user queries.
  6. **Conversation Display**:
    - The display_chat_history() function handles the rendering of the chat interface, displaying the user's questions and the AI assistant's responses.
    -It uses the message() function from the streamlit_chat library to format and present the conversation in a user-friendly manner.
  7. **Multiple PDF upload for Query**
     - The application allow user to upload multiple pdfs for easy querying on the data present inside it at a time .  

 
## Technologies Used
  
- *HuggingFace Modal*
- *HuggingFace Embeddings*
- *Langchain*
- *Streamlit*
- *Python*
- *PyPDF*

![WhatsApp Image 2024-07-10 at 11 28 58_552b71d9](https://github.com/SatyajeetPatra-11/AUDIRE_Document_Analysis/assets/117520211/5a8f145c-f6ea-4218-9569-161a5e8436e4)

![Screenshot 2024-03-05 101307](https://github.com/SatyajeetPatra-11/AUDIRE_Document_Analysis/assets/117520211/1683fc84-cd48-418a-adc5-2aff974c742b)

