### N8N Starter Kit https://github.com/n8n-io/self-hosted-ai-starter-kit
```bash
git clone https://github.com/n8n-io/self-hosted-ai-starter-kit.git
cd self-hosted-ai-starter-kit
cp .env.example .env # you should update secrets and passwords inside
docker compose --profile gpu-nvidia up
```
```bash
# Reset Admin on Self Hosted
docker exec -it n8n n8n user-management:reset
docker restart n8n
```
```bash
# Upgrading
docker compose --profile gpu-nvidia pull
docker compose create && docker compose --profile gpu-nvidia up
```

### Owner Account
- email = puzzlemonkey@hpe.com
- name = Puzzle Monkey
- passwd = 1PuzzleMonkey
