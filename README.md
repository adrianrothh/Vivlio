# Vivlio — Plataforma de Troca de Livros Usados

> Sistema desenvolvido para promover a troca gratuita e sustentável de livros entre moradores de comunidades locais através de um sistema simplificado de créditos.

---

## Sobre o Projeto

Bibliotecas e feiras comunitárias frequentemente enfrentam dificuldades para precificar livros usados e controlar o fluxo de trocas. O **Sebo Comunitário** resolve esse problema implementando a equivalência por **créditos de doação**:
* **Doou 1 livro** ➔ Ganha **1 crédito**.
* **1 crédito** ➔ Dá direito a **resgatar 1 livro** do acervo.

---

## Regra de Negócio Crítica (RN Crítica)

> **Regra:** Um usuário só pode solicitar o resgate de um livro se possuir **pelo menos 1 crédito ativo** em sua conta.

---

## Tecnologias Utilizadas

### Frontend
* **React** (v18+)
* **Vite** (Build tool e servidor de desenvolvimento)
* **React Router DOM** (Navegação SPA)
* **Axios / Fetch API** (Consumo da API REST)

### Backend
* **Java 17+ / Spring Boot**
* **Spring Data JPA** (Persistência e ORM)
* **Spring Security / JWT** (Autenticação e Autorização)

### Banco de Dados & Infraestrutura
* **PostgreSQL** (Banco de dados relacional)
* **Docker / Docker Compose** (Ambiente de desenvolvimento do BD)

---

## 👥 Equipe e Responsabilidades

| Nome | Papel / Função |
| :--- | :--- |
| **Ana** | Product Owner (PO) |
| **Adrian** | Engenheiro de Requisitos |
| **Daniela** | Quality Assurance (QA) |
| **Marcelo** | Desenvolvedor Frontend |
| **João** | Desenvolvedor Frontend |
| **Leonardo** | Desenvolvedor Backend |
| **Gustavo** | DevOps |

---

## 🚀 Funcionalidades (Escopo do Sistema)

### 🟢 Nível 1 — MVP (Fase Atual)
- [x] **Cadastro e Autenticação:** Registro e login de usuários.
- [x] **Acervo de Livros:** Listagem de livros disponíveis para troca.
- [x] **Cadastro de Doação:** Cadastro de novos livros no acervo (adiciona +1 crédito ao usuário).
- [x] **Solicitação de Troca/Resgate:** Resgate de livros utilizando o saldo de créditos (validação da RN Crítica).

### 🟡 Níveis 2 e 3 — Evoluções Futuras
- [ ] **Avaliação do Estado do Livro:** Classificação de conservação (1 a 5 estrelas).
- [ ] **Clubes de Leitura Locais:** Criação e gestão de grupos comunitários de discussão e leitura.

---

## 📁 Estrutura do Repositório

```text
sebo-comunitario/
├── backend/                  # Aplicação Java Spring Boot
│   ├── src/main/java/        # Controllers, Services, Repositories, Entities
│   └── src/main/resources/   # application.properties / application.yml
├── frontend/                 # Aplicação React + Vite
│   ├── src/components/       # Componentes reutilizáveis
│   ├── src/pages/            # Telas da aplicação (Login, Acervo, Perfil)
│   └── src/services/         # Configuração de chamadas de API (Axios)
└── README.md
