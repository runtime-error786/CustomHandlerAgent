Overview
This project is an AI-driven query routing system that processes user queries and directs them to the appropriate processing category: SQL, Vector, or Wikipedia-based retrieval. The system integrates various AI tools and techniques to generate SQL queries, retrieve relevant information from documents or Wikipedia, and provide detailed answers based on the retrieved context.

Features
SQL Query Processing:

The system can generate SQL queries based on user input related to a predefined students table in an SQLite database.
It executes the SQL query against the database and returns the results in a summarized format.
Vector-Based Retrieval (RAG):

If the query relates to advanced AI topics like Retrieval-Augmented Generation (RAG), it searches for relevant information in a local document database using vector embeddings.
The system uses Hugging Face's all-MiniLM-L6-v2 model for embedding generation and Chroma as the vector store.
Wikipedia-Based Retrieval:

For queries that do not match the SQL or Vector categories, the system retrieves relevant information from Wikipedia using the WikipediaQueryRun and WikipediaAPIWrapper.
Dynamic Routing:

The system dynamically routes queries to the appropriate category (SQL, Vector, or Wikipedia) based on the content of the query.


![image](https://github.com/user-attachments/assets/32cd86e5-1661-4ff8-a5bd-ce45d27b798b)
