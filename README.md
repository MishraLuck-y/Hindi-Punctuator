# Hindi-Language-Punctuator
Designing punctuator is the process of adding punctuation marks in the plain sentences to make it appropriate one. With correct punctuation, the reader understands your tone and inflection. It Give meaning to the words you write and express your thoughts, questions, statements, and feelings in an organized way. The punctuator for Hindi language, which when given a Hindi text as input, will add punctuation marks at the appropriate positions and display the punctuated text as output. 

## Methodology
The model used for this project is a pre-trained model that is provided as  oliverguhr/full stop-punctuation-multilang-large (Owner: Oliver Guhr).
This model majorly predicts the punctuation of English, Italian, French and German texts. Some of the changes were done in the model to predict the punctuation in Hindi Language as well.

## Requirements
* Python 3.5+
* Transformers
* SentencePiece\
* Pipeline
* Spacy

## Contents
* Pre-trained model: The model used for this project is a pre-trained model that is provided as  oliverguhr/full stop-punctuation-multilang-large (Owner: Oliver Guhr).
* Notebooks: Jupyter Notebook for using pre-trained model and performing addition of punctuation in sentences/paragraph.

## Installation and Import
```
!pip install sentencepiece
!pip install transformers
from transformers import AutoTokenizer, AutoModelForTokenClassification, pipeline
from spacy import displacy
from IPython.core.display import display, HTML
```

## Usage
* Install Dependencies and Requirments
* Import Libraries
* Download pre-trained model
* Define the model, pass the path of pre-trained model in the argument of the model
* Define pipeline with parameter as 'pun'
* Run the model with text as a parameter
* Extract the word and replace '_' with ' '(i.e, replace underscore with space)
* Print the output with appended punctuation at the suitable place

> :warning: **Note: Use of spacy is optional it is just used for visualization of punctuations after a word.**
