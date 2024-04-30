## Install Docker + WSL + Ubuntu + Nvidia on Win11
[link](https://blog.csdn.net/godblesstao/article/details/135893429)
1. Install Docker Desktop
2. Install WSL2 (Ubuntu22.04)
3. Update Win11 Nvidia driver and cuda>=12.0 via Nvidia GeForce Experience
4. MobaXterm with session Ubuntu22.04
5. Install Docker in Ubuntu22.04
6. Install Nvidia Container Toolkit

## Both run in docker!
### [Ollama](https://ollama.com/)
```
sudo docker run -d --gpus=all -v ollama:/root/.ollama -p 11434:11434 --name ollama ollama/ollama
sudo docker exec -it ollama ollama run llama3
```
### [OpenWebUI](https://github.com/open-webui/open-webui)
```
sudo docker run -d -p 3000:8080 --add-host=host.docker.internal:host-gateway -v open-webui:/app/backend/data --name open-webui --restart always ghcr.io/open-webui/open-webui:main
http://localhost:3000
```

## [Llama3](https://github.com/meta-llama/llama3)
```
torchrun --nproc_per_node 1 example_chat_completion.py \
    --ckpt_dir Meta-Llama-3-8B-Instruct/ \
    --tokenizer_path Meta-Llama-3-8B-Instruct/tokenizer.model \
    --max_seq_len 512 --max_batch_size 6
```