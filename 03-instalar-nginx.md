# Tarefa 2 - Instalar servidor NGINX

Acesse a VM via SSH e execute os seguintes comandos:

```bash
sudo apt-get update
sudo apt-get install -y nginx

Verifique se o NGINX está rodando:
ps auwx | grep nginx

Acesse via navegador: http://EXTERNAL_IP/

Você deverá ver: Welcome to nginx!

---

#### `04-criar-instancia-gcloud.md`

```markdown
# Tarefa 3 - Criar instância via gcloud CLI

No Cloud Shell:

```bash
gcloud compute instances create gcelab2 \
  --machine-type e2-medium \
  --zone=$ZONE

Para acessar via SSH:

bash
Copy code
gcloud compute ssh gcelab2 --zone=$ZONE

Depois de usar:

bash
Copy code
exit


