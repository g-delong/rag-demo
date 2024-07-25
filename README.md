
# Proof of Concept: RAG Implementation

This repository demonstrates a simple Retrieval-Augmented Generation (RAG) implementation using Conda for the virtual environment, pip for package management, and the `transformers` and `langchain` libraries for tooling. It utilizes a small FLAN-T5 LLM model and a LLaMA2 7B chat LLM model deployed via Amazon SageMaker Jumpstart.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)

## Installation

### Prerequisites
- [Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html)
- [AWS CLI](https://aws.amazon.com/cli/) (this is provided out of the box in a Sagemaker Notebook)

### Steps
1. Clone the repository:
    ```bash
    git clone https://github.com/g-delong/rag-demo.git
    cd rag-demo
    ```

2. Create and activate the Conda environment:
    ```bash
    conda create --name rag-env python=3.10
    conda activate rag-env
    ```

3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage


### Running the RAG Notebook
1. Select your `rag-env` virtual environment as the kernel for the Jupyter notebook.

2. I prepared several documents from a few random open source documentation websites for this example, but any documents can be added or substituted for your use case.

3. This demo does not cover deploying LLM models through Sagemaker Jumpstart. Refer to [Sagemaker Jumpstart Foundation Models Documentation](https://docs.aws.amazon.com/sagemaker/latest/dg/jumpstart-foundation-models-use-studio-updated.html) for deploying Llama2 or other foundation models. When you have an endpoint name for your deployed model, update the `endpoint_name` variable in order to run the last few cells in the notebook.


## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
