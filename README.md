# Versions.core

O intuito deste repositório é o teste e entendimento de como funcionam os gitmodules e, juntamente com isso, o funcionamento de um simples sistema de microserviço responsável por fazer o cadastro e login do usuário. 

O sistema não conta com nenhuma interface de front-end para realização do login nem criação do usuário.

## Tecnologias 
Node, Nest.js, Prisma, SQLite, Jest, Swagger + Scalar

## Divisão do projeto

Para entender melhor o que faz cada módulo, consulte o README.md de cada módulo, disponível no final de cada descrição.

**Versions.core** -
Concentra o projeto "final", agrupando todos os demais módulos necessários para o funcionamento do sistema. [README.core](https://github.com/JoaoVitorGirardii/versions.core/blob/master/README.md)

**Versions.login** - 
Ponta de entrada para o sistema, responsável por receber as requisições vindas do usuário. [README.login](https://github.com/JoaoVitorGirardii/versions.login/blob/master/README.md)

**Versions.usuarios** - 
Responsável por controlar os usuários do sistema, tendo como único intuito gravar e consultar usuários. [README.usuarios](https://github.com/JoaoVitorGirardii/versions.usuarios/blob/master/README.md)

**Versions.auth** - 
Responsável por validar se o usuário digitou os dados de login corretamente e retornar o seu token de acesso ao sistema. [README.auth](https://github.com/JoaoVitorGirardii/versions.auth/blob/master/README.md)

## Baixe e teste

Clone o projeto

```bash
  git clone https://github.com/JoaoVitorGirardii/versions.core.git
```

Vá para a pasta do projeto

```bash
  cd versions.core
```

Instale os submódulos
```bash
  git submodule update --init --recursive
```

Instale as dependências
```bash
  npm install
```

Executa o container docker
```bash
  docker compose up --build
```

Por fim, acesse onde será possível ter acesso aos endpoints disponíveis para testes
```
  http://localhost:3000/api/reference
```