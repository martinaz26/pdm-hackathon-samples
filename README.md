# Politecnico Di Milano Hackathon samples

## Setup

Create a file `.env` and write the following env variables:

```
AZURE_OPENAI_ENDPOINT=https://<REPLACE_ME>/api/v1
AZURE_OPENAI_API_KEY=<REPLACE_ME>
OPENAI_API_VERSION=<REPLACE_ME>
```

**Note**: The way to access those credentials will be sent through private communication.

## Available samples

This repository contains the following samples

| Sample  | Explanation |
| ------------- | ------------- |
| [dalle3.py](./dalle3.py)  | Generate an image using Azure OpenAI DALL-E 3 |
| [gpt.py](./gpt.py) | Generate text using a Azure OpenAI GPT model |
| [embeddings.py](./embeddings.py) | Generate embeddings using an Azure OpenAI embedding model |

## Available models

| Model name  | Type | Sample |
| ------------- | ------------- | ------------- |
| Dalle3  | OpenAI Dalle3 | [dalle3.py](./dalle3.py)  |
| gpt-35-turbo  | OpenAI Chat | [gpt.py](./gpt.py) |
| gpt-4-turbo  | OpenAI Chat | [gpt.py](./gpt.py) |
| gpt-4-vision  | OpenAI Chat | [gpt.py](./gpt.py) |
| text-embedding-ada-002  | OpenAI Embedding | [embeddings.py](./embeddings.py) |


## Info about the code

Each sample reads Azure OpenAI connection information from environment variables stored in the `.env` file using the following snippet of code:

```
from dotenv import load_dotenv

load_dotenv()  # take environment variables from .env.
```
