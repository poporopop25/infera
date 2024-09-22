# Infera Node
Infera is building a decentralized network for LLM inference allowing developers API access to dozens of open source and custom fine tuned models.

![ALT TEXT](https://github.com/poporopop25/infera/blob/main/INFERA2.jpg)
# Run node:
Install Ollama
```
curl -fsSL https://ollama.com/install.sh | sh
```
```
curl -O https://www.infera.org/scripts/install_script_linux.sh
chmod +x install_script_linux.sh
./install_script_linux.sh
```

```
grep 'alias init-infera' ~/.bashrc
source ~/.bashrc
~/infera
```

```
mkdir ~/infera-docker
cd ~/infera-docker
cp ~/infera ./
```
Paste in Dockerfile
```
nano Dockerfile
```
```
FROM ubuntu:latest

RUN apt-get update && apt-get install -y curl

COPY infera /app/infera
RUN chmod +x /app/infera

WORKDIR /app

CMD ["./infera"]
```
Control ``X+Y+Enter`` to save the file

```
sudo docker build -t infera-app .
```
```
sudo docker run -it --network host infera-app
```
```
sudo docker run -d --network host infera-app
```
```
install the llama3:latest model
curl -X POST http://localhost:11025/install_new_model \
        -H "Content-Type: application/json" \
        -d '{"install_model_name": "llama3:latest"}'
```
Access SSH

Replace ``your_vps_ip`` the IP of your VPS
```
ssh -L 11025:localhost:11025 root@your_vps_ip
```

# Download the extension - INFERA LIGHT
![ALT TEXT](https://github.com/poporopop25/infera/blob/main/INFERA%20NODE.jpg)

*Run node for 6hours and be active on discord to get Pre-Alpha OG role

*Send the screenshot of infera light to their discord under OG role channel

Join: https://discord.gg/RFc7nK7z

Join my telegram if you have question: https://t.me/airdropPH2024room
