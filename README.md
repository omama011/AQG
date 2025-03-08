# AQG
Automatic question generation (QG) is the task of preparing relevant questions from a context 
or a paragraph .It can be used to generate assessment questions to test the learning of a 
particular topic or lesson.We explore the performance of diverse approaches for 
QG utilizing the Stanford Question Answering Dataset (SQuAD) as the benchmark. The 
methodology encompasses transformer architectures for question generation on SQUAD 
dataset. 

## End to end question generation 
This approach focuses on generating multiple questions related to a single context .During 
training the context is provided as an input and a set of related questions separated by <sep> 
token are provided as the target text . The input text and target text are then padded to a uniform 
length sequence. For fine-tuning t5 small is used. It is an encoder-decoder based transformer 
model with 6 encoder and 6 decoder layers. It is pre-trained on C4 dataset. It has 60 million 
parameters due to which it supports faster inference , faster training and flexible for multiple 
NLP applications.
