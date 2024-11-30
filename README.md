Chat.With.Your.PDF_ChatBot:
Chat.With.Your.PDF_ChatBot is an AI-powered chatbot that enables users to interact with PDF documents through natural language queries. Built using advanced tools such as the langchain library and OpenAI's GPT-3.5-turbo model, this application processes PDF files, extracts relevant information, and provides precise answers to user questions. It is ideal for simplifying research, analyzing documents, and extracting insights seamlessly.

Features
PDF Content Interaction: Upload PDF files and query their content.
Accurate Responses: Receive context-aware answers powered by GPT-3.5-turbo.
Conversational History: Track past interactions for seamless conversation continuity.
Customizable Settings: Configure chain types, document loaders, and database settings.
Setup and Installation
To run this project, ensure you have the required Python libraries installed:

bash
Copy code
pip install langchain
pip install pypdf
pip install openai
pip install tiktoken
pip install -U docarray
pip install -U langchain-community
How It Works
PDF Loading: Upload a PDF file using the PyPDFLoader.
Document Splitting: Use RecursiveCharacterTextSplitter to divide the document into manageable chunks.
Embedding Creation: Generate vector embeddings with OpenAIEmbeddings.
Conversational Chain: Utilize ConversationalRetrievalChain to create a chatbot capable of retrieving and answering based on document content.
Key Components
LangChain: Provides the framework for creating conversational and retrieval chains.
OpenAI GPT-3.5-turbo: Processes user queries and generates responses.
Panel: Builds the interactive dashboard for file upload, conversation, and database queries.
How to Use
Launch the Dashboard: The chatbot's interface is built using Panel. To activate it, use the following script:
python
Copy code
import panel as pn
pn.extension()
dashboard.show()
Interact with PDFs:
Upload a PDF document via the Configure tab.
Start querying content in the Conversation tab.
View database interactions in the Database tab.
Access chat history in the Chat History tab.
Example Usage
python
Copy code
cb = cbfs()
dashboard.show()
Upload a PDF file, enter queries in the input box, and receive instant responses!

Future Enhancements
Add multi-document support.
Enhance the conversational memory for complex interactions.
Integrate with additional file types like DOCX and HTML.
Acknowledgments
LangChain for providing the tools to build conversational AI.
OpenAI for the GPT-3.5-turbo model.
