# sample_set_assignment
Deployment Instructions

To deploy the RAG model, you can install Jupyter notebook locally or use Google colab:

1- Install Ollama and add to your system path https://ollama.com/download
2. Open a terminal and run 'ollama serve'
3. In another terminal download ollama models by 'ollama pull llama3.1'
4. Create a virtual environment 'python -m venv rag_env'
5. Open a terminal Activate 'rag_env' by 'source rag_env/bin/activate' or 'rag_venv/Scripts/bin/activate' depending on OS
6. Using the same terminal where the venv is activated, go inside the shared project via cd <project_folder>
7. pip install -r requirements.txt
8. There is a notebook with name 'Sample_Set_RAG_Assignment.ipynb' shared.
9. Run 'Jupyter notebook' from same terminal where rag_env is active and open the shared Notebook and Run all
 


To deploy the QA bot, you can use a cloud platform like Streamlit Cloud or Heroku. Here are the steps:


1. If the previous instructions have been followed, you will already have the environment and dependencies downloaded.
2. Open a terminal and run 'ollama serve'
3. from same terminal where rag_env is active run command 'streamline run <Project_folder>/src/main.py'
4. A UI will open. Upload any pdf file (Since using local ollma model use PDF< 1mb) and start asking question
5. If you see any error it might be due to memory issue. Run refresh the page or rerun the app.

Minimum memory requirement 8GB+ to load LLM models locally, so make sure to have minimum 16GB RAM