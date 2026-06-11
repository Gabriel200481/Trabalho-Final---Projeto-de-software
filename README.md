<!-- Este template foi criado para servir como referência e pode ser facilmente adaptado para diferentes projetos de desenvolvimento -->

<a href="#"><img src="[https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)" width="200"/></a> <a href="#"><img src="[https://classroom.github.com/assets/launch-codespace-2972f46106e565e64193e422d61a12cf1da4916b45550586e14ef0a7c637dd04.svg](https://classroom.github.com/assets/launch-codespace-2972f46106e565e64193e422d61a12cf1da4916b45550586e14ef0a7c637dd04.svg)" width="250"/></a>

---

# 🏷️ Mango Fit Academia 👨‍💻

> [!NOTE]
> Sistema completo para gestão de academias poliesportivas. **Foque no principal valor/benefício:** Automatizar a criação de treinos periodizados (hipertrofia), agendamento de aulas de luta e controle de catraca via status financeiro.

<table>
  <tr>
    <td width="800px">
      <div align="justify">
        Este <b>README.md</b> apresenta a documentação arquitetural do <b>Mango Fit Academia</b>. O projeto foi desenhado para atender às necessidades complexas de uma academia moderna, unificando a gestão de alunos, controle de inadimplência na catraca, prescrição de treinos e lotação de turmas de artes marciais. Elaborado como parte da disciplina de Projeto de Software da Engenharia de Software da PUC Minas, o sistema aplica <i>organização clara</i> e <b>boas práticas</b> de arquitetura corporativa, contando com diagramação UML (PlantUML) para facilitar a compreensão do domínio. Observação: Este repositório foca 100% na modelagem e documentação de software.
      </div>
    </td>
    <td>
      <div>
        <img src="https://placehold.co/120x120/F97316/white?text=Mango+Fit" alt="Logo do Projeto" width="120px" style="border-radius: 15px;"/>
      </div>
    </td>
  </tr> 
</table>

---

## 🚧 Status do Projeto

