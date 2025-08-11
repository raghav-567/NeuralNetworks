# CodeGenerator

A Python code generator model fine-tuned from the Salesforce T5-small model using the Hugging Face BigCode Stack Python dataset.

## Overview

This project leverages transfer learning by fine-tuning the [Salesforce T5-small](https://huggingface.co/Salesforce/codet5-small) model on the [BigCode Stack Python dataset](https://huggingface.co/datasets/bigcode/the-stack) to generate Python code from natural language prompts.

## Features

- Generates Python code from text prompt
- Built on top of the T5-small transformer architecture
- Fine-tuned for Python syntax and idioms


## Usage

```python
from code_generator import generate_code

prompt = "Write a Python function to compute factorial"
code = generate_code(prompt)
print(code)
```

## Model Details

- **Base Model:** Salesforce/codet5-small
- **Dataset:** BigCode Stack Python
- **Framework:** Hugging Face Transformers

## Training

The model was fine-tuned using the Hugging Face Trainer API. See `python-code-generator.ipynb` for details.


## Acknowledgements

- [Salesforce CodeT5](https://github.com/salesforce/CodeT5)
- [Hugging Face Datasets](https://huggingface.co/datasets)
- [BigCode Project](https://bigcode-project.github.io/)
