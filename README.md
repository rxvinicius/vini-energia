# Clarke Energia

Instruções para iniciar os repositórios do desafio técnico da **Clarke Energia**.

## Demo online

👉 [Frontend](https://clarke-energia-frontend.vercel.app) <br>
👉 [Backend](https://clarke-energia-backend-8da448044f10.herokuapp.com)

## Passo a passo para rodar a aplicação com Docker Compose

Siga as instruções abaixo:

1. Clone esse repositório e os submódulos e acesso a raiz do projeto:

```
git clone --recurse-submodules https://github.com/rxvinicius/clarke-energia.git && cd clarke-energia
```

> Se você já clonou o repositório sem os submódulos, você pode inicializá-los e atualizá-los usando os seguintes comandos:

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

## Rodar a aplicação localmente

O passo a passo para rodar o frontend e o backend localmente estão em seus respectivos repositórios:

- [Frontend](https://github.com/rxvinicius/clarke-energia-frontend)
- [Backend](https://github.com/rxvinicius/clarke-energia-backend)
