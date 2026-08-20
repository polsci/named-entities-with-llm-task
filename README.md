# Extract named entities with an LLM (lab task notebook)  

Geoff Ford  
[https://geoffford.nz](https://geoffford.nz/)  
![GitHub Release](https://img.shields.io/github/v/release/polsci/named-entities-with-llm-task) 

The notebook in this repository is provided for students in DIGI405 at the University of Canterbury for a lab task that involves writing a query to use a Large Language Model (LLM) to extract named entities from arbitrary texts. Students find this task interesting to understand system and user prompts, and zero-shot, one-shot, few-shot paradigms for prompting.

A smaller model is used to make the task more challenging and demonstrate the sensitivity of LLM output to prompt wording. During our first run of this lab task, students found it interesting to see that even with identical prompting, settings and input text, LLMs often return different results. In addition, even the formatting of the JSON is a point of failure. 

I appreciate this notebook may be relevant for others. If you use it please retain the authorship information and links.  

Changes are documented in the [CHANGELOG](changelog.md).

## Note on previous OpenRouter / Cerebras support 

Note: that version 1.0.0 of this repository used the OpenRouter API. Up to version 1.0.2 the notebook uses Cerebras.  

## Note on LLM Providers

Check [Free-LLM — Open Directory of Free AI & LLM APIs](https://github.com/nejib1/Free-LLM) for a repository of free LLM providers. Access to free LLM APIs is changeable. The requirement to run the notebook is an LLM API that is Open-AI compatible via the completions endpoint. The API endpoints for the free providers are listed in [the Free LLM repository](https://github.com/nejib1/Free-LLM). An endpoint base URL and api key can be configured in the notebook. 

API providers require completing a sign-up process. Look for a provider that does not require a credit card for sign-up. 

NOTE: If you are a DIGI405 student, in 2026 we are making use of Mistral AI. If you have problems getting this working, look for an provider that does not require credit card registration and the process should be similar. 

## Create a Mistral API Key

Go to [Mistral](https://console.mistral.ai/) and complete the sign-up process. For students in DIGI405, you can signup with your UC email address. Once sign-up is complete you may be prompted to create an API key. If you are not prompted for this, click the link to "Create an API key". Copy and paste the key into your password manager for future use. There is a field in the notebook where you need to paste in your key. Don't share your key with anyone else. 

## Instructions for DIGI405 students - warning about excessive, rapid or repeated requests during lab times

This is the first semester we are using the Mistral AI service in DIGI405. All LLM providers have rate limits. Avoid making excessive, rapid or repeated requests during the lab times as there is the potential this could cause our network to be flagged as malicious and create problems for your classmates accessing the API.  

## Installation  

If you are a DIGI405 student running this on our JupyterHub instance, most required libraries are pre-installed. The notebook has a cell to run to install a new library for labs in 2026. If you want to install this on your own computer, there is a requirements.txt file with required libraries. To install the required libraries run:  

```
    pip install -r requirements.txt
```
