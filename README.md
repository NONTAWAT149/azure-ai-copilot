# Copilot with Azure AI Foundry (Implementation of PromptFlow)
Custom Copilot with Azure AI Foundry Service | Udacity project

This is a report to show information about developing copilot to support customer by asnwering questions related to product.

The copilot is implemented on Azure AI Foundry using Prompt Flow.

![overview](https://github.com/user-attachments/assets/cd94fe99-ed1c-4ecf-9bee-d592b2fd2a7d)


## 1. Project Data Configuration and Preparation

### 1.1 AI model is deployed within the project
GPT-4o-mini is deployed to use as a base model.
text-embedding-ada-002 is used as an embedding.

![image](https://github.com/user-attachments/assets/34b19015-c6e1-4af3-954d-50a5ead384db)


### 1.2 Upload and management of data in AI Studio

<ins>Prompt Management</ins>

Prompt 1 (variant_0)
```
You are an AI assistant that helps users answer questions given a specific context. You will be given a context and asked a question based on that context. Your answer should be as precise as possible and should only come from the context.
Please add citation after each sentence when possible in a form "(Source: citation)".
```

Prompt 2 (variant_1)
```
You are an AI assistant that helps users answer questions about products. 
You will be given a context and asked a question based on that context. 
Your answer should be as precise as possible and should only come from the context.
Please add citation after each sentence when possible in a form "(Source: citation)".
```

Prompt 3 (variant_2)
```
You are an AI assistant for helping users answering question related to products.
You are given a context and you'll be asked a question based on the context.
Your answer should be as precise as possible and answer should be only from the context.
If you cannot find the answer, say that "I cannot find information from the database".
```

<ins>Grounded data</ins>
![image](https://github.com/user-attachments/assets/4329448f-5a9c-4260-bf33-54255aa7a6c8)

### 1.3 AI Search index using the uploaded data
The original data is tranformed into vectoring data. In Prompt Flow, `lookup` function searches relevant information from vetoring (indexing) data.

![image](https://github.com/user-attachments/assets/2ad149a9-4c22-4c1c-aa5f-10ba9e345bde)


## 2. Copilot App Development

### 2.1 Implementation of Prompt Flow for the custom AI Copilot
![image](https://github.com/user-attachments/assets/c04dafee-aaed-488d-9f11-0d2275c2cd4c)


### 2.2 The Copilot is tested with relevant questions.
Examples of response from Copilot (Prompt Flow). Three outputs are from three different prompts.

![image](https://github.com/user-attachments/assets/11934c2b-5454-4b2b-b521-c69f034bb6cb)

![Test_result_02](https://github.com/user-attachments/assets/31aa3ab3-d5ad-40b4-bad9-ba940813fc5a)

![Test_result_03](https://github.com/user-attachments/assets/88d7a7ed-ca22-46fb-9b84-ae8d82809881)


## 3. Evaluation of the Copilot

### 3.1 The automated evaluation of the copilot is performed with a structured dataset

<ins>Evaluation of Prompt 1</ins>
![image](https://github.com/user-attachments/assets/44f5e93a-677b-49b2-b40c-d89d1812adf8)

<ins>Evaluation of Prompt 2</ins>
![image](https://github.com/user-attachments/assets/17a8f3fc-4e5d-4852-880f-a94925a2f3e3)

<ins>Evaluation of Prompt 3</ins>
![image](https://github.com/user-attachments/assets/ce1bcfc7-119f-4a31-9cf9-7d6d68547751)


### 3.2 Manual prompt evaluation is conducted



## 4. Deployment
![image](https://github.com/user-attachments/assets/0c852ceb-e85b-4c74-bd85-9799b73ae791)

