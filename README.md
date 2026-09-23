# 🏟️ Agenda Sport

Sistema desenvolvido para facilitar a **reserva e gerenciamento de quadras esportivas**, permitindo que usuários encontrem locais, consultem horários disponíveis e realizem reservas de forma rápida e organizada.

O projeto conta com uma aplicação **Web**, um **aplicativo Mobile** e uma **API Back-end**, integrados a um banco de dados.

---

## 👥 Equipe

| Integrante       | Integrante   |
| ---------------- | ------------ |
| João Lucas Dutra | Registrador  |
| Lucas Pouey      | Scrum Master |
| Rafael Djouquin  |      PO      |
| Helaman Brollo   |   Guardião   |

---

## 📌 Sobre o Projeto

### Problema

Atualmente, a reserva de quadras esportivas pode ser um processo pouco organizado, envolvendo contato direto com os estabelecimentos, troca de mensagens e dificuldade para consultar horários disponíveis.

### Público-alvo

* Pessoas que frequentam quadras esportivas;
* Clientes que desejam realizar reservas;
* Administradores de locais esportivos;
* Responsáveis pelo gerenciamento de quadras e horários.

### Objetivo

O **Agenda Sport** tem como objetivo facilitar o aluguel de quadras esportivas, permitindo que os usuários:

* 🔎 Pesquisem locais esportivos;
* 🏟️ Consultem quadras disponíveis;
* 📅 Visualizem horários disponíveis;
* 📋 Consultem informações dos locais;
* 🏸 Visualizem equipamentos e recursos disponíveis;
* 📆 Realizem reservas;
* 🔔 Recebam notificações sobre suas reservas.

Para os administradores, o sistema permitirá gerenciar **quadras, horários, reservas, dias de funcionamento, informações e equipamentos do estabelecimento**.

---

# 🛠️ Tecnologias

## 🌐 Front-end Web

### React

Utilizado para desenvolver a aplicação Web do Agenda Sport, permitindo a criação de uma interface dinâmica, responsiva e adequada para diferentes dispositivos.

* React
* JavaScript / TypeScript
* HTML
* CSS

---

## 📱 Aplicativo Mobile

### React Native + Expo

Utilizados para desenvolver o aplicativo mobile do Agenda Sport para **Android e iOS**, mantendo uma estrutura tecnológica semelhante à aplicação Web.

---

## ⚙️ Back-end

### Node.js + Express

Responsáveis pelo desenvolvimento da API e pelas regras de negócio do sistema.

O back-end será responsável por:

* Gerenciamento de usuários;
* Autenticação;
* Gerenciamento de administradores;
* Gerenciamento de locais;
* Gerenciamento de quadras;
* Controle de horários;
* Gerenciamento de reservas;
* Comunicação com o banco de dados;
* Processamento das regras de negócio.

---

## 🗄️ Banco de Dados

### MySQL

Utilizado para armazenar e organizar os dados do sistema, incluindo:

* Usuários;
* Administradores;
* Locais esportivos;
* Quadras;
* Horários;
* Reservas;
* Equipamentos;
* Dias de funcionamento.

---

## 🔐 Autenticação

### JWT — JSON Web Token

Utilizado para realizar a autenticação dos usuários e controlar o acesso às diferentes áreas do sistema.

O JWT será utilizado para diferenciar, por exemplo:

* Usuários comuns;
* Administradores;
* Áreas restritas do sistema.

---

## 🔔 Notificações

### Firebase Cloud Messaging — FCM

Utilizado para o envio de notificações aos usuários e administradores.

Entre as notificações previstas estão:

* 📩 Nova solicitação de reserva;
* ✅ Reserva aceita;
* ❌ Reserva recusada;
* 🕐 Alteração de horário;
* ⏰ Lembrete de reserva.

---

## 🎨 Design e Prototipação

### Figma

Utilizado para criação dos protótipos e definição da interface do sistema.

Os protótipos serão utilizados para planejar:

* Telas da aplicação Web;
* Telas do aplicativo Mobile;
* Fluxos de navegação;
* Experiência do usuário;
* Componentes visuais;
* Layouts responsivos.

---

## 📦 Versionamento

### Git + GitHub

Utilizados para controle de versão, organização e colaboração entre os integrantes da equipe.

O GitHub também será utilizado para:

* Gerenciamento do código-fonte;
* Controle de branches;
* Pull Requests;
* Issues;
* Organização das tarefas;
* Acompanhamento do desenvolvimento do projeto.

---

# 🏗️ Estrutura do Projeto

A estrutura do projeto será organizada de forma a separar as diferentes aplicações e responsabilidades do sistema.

```text
AgendaSport/
│
├── frontend/        # Aplicação Web
│
├── mobile/          # Aplicativo Mobile
│
├── backend/         # API e regras de negócio
│
├── database/        # Scripts e estrutura do banco de dados
│
├── docs/            # Documentação e protótipos
│
└── README.md
```

---

# 🔄 Funcionamento do Sistema

O fluxo principal do Agenda Sport será:

```text
Usuário
   │
   ▼
Aplicação Web / Mobile
   │
   ▼
API — Node.js + Express
   │
   ├── Autenticação — JWT
   │
   ├── Reservas
   │
   ├── Usuários
   │
   ├── Quadras
   │
   └── Horários
   │
   ▼
MySQL
   │
   ▼
Firebase Cloud Messaging
   │
   ▼
Notificações
```

---

# 🎯 Principais Funcionalidades

### 👤 Usuário

* Cadastro e login;
* Pesquisa de locais esportivos;
* Visualização de quadras;
* Consulta de disponibilidade;
* Visualização de informações do local;
* Visualização de equipamentos;
* Realização de reservas;
* Acompanhamento das reservas;
* Recebimento de notificações.

### 🏢 Administrador

* Cadastro e gerenciamento do local;
* Gerenciamento de quadras;
* Definição de horários;
* Definição dos dias de funcionamento;
* Visualização das reservas;
* Aprovação ou recusa de reservas;
* Gerenciamento das informações do estabelecimento;
* Gerenciamento dos equipamentos disponíveis.

---

# 🚀 Objetivo do Projeto

O Agenda Sport busca proporcionar uma experiência mais **simples, rápida e organizada** para a reserva de quadras esportivas, conectando usuários e administradores em uma única plataforma.

O projeto também tem como objetivo aplicar, na prática, conhecimentos de **desenvolvimento Web, desenvolvimento Mobile, APIs, banco de dados, autenticação, versionamento e metodologias de desenvolvimento de software**.
