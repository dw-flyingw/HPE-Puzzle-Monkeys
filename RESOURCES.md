### HPE AI Training Modules https://github.com/frontier-tops/

### N8N Starter Kit https://github.com/n8n-io/self-hosted-ai-starter-kit
```bash
git clone https://github.com/n8n-io/self-hosted-ai-starter-kit.git
cd self-hosted-ai-starter-kit
cp .env.example .env # you should update secrets and passwords inside
docker compose --profile gpu-nvidia up

# Reset Admin on Self Hosted
docker exec -it n8n n8n user-management:reset
docker restart n8n
```
