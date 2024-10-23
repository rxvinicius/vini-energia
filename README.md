<div align='center'>
  <img style="width:300px;" src='https://github.com/rxvinicius/vini-energia-frontend/blob/2d903a3c91e6738defc6895d56b04445a24b2210/public/images/project-logo.png'/>
</div>

# Vini Energia

Este repositório contém o projeto full stack, incluindo o frontend e o backend, ambos organizados como submódulos Git. Ele também inclui arquivos de configuração para facilitar o setup do ambiente usando Docker.

## 🌐 Links dos Ambientes e Repositórios

### Produção

- **🖥️ [Frontend](https://vini-energia-frontend.vercel.app)**
- **🛠️ [Backend](https://vini-energia-backend-production.up.railway.app)**

### Repositórios no GitHub

- **📂 [GitHub - Frontend Repo](https://github.com/rxvinicius/vini-energia-frontend)**
- **📂 [GitHub - Backend Repo](https://github.com/rxvinicius/vini-energia-backend)**

## 🐳 Passo a passo para rodar a aplicação com Docker Compose

Para rodar a aplicação utilizando o Docker Compose, siga as instruções abaixo:

### 1. Clone esse repositório e os submódulos e acesso a raiz do projeto:

```bash
git clone --recurse-submodules https://github.com/rxvinicius/vini-energia.git && cd vini-energia
```

> ⚠️ **IMPORTANTE:** Se você já clonou o repositório sem os submódulos, você pode inicializá-los e atualizá-los usando os seguintes comandos:

```bash
git submodule init
git submodule update
```

### 2. Construa e inicie os serviços:

```bash
docker-compose up --build
```

### 3. Acesse a aplicação:

- **Frontend:** http://localhost:8080
- **Backend:** http://localhost:3000

### Executando o Docker Compose no Ambiente Local (opcional)

Para rodar a aplicação utilizando o Docker Compose no ambiente local, você precisará ajustar o arquivo `docker-compose.yml` para usar as variáveis de ambiente corretas. Siga as instruções abaixo:

1. **Abra o arquivo `docker-compose.yml`.**

2. **Localize a seção do serviço `backend`.**

3. **Modifique a linha `env_file` para referenciar o arquivo `.env.development`.** A alteração deve ficar assim:

```yaml
  backend:
    ...
    env_file:
      - ./backend/.env.docker
    ...
```

> **🗂️ Configuração dos Arquivos `.env`** <br>
> Para mais detalhes sobre como configurar os arquivos `.env`, acesse a [documentação dos arquivos `.env`](https://github.com/rxvinicius/vini-energia-backend?tab=readme-ov-file#configura%C3%A7%C3%A3o-do-ambiente) no repositório do backend

## 💻 Executar a aplicação no ambiente de desenvolvimento

O passo a passo para rodar o frontend e o backend localmente estão em seus respectivos repositórios:

- **[📂 Backend](https://github.com/rxvinicius/vini-energia-backend)**
- **[📂 Frontend](https://github.com/rxvinicius/vini-energia-frontend)**
