
# 🎓 Sistema de Gerenciamento Escolar - Ensino Médio

Este é um sistema web desenvolvido com React, HTML, CSS e JavaScript, com o objetivo de facilitar o gerenciamento de turmas, alunos, professores, comunicados e presenças em uma escola de ensino médio.

## 📌 Funcionalidades

- Cadastro e listagem de alunos
- Registro de presenças com data, hora e localização
- Emissão de comunicados por turma ou aluno
- Painel de turmas e disciplinas
- Interface simples, responsiva e de fácil navegação

---

## 🚀 Tecnologias Utilizadas

- React
- JavaScript (ES6+)
- HTML5
- CSS3
- React Router
- Axios
- JSON Server (para simular a API local)

---

## 🛠️ Guia de Instalação

Siga os passos abaixo para rodar o projeto localmente:

### ✅ Pré-requisitos

- Node.js v18+
- NPM v9+
- Git instalado

### 📦 Passos

1. Clone o repositório:

```bash
git clone https://github.com/seu-usuario/sistema-escolar.git
````

2. Acesse a pasta do projeto:

```bash
cd sistema-escolar
```

3. Instale as dependências:

```bash
npm install
```

4. Inicie o servidor de desenvolvimento:

```bash
npm run dev
```

5. Acesse `http://localhost:5173` no seu navegador.

---

## 🔌 API Reference

A aplicação consome uma API REST simulada com JSON Server. Os principais endpoints disponíveis são:

### 🔹 Base URL

```
http://localhost:3000/api
```

---

### 📄 GET `/students`

Retorna todos os alunos cadastrados.

**Resposta:**

```json
[
  {
    "id": 1,
    "name": "João Silva",
    "class": "3ºA"
  }
]
```

---

### ➕ POST `/students`

Cadastra um novo aluno.

**Body:**

```json
{
  "name": "Maria Oliveira",
  "class": "2ºB"
}
```

---

### 📄 GET `/presences`

Retorna todas as presenças registradas.

**Resposta:**

```json
[
  {
    "id": 1,
    "student": "João Silva",
    "class": "3ºA",
    "summary": "Aula de Matemática",
    "date": "2025-06-05",
    "location": "Sala 202"
  }
]
```

---

### ➕ POST `/presences`

Registra uma nova presença.

**Body:**

```json
{
  "student": "Maria Oliveira",
  "class": "2ºB",
  "summary": "Aula de Biologia",
  "date": "2025-06-06",
  "location": "Sala 101"
}
```

---

### 📄 GET `/announcements`

Retorna os comunicados cadastrados.

---

### ➕ POST `/announcements`

Cria um novo comunicado.

**Body:**

```json
{
  "content": "Prova de História na próxima segunda-feira",
  "class": "1ºC",
  "date": "2025-06-06",
  "author": "Coordenação"
}
```
---

## 🤝 Guia de Contribuição

Contribuições são bem-vindas! Se quiser ajudar a melhorar este sistema, siga as etapas abaixo:

### 📌 Requisitos

* Node.js instalado
* Conhecimentos básicos de React, JS, HTML e CSS
* Boa comunicação e organização nos commits

### 🚀 Como Contribuir

1. Faça um **fork** do repositório

2. Crie uma nova branch:

```bash
git checkout -b feature/nome-da-sua-feature
```

3. Faça suas alterações e commite:

```bash
git commit -m "feat: adiciona nova funcionalidade"
```

4. Envie para o repositório remoto:

```bash
git push origin feature/nome-da-sua-feature
```

5. Abra um **Pull Request** explicando suas alterações.

---

### 🧹 Boas práticas

* Faça commits claros e objetivos
* Teste as funcionalidades antes de enviar
* Comente seu código quando necessário
* Respeite os padrões e estilo do projeto

---

## 👥 Integrantes do Grupo

* Josivaldo Braga
* Edson Nascimento
* João Guilherme
* Ruan Ribeiro
* Gian Vitor

---

## 📄 Licença

Este projeto é apenas educacional e não possui licença comercial no momento.

---

## 📬 Contato

Para dúvidas ou sugestões, abra uma [Issue](https://github.com/bragaz/sistema-escolar/issues) ou envie um e-mail para `jbragaz@outlook.com`.

