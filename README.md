# self-hosted-ollama
setup ai chat module locally and use it without the need of internet and make data security ( use it in terminal)
## updates and upgrades
```bash
sudo apt-get update && sudo apt-get upgrade -y
```
## download the curl package
```bash
curl -fsSL https://ollama.com/install.sh | sh
```

## enable the ollama
```bash
sudo systemctl enable ollama
```
## start the ollama
```bash
sudo systemctl start ollama
```
## check the status of ollama active and running
```bash
sudo systemctl status ollama
```
## if not active then restart
```bash
sudo systemctl restart ollama 
```
## check the version of the installed ollama
```bash
ollama --version
```
> it will give u a warning about the gpu acceleration (means if u have gpu card then it would be better for the ollama )
## select the best model to pull for ur ollama 
* go to this link [link](https://ollama.com/search) and select the model as per ur requirements and the system specification
* `llama3:8db` - for general research/writing/reasoning)
* `qwen2.5-coder:3b` - for coding and pipelines
```bash
ollama pull llama3:8b
```bash
ollama pull qwen2.5-coder:3b
```
## now run only one at a time 
```bash
ollama run llama3:8b
```
or
```bash run qwen2.5-coder:3b
```

##  to quick run make alias for the commmands
### open the bashrc file
```bash
gedit ~/.bashrc
```

## add this line in the end of the file
```bash
alias bio_assist='ollama run llama3:8b
alias code_assist='ollama run qwen2.5-coder:3b
```
## reload config file (bashrc)
```bash
source ~/.bashrc
```
