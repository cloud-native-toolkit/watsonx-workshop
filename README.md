
# LABs

### Prerequisites:

```

#FOR MAC OS
export HNSWLIB_NO_NATIVE=1

pyenv install 3.10.2
pyenv global 3.10.2

virtualenv venv -p python3.10
source venv/bin/activate

#pip freeze > requirements.txt
pip install -r requirements.txt

```

  - **Or you can install following libraries separately as well**

```

pip install python-dotenv

pip install "ibm-watson-machine-learning>=1.0.320" | tail -n 1
pip install "pydantic>=1.10.0" | tail -n 1
pip install langchain | tail -n 1

pip install pypdf
pip install InstructorEmbedding
pip install 'transformers[torch]'
pip install sentence-transformers

pip install cachetools
pip install unstructured
pip install from-root
pip install chromadb
pip install chroma-migrate
pip install text-extensions-for-pandas
pip install --upgrade ibm-watson

pip install matplotlib

pip install jupyterlab

NOT REQUIRED
pip install faiss-cpu
pip install ibm-generative-ai
pip install "ibm-generative-ai[langchain]"
pip install Flask flask-restful flask_httpauth
pip install ibm-watson-machine-learning

```

# watsonx-workshop
Integrating WA + WD + WX
