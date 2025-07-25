# API Node.js - Projeto Bootcamp SoulCode

Este projeto é uma API desenvolvida em Node.js como parte do Bootcamp SoulCode. O objetivo é fornecer uma estrutura básica para gerenciamento de produtos e usuários, utilizando boas práticas de organização de código, autenticação e integração com o Firebase.

## Índice
- [Funcionalidades](#funcionalidades)
- [Estrutura de Pastas](#estrutura-de-pastas)
- [Requisitos](#requisitos)
- [Configuração do Ambiente](#configuração-do-ambiente)
- [Instalação](#instalação)
- [Como Usar](#como-usar)
- [Coleção Postman](#coleção-postman)
- [Scripts Úteis](#scripts-úteis)
- [Credenciais e Segurança](#credenciais-e-segurança)
- [Licença](#licença)

## Funcionalidades
- CRUD de produtos
- CRUD de usuários
- Autenticação e autorização (Firebase)
- Estrutura modularizada (routers, services)
- Exemplo de integração com Firebase

## Estrutura de Pastas
```
Node/
├── .env.example                # Exemplo de variáveis de ambiente
├── API Node.js.postman_collection.json  # Coleção de testes para o Postman
├── comandos.txt                # Comandos úteis para o projeto
├── package.json                # Dependências e scripts do projeto
├── package-lock.json           # Lockfile do npm
└── src/
    ├── index.js                # Ponto de entrada da aplicação
    ├── firebase/
    │   └── app.js              # Configuração do Firebase
    ├── routers/
    │   ├── produtosRouter.js   # Rotas de produtos
    │   └── usuariosRouter.js   # Rotas de usuários
    └── services/
        ├── produtosService.js  # Lógica de negócio de produtos
        └── usuariosService.js  # Lógica de negócio de usuários
```

## Requisitos
- Node.js >= 14.x
- npm >= 6.x

## Configuração do Ambiente
1. Copie o arquivo `.env.example` para `.env` e preencha as variáveis necessárias.
2. Adicione o arquivo de credenciais do Firebase (`serviceAccount.json`) na pasta `Node/` (não versionado por segurança).

## Instalação
```bash
cd Node
npm install
```

## Como Usar
Para iniciar a API em modo desenvolvimento:
```bash
npm start
```
A aplicação estará disponível em `http://localhost:3000` (ou porta definida no `.env`).

## Coleção Postman
O arquivo `API Node.js.postman_collection.json` contém exemplos de requisições para testar todos os endpoints da API. Importe-o no Postman para facilitar seus testes.

## Scripts Úteis
- `npm start` — Inicia a aplicação
- `npm run dev` — Inicia em modo desenvolvimento (se configurado)

## Credenciais e Segurança
- O arquivo `serviceAccount.json` (Firebase) **NÃO** deve ser versionado. Ele é ignorado pelo `.gitignore`.
- Nunca compartilhe suas credenciais públicas.

## Licença
Este projeto é apenas para fins educacionais no Bootcamp SoulCode.
