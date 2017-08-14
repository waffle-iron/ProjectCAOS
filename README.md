[![Stories in Ready](https://badge.waffle.io/mateusbpt/ProjectCAOS.png?label=ready&title=Ready)](https://waffle.io/mateusbpt/ProjectCAOS?utm_source=badge)
# ProjectCAOS - Controlling Activities Of Students [![Build Status](https://travis-ci.org/mateusbpt/ProjectCAOS.svg?branch=master)](https://travis-ci.org/mateusbpt/ProjectCAOS)

Aplicação criada com o objetivo ajudar na organização das avaliações dos repositórios dos estudantes do Projeto Crescer.

[**Trello**: informações do que está sendo/ainda será feito](https://trello.com/b/wmcOsXBx/anonymousquestions)

# Quickstart

- Para **instalar as dependências**, utilize o comando `npm install` na raiz do repositório.

- Para realizar o **build da API**, utilize o comando `npm run build`.

- Para inicializar o **banco**, utilize o comando `npm run start-db`. 

- Para inicializar a **API** (depois do build), use o comando `npm run start`.

## TODOs
- Criar informações dos demais scripts do `package.json`.

- Criar tutorial de como instalar o mongo-db.

# Arquitetura

A aplicação consiste de um conjunto de serviços disponibilizados pela API a serem consumidos pelo client (*front-end*).

Os serviços da API (que realizam tarefas e acessam o DB) rodam em um servidor à parte do servidor de *assets*.

Ambos utilizam **Node.js** e **Typescript**. A API utiliza autenticação via **WebToken (JWT)** e **MongoDB** como banco de dados. O *front-end* está montado utilizando **Sass** e **Vue.js**.

# Modelo de projeto

O diretório `api` é destinado à API com os serviços a serem consumidos pela aplicação (*back-end* real).

O diretório `app` é destinado à criação do *front-end* e ao servidor de *assets* (como `.js`, `.htlm` e `.css`).
