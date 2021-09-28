## chaii-hindi-and-tamil-question-answering
This project is a part of Kaggle's Google challenge for AI for India ([chaii](https://www.kaggle.com/c/chaii-hindi-and-tamil-question-answering)). 

In the Kaggle competition, we will be predicting the answers to questions in Hindi and Tamil. The answers are drawn directly (see the Evaluation page for details) from a limited context. We have provided a small number of samples to check your code with. 

The way to go about solving the challenge according to us is using sequence to sequence models which using RNN to capture the time series nature of the natural language. Adding to it, we have used attension, particularly Bahdanau and Luong attension architectures to address the problem statement for attension. 

We have build seperate models for each Hindi and Tamil, where the input to the model is question sentence as embeddi ng and the target is the answer in that respective language.

## Packages used for setup:

System Reqirements:
* Python3 (spacy, numpy, torch, matplotlib, pandas, tqdm)
* Linux machine with atleast 4 cores and 4GB Ram.

Here are the steps for test the model on the given sentence in Hindi or Tamil written in the format in the same way as that of test.csv file:

1) Clone the repository from https://github.com/mltechsachin/chaii using

  ```
   git clone https://github.com/mltechsachin/chaii
  ```
2) After installing the dependencies run the below, for decoding the answer for question in a test file, say sample.csv
  ```
   python test.py sample.csv
  ```
 ## References
 [1] Luong, Bahdanau attention: https://blog.floydhub.com/attention-mechanism/
