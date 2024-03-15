# ManPageChat
This is just a simple Artificial Intelligence (AI) Large Language Model (LLM) Chat Bot leveraging Retrieval Augmented Generation (RAG).  It is still in Jupyter Notebook form (sorry, no GUI yet).

## Assumptions
The script assumes that you have Ollama running somewhere with the Mistral:Instruct LLM loaded.  I used OpenShift AI to create the notebook and host Ollama in the OpenShift environment.

## General Use
1.  Download the notebook and import it into Jupyter.
2.  Edit the question at the bottom of the Notebook.
3.  Run all of the steps in the Notebook.  Your original question will be answered when the last block runs.
4.  Edit the question and run the last block in the notebook again to get another answer.

If the chromadb database it not setup yet, it will download about 1,500 web pages from http://www.man7.org and use them to populate the database.  Subsequent runs will be faster.

It does take a little bit of time to answer the query.  Patience is key here.

Note: LLMs are not perfect and tend to only be as accurate as the questions that they are asked.  It is very likely that you will receive some silly answers or ones that are just wrong.  My best suggestion is to rephrase the question and try again.
