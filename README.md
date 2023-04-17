# Chatbot-PyTorch-NLP

## Installation

### Create an environment
Create a new environment with a specified name (e.g., "myenv") and the Python version you want to use:
```console
conda create --name myenv python=3.8
```

### Activate it
Activate the environment:
```console
conda activate myenv
```

### Install PyTorch and dependencies

For Installation of PyTorch see [official website](https://pytorch.org/).

You also need `nltk`:
 ```console
pip install nltk
 ```

If you get an error during the first run, you also need to install `nltk.tokenize.punkt`:
Run this once in your terminal:
 ```console
$ python
>>> import nltk
>>> nltk.download('punkt')
```

## Usage
Every time you change [intents.json](intents.json) & after cloning the repository for the first time, train your model:
```console
python train.py
```
This will dump `data.pth` file. And then run
```console
python chat.py
```

## References
Project was inspired from the **Medium article**:
"*Contextual Chatbots with Tensorflow*": 
https://chatbotsmagazine.com/contextual-chat-bots-with-tensorflow-4391749d0077

Huge thanks to **Patrick Loeber** for providing an incredible tutorial:
https://youtu.be/RpWeNzfSUHw
