# azure-ai-copilot
Custom Copilot with Azure AI Foundry Service | Udacity project

This is a report to show information about developing copilot to support customer by asnwering questions related to product.

The copilot is implemented on Azure AI Foundry using Prompt Flow.

![overview](https://github.com/user-attachments/assets/cd94fe99-ed1c-4ecf-9bee-d592b2fd2a7d)


## Project Data Configuration and Preparation

#### AI model is deployed within the project
GPT-4o-mini is deployed to use as a base model.
text-embedding-ada-002 is used as an embedding.

![image](https://github.com/user-attachments/assets/34b19015-c6e1-4af3-954d-50a5ead384db)


#### Upload and management of data in AI Studio

Example of response from Copilot (Prompt Flow). Three outputs are from three different prompts.

Prompt 1
```
You are an AI assistant that helps users answer questions given a specific context. You will be given a context and asked a question based on that context. Your answer should be as precise as possible and should only come from the context.
Please add citation after each sentence when possible in a form "(Source: citation)".
```

Prompt 2
```
You are an AI assistant that helps users answer questions about products. 
You will be given a context and asked a question based on that context. 
Your answer should be as precise as possible and should only come from the context.
Please add citation after each sentence when possible in a form "(Source: citation)".
```

Prompt 3
```
You are an AI assistant for helping users answering question related to products.
You are given a context and you'll be asked a question based on the context.
Your answer should be as precise as possible and answer should be only from the context.
If you cannot find the answer, say that "I cannot find information from the database".
```

![image](https://github.com/user-attachments/assets/11934c2b-5454-4b2b-b521-c69f034bb6cb)


#### AI Search index using the uploaded data
The original data is tranformed into vectoring data. In Prompt Flow, `lookup` function searches relevant information from vetoring (indexing) data.

![image](https://github.com/user-attachments/assets/2ad149a9-4c22-4c1c-aa5f-10ba9e345bde)


## Copilot App Development


## Evaluation of the Copilot


## Deployment
