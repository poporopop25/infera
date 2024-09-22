# Infera Node
Infera is building a decentralized network for LLM inference allowing developers API access to dozens of open source and custom fine tuned models.
#Run node:
```curl -fsSL https://ollama.com/install.sh | sh```
```curl -O https://www.infera.org/scripts/install_script_linux.sh
chmod +x install_script_linux.sh
./install_script_linux.sh```

```grep 'alias init-infera' ~/.bashrc
source ~/.bashrc
~/infera```

```mkdir ~/infera-docker
cd ~/infera-docker
cp ~/infera ./
nano Dockerfile```
