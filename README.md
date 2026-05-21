# AI-Powered Multilingual Complaint Resolution Chatbot using Semantic Search and Intelligent Caching


The AI-Powered Multilingual Complaint Resolution Chatbot is an intelligent system developed to improve customer complaint handling using Artificial Intelligence (AI) and Natural Language Processing (NLP). Traditional complaint systems often rely on manual support or simple keyword-based chatbots, which may produce slow and inaccurate responses. This project aims to provide a smarter and faster solution by understanding the meaning of customer complaints and generating appropriate responses automatically.

The chatbot allows users to submit complaints in multiple languages, including English and Tamil. When a complaint is entered, the system first detects the language and translates it into English for processing. The complaint text is then cleaned and converted into embeddings using NLP techniques. These embeddings help the system understand the semantic meaning of the complaint rather than depending only on exact keyword matching.

To improve response speed and efficiency, the chatbot uses two caching mechanisms: exact cache and semantic cache. The exact cache checks whether the same complaint already exists and immediately returns the stored response. The semantic cache identifies complaints with similar meanings using cosine similarity and retrieves relevant responses without processing the complaint again. If no matching complaint is found in the cache, the system performs similarity search using FAISS to retrieve related complaints from the dataset.

The project uses the real-world consumer complaint dataset provided by the Consumer Financial Protection Bureau (CFPB), which contains customer complaints, issue categories, and resolution information. Based on the retrieved complaint data, the chatbot identifies the issue category and generates an appropriate response.

                          ![Architecture Diagram](images/architecture_diagram.png)
                          
The final response is translated back into the user’s original language and displayed along with the similarity score and cache status. This helps improve transparency and demonstrates how the system processes complaints efficiently.

Overall, the proposed chatbot provides a scalable, multilingual, and intelligent complaint management solution that improves response speed, reduces repetitive processing, and enhances user experience through semantic understanding and automated response generation.


