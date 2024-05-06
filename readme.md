
# **LLM Project to Build and Fine Tune a Large Language Model**


## Project Overview

In today's data-driven world, the ability to process and generate natural language text at scale has become a transformative force across industries. Large Language Models (LLMs) represent a cutting-edge advancement in natural language processing, enabling businesses to extract valuable insights, automate tasks, and enhance user experiences. By harnessing the power of LLMs, organizations can improve customer service, automate content creation, and gain a competitive edge in the digital landscape.

This project builds the foundation for Large Language Models by diving deep into the details of their inner workings. It shows how to optimize their use through prompt engineering and fine-tuning techniques such as LoRA. Prompt engineering involves crafting specific instructions or queries given to the language model to influence its output, guiding LLMs in generating desired responses through zero-shot, one-shot, and few-shot inferences. Fine-tuning entails training a pre-trained language model on a specific task or dataset to adapt it for a particular application. It explores full fine-tuning and Parameter Efficient Fine Tuning (PEFT), a technique that optimizes the fine-tuning process by focusing on a subset of the model's parameters, making it more resource-efficient.

The project also involves the application of Retrieval Augmented Generation (RAG) using OpenAI's GPT-3.5 Turbo, resulting in the development of a chatbot for online shopping. Knowledge grounding with Retrieval Augmented Generation (RAG) is implemented to mitigate hallucinations and provide trustworthy and reliable responses by incorporating information from external sources to validate and support the generated text.

## Aim

The aim of this project is to provide a comprehensive understanding and practical experience in working with Large Language Models (LLMs). It covers fundamental concepts, advanced techniques, and practical applications of LLMs, to effectively leverage them for tasks such as text generation, fine-tuning, and building knowledge-grounded applications like a chatbot for online shopping.

## Data Description

- The dialogue summarization exercises in this project utilize the knkarthick/dialogsum dataset from the Hugging Face library.
- For the purpose of demonstrating the development of a chatbot, data about apparel and paper products is provided. This dataset includes textual information about various apparel items and paper products.

## Tech Stack

- **Language:** Python 3.8
- **Libraries:** transformers, datasets, torchdata, torch, streamlit, openai, langchain, unstructured, sentence-transformers, chromadb, evaluate, rouge_score, loralib, peft

## Approach

- **Introduction to LLMs and Basics:** Explanation of RNNs, transformers, attention mechanism, and Large Language Models (LLMs). Illustration of use cases, including text generation, to establish foundational knowledge.
- **Prompt Engineering:** Introduction to prompt engineering techniques, including zero, one, and few-shot inferences.
- **Dialogue Summarization Task:** Implementation of prompt engineering on a dialogue summarization task, showcasing practical application.
- **Fine Tuning and PEFT:** Implementing full fine-tuning and parameter-efficient fine-tuning (PEFT) on dialogue summarization. Model evaluation using ROUGE metrics for performance assessment.
- **RLHF (Reinforcement Learning from Human Feedback):** Explanation and exploration of the RLHF concept.
- **Retrieval Augmented Generation (RAG):** Practical implementation of RAG using OpenAI's GPT3.5 for creating a chatbot.
- **Development of Chatbot Application:** Step-by-step guide on building a functional chatbot application for online shopping using RAG.

## Modular code overview

Once you unzip the `code.zip` file, you can find the following files/folders:

1. `full`: Contains files related to full fine-tuning of the language model.
2. `images`: Stores images used for demonstration or visualization purposes within the project.
3. `kb`: Contains two text files, `apparel_products.txt` and `paper_products.txt`, serving as knowledge bases for the chatbot.
4. `llm_app.py`: Streamlit application for interacting with the chatbot. Users need to enter their OpenAI API key in this application.
5. `llm_labs.ipynb`: Jupyter notebook serving as the central hub for all explanatory material and codes related to different use cases.
6. `peft`: Contains files related to the parameter-efficient fine-tuning of the language model.
7. `readme.md`: Provides essential information about the project, including the Python version required to run the code and instructions for execution.
8. `requirements.txt`: Contains a list of all required libraries and their versions needed to run the project.



​
​
​
# Execution Instructions
​
# Python version 3.8.10
​
To create a virtual environment and install requirements in Python 3.8.10 on different operating systems, follow the instructions below:
​
### For Windows:
​
Open the Command Prompt by pressing Win + R, typing "cmd", and pressing Enter.
​

Change the directory to the desired location for your project:
​

`cd C:\path\to\project`

​
Create a new virtual environment using the venv module:

​
`python -m venv myenv`

​
Activate the virtual environment:

​
`myenv\Scripts\activate`

​
Install the project requirements using pip:

​
`pip install -r requirements.txt`


​
​
### For Linux/Mac:
​
Open a terminal.

​
Change the directory to the desired location for your project:
​

`cd /path/to/project`
​

Create a new virtual environment using the venv module:
​

`python3 -m venv myenv`
​

Activate the virtual environment:
​

`source myenv/bin/activate`
​

Install the project requirements using pip:
​

`pip install -r requirements.txt`
​

These instructions assume you have Python 3.8.10 installed and added to your system's PATH variable.
​
​

## Execution Instructions if Multiple Python Versions Installed
​
​
If you have multiple Python versions installed on your system , you can use the Python Launcher to create a virtual environment with Python 3.8.10, you can specify the version using the -p or --python flag. Follow the instructions below:
​

### For Windows:
​

Open the Command Prompt by pressing Win + R, typing "cmd", and pressing Enter.
​

Change the directory to the desired location for your project:
​

`cd C:\path\to\project`
​

Create a new virtual environment using the Python Launcher:
​

`py -3.8 -m venv myenv`
​

Note: Replace myenv with your desired virtual environment name.
​

Activate the virtual environment:
​

`myenv\Scripts\activate`
​

Install the project requirements using pip:
​

`pip install -r requirements.txt`
​

​
For Linux/Mac:

​

Open a terminal.
​

Change the directory to the desired location for your project:

​

`cd /path/to/project`


Create a new virtual environment using the Python Launcher:
​

`python3.8 -m venv myenv`


Note: Replace myenv with your desired virtual environment name.
​

Activate the virtual environment:
​

`source myenv/bin/activate`


Install the project requirements using pip:
​

`pip install -r requirements.txt`
​


​

By specifying the version using py -3.8 or python3.8, you can ensure that the virtual environment is created using Python 3.8.10 specifically, even if you have other Python versions installed.
​
​

Then you can run the notebook or use the command to run the app:

`streamlit run llm_app.py`



```
code
├─ full
├─ images
├─ kb
│  ├─ apparel_products.txt
│  └─ paper_products.txt
├─ llm_app.py
├─ llm_labs.ipynb
├─ peft
├─ readme.md
└─ requirements.txt

```
