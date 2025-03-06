Watsonxai environment url - https://techzone.ibm.com/my/workshops/student/65381d845739e500178a849e

# watsonx.ai and watsonx.governance (Overview) - training

### Prerequisites:

```

#FOR MAC OS (Arm architecture)
export HNSWLIB_NO_NATIVE=1
brew install cmake libomp
declare -x TESSDATA_PREFIX=/usr/share/tesseract-ocr/4.00/tessdata

arch -x86_64 /bin/zsh or arch -x86_64 /bin/bash

# For arm64 Pythons:
~/.pyenv/versions/3.10.2/bin/python -m venv venv

# For x86 Pythons:
~/.pyenv/versions/3.10.2_x86/bin/python -m venv venv

pyenv install 3.11
pyenv global 3.11

pip install --upgrade pip

virtualenv venv -p python3.11
source venv/bin/activate

```

### INSTALLING DEPENDENCIES

```

pip install pip-tools

pip install --no-cache-dir -r requirements.txt --extra-index-url https://download.pytorch.org/whl/cpu

## Uncomment below installs only if you are running this notebook fresh

pip install python-dotenv
pip install pypdf
pip install InstructorEmbedding
pip install 'transformers[torch]'
pip install sentence-transformers
pip install cachetools
pip install unstructured
pip install from-root
pip install chromadb
pip install chroma-migrate
pip install --upgrade ibm-watson

pip install matplotlib
pip install ibm-watson-machine-learning
pip install PyPDF2
pip install langchain | tail -n 1
pip install langchain --upgrade
pip install -U langchain-community

```

### USING requirements.in (OPTIONAL)

  - Finally, run the following command to generate a requirements.txt file:
  
```
pip-compile requirements.in
or
python -m piptools compile

```

TrainingMaterial - Presentation Decks

labs - Hands on labs

### Some important Links for IBM Watsonx Platform Learning:

**IBM Granite LLM**
- https://www.ibm.com/granite

**IBM watsonx Developer Hub**
- https://www.ibm.com/watsonx/developer/get-started/quick-start

**IBM watsonx.ai samples**
- https://github.com/IBM/watsonx-ai-samples/tree/master

**IBM watsonx.ai samples**
- https://github.com/IBM/watsonx-ai-samples/tree/master

**IBM Docling library**
- https://ds4sd.github.io/docling/

**Multi-Task Prompt Tuning**
- https://arxiv.org/pdf/2303.02861.pdf

**Fine Tuning a Slate LLM**
- https://medium.com/@alex.lang/fair-is-fast-and-fast-is-fair-ibm-slate-foundation-models-for-nlp-3508412a4b04

**Good article on the True cost of Generative AI:**
- https://www.linkedin.com/pulse/decoding-true-cost-generative-ai-your-enterprise-maryam-ashoori-phd/


