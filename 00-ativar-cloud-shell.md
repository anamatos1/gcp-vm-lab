# Ativar Cloud Shell

Abra o console do Google Cloud e ative o Cloud Shell clicando no ícone no canto superior direito.

Ao conectar, o projeto será autenticado automaticamente. Para verificar o `Project ID`:

```bash
gcloud config list project


Para listar a conta ativa:
gcloud auth list

Saída esperada:
ATIVO: *
CONTA: "CONTA"


Para  definir a conta ativa, execute:
    $ gcloud config definir conta `CONTA`


(Opcional) Você pode listar o ID do projeto com este comando:
gcloud config list project

Saída:

[core] 
projeto = "ID_DO_PROJETO"

---

#### `01-definir-regiao-zona.md`

```markdown
# Definir Região e Zona

As regiões e zonas determinam a localização física dos recursos. Para definir no projeto:

```bash
gcloud config set compute/region us-central1
gcloud config set compute/zone us-central1-c

export REGION=us-central1
export ZONE=us-central1-c

---

#### `02-criar-instancia-console.md`

```markdown
# Tarefa 1 - Criar Instância no Console do Cloud

Acesse: **Compute Engine > Instâncias de VM > Criar instância**

### Configurações usadas:

- **Nome**: gcelab
- **Região**: us-central1
- **Zona**: us-central1-c
- **Série**: E2
- **Tipo de máquina**: e2-medium
- **Sistema operacional**: Debian GNU/Linux 11
- **Tamanho disco**: 10 GB
- **Firewall**: Permitir tráfego HTTP

Depois, clique em **Criar** e conecte-se via SSH.
