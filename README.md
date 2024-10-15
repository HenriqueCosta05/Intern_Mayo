# Intern_Mayo
Solução proposta para o desafio de vaga de estágio da Mayo Consultoria

Esse case técnico teve como objetivo a avaliação das habilidades de código para vaga de **estágio como desenvolvedor full-stack**.

Toda a documentação está disponível neste repositório, enquanto o código foi separado em diferentes repositórios - frontend e backend.

## Front-end
[Link do Repositório](https://github.com/HenriqueCosta05/Intern_Mayo_FrontEnd)

## Back-end
[Link do Repositório](https://github.com/HenriqueCosta05/Intern_Mayo_BackEnd)

### Ajustes e melhorias

O projeto ainda está em desenvolvimento e as próximas atualizações serão voltadas para as seguintes tarefas:

- [ ] Cobertura completa de testes (em andamento)
- [ ] Melhoria na lógica do front-end
- [ ] Deploy adequado do front-end

### Tecnologias Utilizadas


#### Back-end
![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)
![NestJS](https://img.shields.io/badge/nestjs-%23E0234E.svg?style=for-the-badge&logo=nestjs&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-3982CE?style=for-the-badge&logo=Prisma&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)


## 💻 Pré-requisitos

Antes de começar, verifique se você atendeu aos seguintes requisitos:

- Você instalou a versão mais recente do `Node.js e NPM`.
- Você instalou o banco de dados `MySQL` (confira como instalar [aqui](https://dev.mysql.com/downloads/installer/))
- Você instalou o banco de dados de cache `Redis` (confira como instalar [aqui](https://redis.io/docs/latest/operate/oss_and_stack/install/install-redis/))


## 🚀 Instalando o projeto

Para instalar o Case técnico, siga estas etapas:


### Back-end

> Observação: no projeto foram utilizadas as seguintes variáveis de ambientes, a serem adaptadas pelo desenvolvedor:

JWT_SECRET=""

MYSQL_URL=""

REDISHOST=""

REDISPORT=""


```
    git clone https://github.com/HenriqueCosta05/Intern_Mayo_BackEnd.git
```

```
    npm install
```

 Após a instalação das dependências, devemos criar um banco de dados respectivo com o Prisma, executando o seguinte comando:

```
    npx prisma db push
```

Para esse projeto, fiz uso do `Prisma` como ORM de banco de dados. Portanto, para executar as alterações realizadas com essa ferramenta, execute os comandos:

```
    npx prisma db push 
```
```
    npx prisma migrate dev --name init
```
Após a sincronização com o banco de dados, devemos realizar o seguinte comando, para inicializar o NestJS:

```
    npm run start:dev
```

