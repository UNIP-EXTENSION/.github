# Bem Para Todos

Sistema desenvolvido como Projeto de Extensão da UNIP com o objetivo de auxiliar a ONG **Bem Para Todos** no gerenciamento de eventos, usuários e comunicação com seus participantes por meio de uma plataforma digital.

O projeto é dividido em duas aplicações:

* **Backend:** API REST desenvolvida em Spring Boot responsável pelas regras de negócio, autenticação, gerenciamento de usuários e eventos.
* **Frontend:** Aplicativo mobile desenvolvido em React Native responsável pela interface utilizada pelos usuários da plataforma.

## Repositórios

| Projeto      | Descrição                                                          |
| ------------ | ------------------------------------------------------------------ |
| **Backend**  | API REST construída com Spring Boot, PostgreSQL, Redis e RabbitMQ. |
| **Frontend** | Aplicativo mobile desenvolvido em React Native, Expo e TypeScript. |

Cada repositório possui um README próprio com instruções detalhadas de instalação, execução e documentação técnica.

## Protótipo

Antes do desenvolvimento da aplicação foi elaborado um protótipo de alta fidelidade utilizando o Figma, servindo como base para a implementação das telas e definição da experiência do usuário.

**Figma:**
https://www.figma.com/design/ICfNfWHxD6tCE80hA1NkuN/App-Bem-Para-Todos?node-id=0-1&p=f&t=JEbPqjDttWjGQzB7-0

## Objetivo

O projeto **Bem Para Todos** foi desenvolvido para facilitar a organização dos eventos promovidos pela ONG, oferecendo uma plataforma que centraliza o gerenciamento das principais funcionalidades da instituição.

A plataforma permite que:

* Usuários realizem cadastro e login;
* Usuários recuperem sua senha por e-mail;
* Administradores gerenciem eventos;
* Usuários visualizem eventos cadastrados;
* Usuários consultem galerias de imagens;
* O sistema realize autenticação segura utilizando JWT;
* Os dados sejam armazenados de forma segura.

## Arquitetura

```text
Frontend (React Native)
          │
          │ HTTP (Axios)
          ▼
Backend (Spring Boot)
          │
          │ Spring Data JPA
          ▼
PostgreSQL
```

Além do banco de dados, o backend utiliza **Redis** para o fluxo de recuperação de senha e **RabbitMQ** para processamento assíncrono do envio de e-mails.

## Tecnologias utilizadas

### Frontend

* React Native
* Expo
* TypeScript
* React Navigation
* React Hook Form
* Axios
* AsyncStorage
* Expo Image Picker

### Backend

* Java 21
* Spring Boot
* Spring Security
* Spring Data JPA
* PostgreSQL
* Redis
* RabbitMQ
* MapStruct
* JWT
* Swagger

## Funcionalidades

* Cadastro de usuários
* Login com JWT
* Recuperação de senha por e-mail
* Gerenciamento de eventos
* Gerenciamento de Dress Codes
* Perfil do usuário
* Galeria de imagens
* API REST

## Como executar o projeto

Clone os dois repositórios:

```bash
git clone <URL_FRONTEND>
git clone <URL_BACKEND>
```

### 1. Inicie o Backend

Entre na pasta do backend e siga as instruções presentes no README correspondente.

Após iniciado, a API estará disponível em:

```text
http://localhost:8080
```

A documentação da API (Swagger) estará disponível em:

```text
http://localhost:8080/swagger-ui.html
```

### 2. Inicie o Frontend

Entre na pasta do frontend e execute as instruções presentes no README.

Após iniciado, basta abrir o aplicativo utilizando o **Expo Go** ou um emulador Android/iOS.

## Organização do projeto

```text
Bem-Para-Todos
├── frontend
│   └── Aplicativo Mobile em React Native
│
├── backend
│   └── API REST em Spring Boot
│
└── README.md
```

## Documentação

Cada projeto possui sua própria documentação:

* **Backend:** documentação completa da API, autenticação, Docker, banco de dados, rotas, Swagger, scripts e configurações.
* **Frontend:** documentação da aplicação mobile, estrutura do projeto, configuração do ambiente, scripts e execução.

## Equipe

Projeto desenvolvido como parte do Projeto de Extensão da Universidade Paulista (UNIP).

## Licença

Este projeto foi desenvolvido exclusivamente para fins acadêmicos como parte do Projeto de Extensão da UNIP.
