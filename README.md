# Lista de Tarefas com Autenticação

![Status](https://img.shields.io/badge/status-desafio%20t%C3%A9cnico-2ea44f?style=for-the-badge)
![Next.js](https://img.shields.io/badge/Next.js-13%2B-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![JSON Server](https://img.shields.io/badge/JSON%20Server-API-000000?style=for-the-badge)
![Licença](https://img.shields.io/badge/licença-MIT-042570?style=for-the-badge)

> Desafio de desenvolvimento fullstack para candidatos, com **Next.js** e **TailwindCSS**: criar uma
> aplicação web de gerenciamento de tarefas com autenticação segura e design moderno. A API de apoio
> roda localmente com JSON Server, a partir de `server/db.json`.

## Sumário

- [Sobre o sistema](#-sobre-o-sistema)
- [O que ele faz](#-o-que-ele-faz)
- [Ajustes e melhorias](#-ajustes-e-melhorias)
- [Pré-requisitos](#-pré-requisitos)
- [Instalando o desafio Lista de Tarefas com Autenticação](#-instalando-o-desafio-lista-de-tarefas-com-autenticação)
- [Usando o desafio Lista de Tarefas com Autenticação](#-usando-o-desafio-lista-de-tarefas-com-autenticação)
- [Configuração](#-configuração)
- [Arquitetura](#-arquitetura)
- [Testes](#-testes)
- [CI e deploy](#-ci-e-deploy)
- [Contribuindo para o desafio Lista de Tarefas com Autenticação](#-contribuindo-para-o-desafio-lista-de-tarefas-com-autenticação)
- [Colaboradores](#-colaboradores)
- [Documentação](#-documentação)
- [Licença](#-licença)

## 📌 Sobre o sistema

Desafio de desenvolvimento fullstack com **Next.js** e **TailwindCSS**. O objetivo é criar uma
aplicação web de gerenciamento de tarefas com autenticação segura e design moderno.

### 🎯 Objetivo

Desenvolver uma aplicação que:

- ✅ Permita o cadastro e login de usuários
- ✅ Liste, adicione, edite e remova tarefas (CRUD)
- ✅ Garanta que cada usuário visualize apenas suas tarefas
- ✅ Tenha uma interface responsiva e bonita

## 🧭 O que ele faz

### 🚀 Funcionalidades Principais

#### **1. Autenticação de Usuário**

- Registro e login com email/senha
- Sessão persistente com JWT ou cookies (NextAuth)
- Redirecionamento de páginas seguras

#### **2. CRUD de Tarefas**

- Criar tarefas com título e descrição
- Editar e excluir tarefas
- Visualizar tarefas em cards ou listas
- Armazenamento no banco vinculado ao usuário

#### **3. UI Responsiva**

- Interface moderna com TailwindCSS
- Feedback visual para ações (ex: toast de sucesso)
- Layout simples e intuitivo

## 🚧 Ajustes e melhorias

### ✨ Sugestões de Melhorias (Bônus)

- 🔔 Notificações de tarefas
- ⏰ Agendamento com datas e horários
- 📊 Filtro por status (feito/pendente)
- 👥 Múltiplos usuários com permissões
- ☁️ Deploy com banco remoto (ex: Supabase, PlanetScale)

## 💻 Pré-requisitos

Os requisitos técnicos do desafio estão em [Arquitetura](#-arquitetura). Para rodar a API, você
precisa do `npm` e do JSON Server.

## 🚀 Instalando o desafio Lista de Tarefas com Autenticação

### Como rodar a API

Instale o JSON Server (caso ainda não tenha):

```bash
npm install -g json-server
git clone https://github.com/GpDevLab/todo-auth-teste-front
cd todo-auth-teste-front/server
json-server --watch db.json --port 3001
```

A API estará acessível em http://localhost:3001.

## ☕ Usando o desafio Lista de Tarefas com Autenticação

A API servida pelo JSON Server expõe as coleções de `server/db.json`, entre elas `users` e `tasks`.
O uso da aplicação é o descrito em [O que ele faz](#-o-que-ele-faz).

## 🔧 Configuração

O enunciado não define variáveis de ambiente. A API usa a porta 3001, definida no comando acima.

## 🧱 Arquitetura

### 📌 Requisitos Técnicos

#### **Obrigatórios**

- ✅ **Next.js** (versão 13 ou superior)
- ✅ **TailwindCSS** para estilização
- ✅ **Autenticação** via credenciais ou com NextAuth.js

#### **Desejáveis (Bônus)**

- 🧪 **Testes unitários** com Jest/RTL
- 🎨 **Dark/Light Mode**
- 🔐 Middleware de proteção de rotas
- 📱 App responsivo e com animações

## 🧪 Testes

Testes unitários são bônus do desafio, como listado em [Arquitetura](#-arquitetura).

## 🔁 CI e deploy

O enunciado não exige pipeline de CI nem deploy. O deploy com banco remoto é uma das
[sugestões de melhorias](#-ajustes-e-melhorias).

## 📫 Contribuindo para o desafio Lista de Tarefas com Autenticação

Este repositório não recebe contribuições de código: cada candidato entrega o próprio projeto,
seguindo as regras abaixo.

### 📌 Regras de Entrega

- ✅ Subir projeto no GitHub (público)
- ✅ README com:
  - 📦 Instruções de instalação
  - 💡 Decisões técnicas
  - 🚧 Dificuldades e aprendizados

## 🤝 Colaboradores

Este desafio é mantido pela GpDevLab.

## 📚 Documentação

### 📎 Links Úteis

- 🔗 [Next.js](https://nextjs.org/)
- 🎨 [TailwindCSS](https://tailwindcss.com/)
- 🔐 [NextAuth.js](https://next-auth.js.org/)

Boa sorte! 🚀 Dê seu melhor e divirta-se desenvolvendo! 🧠🛠️

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE).
