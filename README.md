# 🤖 **Domain-Specific Intelligent Assistant Powered by RAG**

This repository hosts a highly adaptable AI-powered assistant capable of serving domain-specific needs such as medical health, education, finance, or any custom requirement. The assistant uses pre-trained data stored in a vector database to deliver precise and context-aware responses based on user queries.

---

## **About the Assistant**

This intelligent assistant leverages Retrieval-Augmented Generation (RAG) to provide highly relevant and accurate answers. Its design allows easy customization for specific domains, making it a versatile solution for various industries or institutions.

### **Key Features**
- **Customizable Knowledge Base**: Tailor the assistant to any domain by training it on specific documents (e.g., medical guidelines, academic resources, financial policies).
- **Contextual Responses**: Maintains session history to deliver seamless and coherent interactions.
- **Data-Driven Query Resolution**: Utilizes similarity search on vectorized data stored in a Chroma database for generating precise outputs.

---

## **Capabilities**
1. **Adaptable to Any Domain**:  
   - Can be tailored for use cases like medical health assistants, financial advisors, or academic support.  
   - Domain-specific data ensures precise and reliable responses.

2. **Real-Time Query Processing**:  
   - Handles user queries effectively by retrieving and processing the most relevant information.  

3. **Customizable and Scalable**:  
   - Easy to expand with additional datasets for new use cases.  

---

## 🛠️ **Technologies and Tools**
- **LangChain**: Implements retrieval pipelines and conversational frameworks.
- **ChromaDB**: Stores document embeddings for similarity-based retrieval.
- **Google Generative AI**: Provides embeddings and question-answering capabilities.
- **Streamlit**: Creates an interactive user interface.
- **Python**: Handles backend operations and integrations.
- **dotenv**: Manages API keys securely.

---

## **How It Works**
1. **Data Vectorization**: Converts provided documents into vector embeddings using Google Generative AI.  
2. **Vector Storage**: Embeddings are stored in a persistent Chroma database for fast and efficient retrieval.  
3. **Query Resolution**:  
   - Retrieves the most relevant vectors from the database based on user queries.  
   - Processes these vectors to generate accurate and domain-specific responses.  
4. **Context Retention**: Maintains session history to ensure continuity in multi-turn conversations.

---

## 📋 **Setup and Usage Instructions**

### **1. Clone the Repository**

- git clone https://github.com/783atulpatel/Domain-AI-Assistant.git
- cd Domain-AI-Assistant

## **Setup and Usage Instructions**

### **1. Install Dependencies**
- Install the required Python libraries:
- pip install -r requirements.txt

### **2. Configure API Keys**
- Obtain the Gemini API key from Google AI Studio.
- Place the credentials.json file in the project directory.
- Set the GOOGLE_APPLICATION_CREDENTIALS environment variable:

- export GOOGLE_APPLICATION_CREDENTIALS=/path/to/credentials.json


### **3. Prepare Vectorized Data**
- Run the vectorization script to process domain-specific documents:

- python vectorize.py

### **4. Launch the Assistant**
- Start the Streamlit app to interact with the assistant:

- streamlit run main.py

## **Sample Use Cases**
- Medical Domain: Train the assistant with medical guidelines and provide instant answers to health-related queries.
- Financial Domain: Offer financial insights based on policies and market data.
- Education: Support students and faculty with course-related information and academic schedules.

