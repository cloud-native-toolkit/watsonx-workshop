
## LABs

### Perform the labs in following order - 
### Lab 1 - [Prompt Engineering](https://github.com/cloud-native-toolkit/watsonx-workshop/tree/MUMBAI/labs/Lab%201%20-%20Prompt%20Engineering)
### Lab 2 - [Retrieval Agumented Generation](https://github.com/cloud-native-toolkit/watsonx-workshop/tree/MUMBAI/labs/retrieval-agumented-generation)
### Lab 3 - [watsonx.ai and Langchain](https://github.com/cloud-native-toolkit/watsonx-workshop/tree/MUMBAI/labs/watsonxai-and-langchain)
### Lab 4 - [watsonx.ai with watsonx Assistant and watsonx Discovery](https://github.com/cloud-native-toolkit/watsonx-workshop/tree/MUMBAI/labs/wa_wd_watsonx)

### Prerequisites:

[Laptop Environment Setup](https://github.com/cloud-native-toolkit/watsonx-workshop/tree/MUMBAI/labs/laptop-environment-setup)
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

!pip install python-dotenv
!pip install ibm-generative-ai
!pip install "ibm-generative-ai[langchain]"
!pip install pypdf
!pip install InstructorEmbedding
!pip install 'transformers[torch]'
!pip install sentence-transformers
!pip install Flask flask-restful flask_httpauth
!pip install cachetools
!pip install unstructured
!pip install from-root
!pip install chromadb
!pip install chroma-migrate
!pip install text-extensions-for-pandas
!pip install --upgrade ibm-watson

!pip install matplotlib
pip install ibm-watson-machine-learning

!pip install jupyterlab

NOT REQUIRED
pip install faiss-cpu

```

