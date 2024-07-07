# evaluating-chatbots

This repo contains a collection of Jupyter notebooks that can be used to evaluate AI Chatbots powered by Large Language Models. 

## Usage

Download the notebook files (.ipynb) and upload them to your Google Drive. You can then open them in Google Colab.

### Llm_evals_test_data_response_generation.ipynb

Use this notebook to generate an excel sheet with responses from your Voiceflow Chatbot provided you have an excel sheet containing questions and ideal answers. The output of this notebook can be used to perform evaluations.

The code in the notebook does the following:

1. Reads questions from an Excel file: It reads questions from an Excel file (llm_evals_test_data_with_context.xlsx) and stores them in a list.
2. Launches a Voiceflow session: It starts a new session with a Voiceflow chatbot using an API key.
3. Gets answers from Voiceflow: It sends each question to the Voiceflow chatbot and receives the corresponding answers.
4. Adds answers to the list: It appends the received answers to the list of questions.
5. Generates an Excel file: It creates a new Excel file (llm_evals_test_data_with_response.xlsx) and writes the questions and answers into it.

### Llm_evals_response_evaluations.ipynb

Use this notebook to evaluate the responses of your chatbot and save the results in an Excel file named 'llm_eval_results.xlsx'. The responses are scored on factual accuracy and relevance with the help of an open source library called [Uptrain](https://github.com/uptrain-ai/uptrain).