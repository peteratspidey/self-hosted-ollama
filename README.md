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
##
