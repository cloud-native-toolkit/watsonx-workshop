# Lab 6: Retrieval Augment Generation (RAG) for Contextual and Timely Answers

### Introduction
In this lab, you will apply Retrieval Augment Generation (RAG) to retrieve then summarize text based on user queries.  Here is a high level view of a RAG implementation.  

<p align="center">
  <img src="images/rag-architecture-with-watson-discovery.png" width="600"/>
</p>

You will not use Watson Discovery, however, in most document-heavy uses cases. Typically, you use Smart Document Understanding in Watson Discovery to extract passaged from documents.  For the following two simplified labs, you will first apply RAG to identify passages within a document that match a user's query.  You will then apply RAG across a large dataset of passages to identify then summarize text to answer a quesions.  You will learn how to evaluate the performance of the RAG passage retrieval technique.

Lab 6.a: [RAG principles using PDFs](./rag-pdf.ipynb)

Lab 6.b: [RAG using vector database and labeled Q&A dataset](./rag-chromadb-flan.ipynb)