[![Versão](https://img.shields.io/badge/Versão-v1.0.0-blue?style=for-the-badge)](#) ![React](https://img.shields.io/badge/React-18.2.0-007ec6?style=for-the-badge&logo=react&logoColor=white) ![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-3.4.1-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white) ![Java](https://img.shields.io/badge/Java-17-007ec6?style=for-the-badge&logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.2.0-007ec6?style=for-the-badge&logo=springboot&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16-316192?style=for-the-badge&logo=postgresql&logoColor=white)

---

## 📚 Índice
- [Links Úteis](#-links-úteis)
- [Sobre o Projeto](#-sobre-o-projeto)
- [Funcionalidades Principais](#-funcionalidades-principais)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Arquitetura](#-arquitetura)
- [Instalação e Execução](#-instalação-e-execução)
- [Estrutura de Pastas](#-estrutura-de-pastas)
- [Autores](#-autores)

---

## 🔗 Links Úteis
* 🌐 **Demo Online:** [Apenas Documentação Acadêmica](#)
* 📖 **Documentação:** [Acesse a pasta de Diagramas PlantUML](https://github.com/Gabriel200481/Trabalho-Final---Projeto-de-software/tree/main/Diagramas)

---

## 📝 Sobre o Projeto

A Mango Fit Academia nasceu da necessidade de unificar o controle operacional de academias de médio e grande porte, que frequentemente sofrem com a fragmentação de sistemas (um software para financeiro, outro para treinos, e o uso de planilhas no salão). 

Ele resolve a dor do instrutor que precisa de um meio ágil para atualizar treinos periodizados de hipertrofia e gerenciar as capacidades de lotação do tatame. O cenário de aplicação abrange academias que oferecem tanto a musculação clássica quanto aulas de artes marciais (Muay Thai, Jiu-Jitsu), além de exigir forte controle de acesso físico integrado ao financeiro.

---

## ✨ Funcionalidades Principais

- 🔐 **Autenticação Baseada em Perfis:** Acessos distintos para Aluno, Instrutor e Recepcionista.
- 🏋️ **Gestão de Treinos:** Criação e atribuição de rotinas de treino focadas em hipertrofia (séries, repetições, carga).
- 🥋 **Agendamento de Aulas:** Sistema de check-in para turmas com vagas limitadas.
- 🚧 **Integração de Catraca:** Bloqueio e liberação física automatizados com base no status da mensalidade (Pendente, Paga, Atrasada).
- 📈 **Painel Financeiro:** Controle de faturas mensais, processamento de pagamentos e histórico de inadimplência.

---

## 🛠 Tecnologias Utilizadas

O ecossistema planejado (stack teórica) para a execução e viabilidade do projeto envolve as seguintes ferramentas:

### 💻 Front-end
* **Biblioteca:** React v18
* **Linguagem:** TypeScript
* **Estilização:** Tailwind CSS (para prototipagem rápida e componentes responsivos).
* **Build Tool:** Vite

### 🖥️ Back-end
* **Linguagem:** Java 17 (JDK)
* **Framework:** Spring Boot 3.x
* **Banco de Dados:** PostgreSQL 16
* **ORM / Query Builder:** Hibernate / JPA
* **Autenticação:** Spring Security + JWT

---

## 🏗 Arquitetura

O sistema Mango Fit utiliza uma arquitetura baseada em **Camadas (Layered Architecture)** no Back-end (Controller, Service, Repository) combinada com o padrão **MVC**. Esta arquitetura foi escolhida por proporcionar uma separação clara de responsabilidades, facilitando a aplicação de regras de negócios rigorosas (como o decremento de vagas em turmas e liberação de catracas).

O modelo segue o padrão **Cliente-Servidor**. O Front-end é uma Single Page Application (SPA) que consome dados de forma assíncrona da API RESTful do Spring Boot.


## 🔧 Instalação e Execução (Estrutura Fictícia)

### Pré-requisitos
* **Java JDK:** Versão 17
* **Node.js:** Versão v18.x LTS
* **PostgreSQL:** Rodando na porta 5432

### 🔑 Variáveis de Ambiente

Crie o arquivo `.env.local` na pasta `/frontend`:
~~~env
VITE_API_URL=http://localhost:8080/api
~~~

Configure no `application.yml` do Spring Boot (`/backend/src/main/resources`):
~~~yaml
spring:
  datasource:
    url: jdbc:postgresql://localhost:5432/mangofit_db
    username: postgres
    password: password123
  jpa:
    hibernate:
      ddl-auto: update
~~~

### ⚡ Como Executar a Aplicação

**Terminal 1: Back-end (Spring Boot)**
~~~bash
cd backend
./mvnw spring-boot:run
~~~

**Terminal 2: Front-end (React, Vite)**
~~~bash
cd frontend
npm install
npm run dev
~~~

---

## 📂 Estrutura de Pastas

Como este repositório é focado 100% na modelagem e documentação arquitetural do sistema, a estrutura de arquivos reflete a organização dos diagramas em código-fonte (PlantUML) e a documentação oficial:

~~~text
Trabalho-Final---Projeto-de-software/
├── README.md                                          # 📘 Documentação principal do projeto
├── /Documentação                                      # 📄 Documentos textuais oficiais
│   └── Trabalho 2 - Preenchido - Documentação de Projeto - 20 pontos.pdf
│
└── /Diagramas                                         # 📂 Código-fonte PlantUML dos diagramas
    ├── /Arquitetura e Implantação                     # 🏗️ Visão estrutural e de infraestrutura
    │   ├── arquitetura_geral.puml
    │   ├── componentes_backend.puml
    │   └── implantacao.puml
    │
    ├── /Comportamental Interno                        # 🔄 Interações e ciclos de vida
    │   ├── comunicacao_agendar.puml
    │   ├── comunicacao_pagamento.puml
    │   ├── comunicacao_treino.puml
    │   ├── estados_mensalidade.puml
    │   ├── seq_agendar_aula.puml
    │   ├── seq_montar_treino.puml
    │   └── seq_pagamento.puml
    │
    ├── /Estrutural e Banco de Dados                   # 🗄️ Entidades, atributos e relacionamentos
    │   ├── der_banco_de_dados.puml
    │   └── diagrama_classes.puml
    │
    └── /Requisitos e Visão de Sistema                 # 👤 Atores, casos de uso e visão caixa-preta
        ├── casos_de_uso.puml
        ├── dss_agendar_aula.puml
        ├── dss_montar_treino.puml
        └── dss_pagamento.puml
~~~

---

## 👥 Autores
| 👤 Nome | 🖼️ Foto | :octocat: GitHub | 💼 LinkedIn | 📤 Gmail |
|---------|----------|-----------------|-------------|-----------|
| Gabriel Afonso Infante Vieira | <div align="center"><img src="https://github.com/Gabriel200481.png" width="70px" height="70px"/></div> | <div align="center"><a href="https://github.com/Gabriel200481"><img src="https://joaopauloaramuni.github.io/image/github6.png" width="50px" height="50px"></a></div> | <div align="center"><a href="#"><img src="https://joaopauloaramuni.github.io/image/linkedin2.png" width="50px" height="50px"></a></div> | <div align="center"><a href="mailto:Gabrielvieira200481@gmail.com"><img src="https://joaopauloaramuni.github.io/image/gmail3.png" width="50px" height="50px"></a></div> |
---

## 🙏 Agradecimentos

Gostaria de agradecer aos seguintes canais e pessoas que foram fundamentais para o desenvolvimento deste projeto e para o meu crescimento profissional:

* [**Engenharia de Software PUC Minas**](https://www.instagram.com/engsoftwarepucminas/) - Pelo apoio institucional, estrutura acadêmica e fomento à inovação e boas práticas de engenharia.
* [**Prof. Dr. João Paulo Aramuni**](https://github.com/joaopauloaramuni) - Pelos valiosos ensinamentos sobre **Arquitetura de Software**, **Padrões de Projeto** e disponibilização de templates profissionais.

---

## 📄 Licença

Este projeto é distribuído sob a **[Licença MIT](https://github.com/joaopauloaramuni/laboratorio-de-desenvolvimento-de-software/blob/main/LICENSE)**.
