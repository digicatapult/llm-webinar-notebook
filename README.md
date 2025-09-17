# LLM Webinar Series: Advanced LLM Capabilities Supplement Jupyter Notebook

## Bridge AI Programme

Innovate UK BridgeAI empowers UK businesses in high-growth sectors, driving productivity and economic growth through the adoption of Artificial Intelligence. We bridge the gap between developers and end-users, fostering user-driven AI technologies.  

With a focus on ethics, transparency, and data privacy, we aim to build trust and confidence in the development of AI solutions. Strengthening AI leadership, supporting workforces, and promoting responsible innovation, BridgeAI shapes a collaborative and AI-enabled future.  

BridgeAI is an Innovate UK funded programme, delivered by a consortium including Innovate UK, Digital Catapult, The Alan Turing Institute, STFC Hartree Centre and BSI.

This repository contains the Jupyter Notebook that was used to demonstrate chunking and evaluation concepts in the Advanced LLM Capabilities webinar.

## Installation

Clone the repository to a suitable location on your computer using the following command:
```
git clone https://github.com/digicatapult/llm-webinar-notebook.git
```

## Pre-requisites

To run the Jupyter Notebook: _llm-3-nb.ipynb_ you must have the following installed:
- Python 3.11+ (tested on Python 3.13)
- pip
- (Optional) Virtual Environment: Conda, Poetry, venv

Install dependencies to your environment. Here is an example with venv:

Create the venv:
```
python3 -m venv venv
```

Activate the venv:
```
source venv/bin/activate
```

Install dependencies:
```
pip install -r requirements.txt
```

Register the venv as a Jupyter kernel:
```
python -m ipykernel install --user --name=llm-3-venv --display-name "llm-3-venv"
```

When you open the _llm-3-nb.ipynb_ Jupyter notebook, you should be able to select the _llm-3-venv_ kernel option. If you are having trouble finding the kernel option on VS Code, try restarting the application. 

You must also have an OpenAI API key (if you would like to run the Semantic Chunking code) which you can create after signing up at: https://platform.openai.com/ . Following this, create a `.env` file in the project root:
```
touch .env
```
Add your OpenAI API key to the `.env` file:
```
OPENAI_API_KEY=your_api_key
```

## License

This project is licensed under the Apache-2.0 License. See the LICENSE file for details.