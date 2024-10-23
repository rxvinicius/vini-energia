<div align='center'>
  <img style="width:300px;" src='./frontend/public/images/project-logo.png'/>
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

Siga as instruções abaixo:

1. Clone esse repositório e os submódulos e acesso a raiz do projeto:

```
git clone --recurse-submodules https://github.com/rxvinicius/vini-energia.git && cd vini-energia
```

> ⚠️ IMPORTANTE: Se você já clonou o repositório sem os submódulos, você pode inicializá-los e atualizá-los usando os seguintes comandos:

```
git submodule init
git submodule update
```

2. Construa e inicie os serviços:

```
docker-compose up --build
```

3. Acesse a aplicação:

- Frontend: http://localhost:8080
- Backend: http://localhost:3000

## 💻 Executar a aplicação no ambiente de desenvolvimento

O passo a passo para rodar o frontend e o backend localmente estão em seus respectivos repositórios:

- [Frontend](https://github.com/rxvinicius/vini-energia-frontend)
- [Backend](https://github.com/rxvinicius/vini-energia-backend)
