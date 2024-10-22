
# Welcome!
this is a `meta-llama/Llama-2-7b-chat-hf` LLM implementation. The aim of this project is to provide an example of how modular LLM prompting functions can accomodate single or batch inference. This project also has a testing functionality (limited to sentiment analysis at the moment). This project is best suited to be used on [Google Colab](https://colab.research.google.com/drive/1Y7GzRFtxOCkfFyHoWOljdKRlvQnlA1_K?usp=sharing)

This repository also serves as the tutorial on using this notebook.

## Start & Login
click `Runtime` --> `Run All`, then click `Start`, then login with your HuggingFace token.

!['start'](https://github.com/user-attachments/assets/555ec5ca-f41b-439b-9ec3-8ff06bc9b1df)

![login](https://github.com/user-attachments/assets/a54a47a9-eeed-4581-8fa2-cb44575b5dcb)


## Load Model
input the desired model and click `Load Model`. When loading done, it should look as follows.

![image](https://github.com/user-attachments/assets/e978a61d-b89c-4efb-bd89-a6364d78fa84)

![image](https://github.com/user-attachments/assets/a01dd425-16f5-4248-ab9b-0f7981531be0)


## Prompt
Insert and load your prompt. Make sure to add `{text}` so the model can insert your text to the prompt. If not, the following error occurs when `Load Prompt` is clicked.

![image](https://github.com/user-attachments/assets/ad63670b-65fb-45b0-bedd-2a18a172610a)

![image](https://github.com/user-attachments/assets/900eed52-5963-47fd-a927-283f1be869de)


## Infer!
Insert your desired text to fill the `{text}` field mentioned before and click `Infer`.

![image](https://github.com/user-attachments/assets/c166781c-6c72-4900-b8d3-9500dda4ab4b)

![image](https://github.com/user-attachments/assets/745a7f5b-e2c7-42de-bd8c-1d21283f1890)

another example:

![image](https://github.com/user-attachments/assets/0fd8b305-eec1-48c2-9549-0b0c45d8a54f)

![image](https://github.com/user-attachments/assets/8878d42b-38b4-4fd0-84f3-260b024cebe1)


## Multiple Inference?
If you wish to infer multiple input text on the same prompt, do as the following for batch inferring. Input and laod the prompt as in previous inference.
![image](https://github.com/user-attachments/assets/a230ec45-32b4-4109-8581-eb23d8208f58)

## Upload Data
This time, we instead upload our data to the `files` tab of the Google Colab then input the file name or you can input a link that directly refers to a `.tsv`/`.csv` dataset. After that, click `Load File`.

![image](https://github.com/user-attachments/assets/821710e6-ff96-47c4-8a18-50387b499994)


## Batch Infer!!
Click on `Batch Infer`.

![image](https://github.com/user-attachments/assets/21e343f2-1c54-4f36-a1a2-48ce8f1d465c)

## Download :D
If you wish to save each prompt + text and its result, input your desired file name for the result `.csv` file and click `Download Predictions`. The file should also appear in the `files` tab

![image](https://github.com/user-attachments/assets/0ac08e53-4667-462d-8c7d-0e76c8c1af40)


## Accuracy
I also add testing functionality. Note that the previous images do miss the `Post-Processing` button which at the moment only accomodate regex on responses that contain 'negative', 'positive', or'neutral' words for sentiment analysis. This button should be clicked right after `Batch Infer` is done. After that, click on `Test`.

![image](https://github.com/user-attachments/assets/0f67f318-d6db-42d9-97d3-160458ba5ee0)

$Naufal \cdot Zafran \cdot Fadil —$ ```Ilmu Komputer 2024```
