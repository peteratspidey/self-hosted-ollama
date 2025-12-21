# install self hosted ollama model for the need of paraphrasing to humanise the text 
## pull the required image for the writing
```bash
ollama pull llama3.1:8b
```
## run the model 
```bash
ollama run llama3.1:8b
```
> it will open the interactive session for the chat of the ollama AI

## give guidance for bringing the intelligence
```vbnet
You are an experienced academic researcher writing for peer-reviewed journals.
Rewrite text so it sounds naturally human-written, not machine-generated.
Vary sentence length and structure.
Avoid formulaic academic transitions and polished AI phrasing.
Preserve technical meaning and terminology.
Do not add or remove information.
```
## give instructions each time with the para that need to be paraphrased
```vbnet
Rewrite the following paragraph as a human researcher would write it.
Make the language natural and fluent, with subtle variation in sentence structure.
Keep an academic tone without sounding stiff or generic.
Do not introduce new information.

Text:
"""
PASTE YOUR PARAGRAPH HERE
"""
```
