# 📰 Trabalho Final: Portal de Notícias

## 🎯 Objetivo

Desenvolver um sistema completo de **portal de notícias em PHP**, aplicando os conceitos de desenvolvimento web vistos durante a disciplina. O projeto deve incluir **CRUDs de usuários e notícias**, autenticação, uso de banco de dados relacional e uma interface amigável.

---

## 🧩 Requisitos do Sistema

### 🔐 Autenticação de Usuários

O sistema deve permitir:

- Cadastro de novos usuários
- Login com verificação
- Logout
- Edição e exclusão de contas

### 📰 Tabela de Notícias

A tabela `noticias` deverá conter os seguintes campos:

| Campo   | Tipo        | Regras |
|---------|-------------|--------|
| `id`    | INT         | Chave primária, auto-incremento |
| `titulo`| VARCHAR     | Obrigatório |
| `noticia`| TEXT       | Obrigatório |
| `data`  | DATETIME    | Data/hora da publicação |
| `autor` | INT         | Chave estrangeira referenciando `usuarios.id` |
| `imagem`| VARCHAR     | Opcional – caminho ou URL da imagem |

### 🔗 Relacionamento entre Usuário e Notícia

O campo `autor` na tabela `noticias` deve referenciar o `id` do usuário logado. Assim, cada notícia será associada ao usuário que a cadastrou.

---

## ⚙️ Funcionalidades do Sistema

### 🧑‍💼 Usuário

- Cadastro, login e logout
- Gerenciamento de conta (editar e excluir)
- Só é possível cadastrar notícias **se estiver logado**

### 📝 Notícia

- Cadastro de novas notícias
- Edição e exclusão (apenas pelo autor)
- Listagem pública na página inicial (`index.php`)
- Página individual para leitura da notícia

### 🖥️ Página Inicial (`index.php`)

- Exibe todas as notícias públicas com:
  - Título
  - Resumo (trecho da notícia)
  - Nome do autor
  - Data de publicação
- Notícias mais recentes aparecem primeiro
- Links para visualizar a notícia completa, cadastrar/login, ou publicar nova notícia (caso esteja logado)

---

## 🧪 Diferenciação entre Projetos (por aluno ou Grupo)

Cada aluno deverá personalizar seu projeto de acordo com o tema escolhido. Exemplos:

01 - Portal de Notícias Esportivas
02 - Portal de Noticias sobre Cultura e Arte
03 - Portal de Noticias sobre Tecnologia e Inovação
04 - Portal de Noticias Estudantil
05 - Portal de Noticias de Fofocas
06 - Portal de Noticias sobre o Mundo
07 - Portal de Notícias de Games e E-Sports
08 - Portal de Notícias de Moda e Estilo
09 - Portal de Notícias de Saúde e Bem-Estar
10 - Portal de Notícias de Curiosidades e Fatos Históricos
11 - Portal de Notícias de Fake News (Sátira)
12 - Portal de Notícias Regionais
13 - Portal de Notícias Religiosas ou Filosóficas
14 - Portal de Notícias Ambientais
15 - Portal de Noticias Gastronomia e Receitas
16 - Portal de Noticias Economia e Finanças Pessoais
17 - Portal de Noticias Cinema, Séries e Streaming
18 - Portal de Noticias Astronomia e Ciência Espacial
---

## 🎨 Estilização

- Interface construída com HTML e CSS
- Pode-se utilizar Bootstrap, Tailwind ou qualquer framework frontend
- Interface **responsiva e intuitiva**
- Organização visual clara entre páginas públicas e privadas

---

## 📁 Estrutura Sugerida de Arquivos

### 🏠 Páginas Públicas

| Arquivo           | Descrição                                        |
|-------------------|--------------------------------------------------|
| `index.php`       | Página inicial com listagem de notícias públicas |
| `noticia.php`     | Página individual para leitura de notícia        |
| `login.php`       | Formulário de login                              |
| `cadastro.php`    | Formulário de criação de conta                   |
| `logout.php`      | Encerrar a sessão do usuário                     |
------------------------------------------------------------------------

### 🔐 Área Restrita (após login)

| Arquivo               | Descrição                               |
|-----------------------|-----------------------------------------|
| `dashboard.php`       | Painel do usuário logado                |
| `nova_noticia.php`    | Formulário para nova notícia            |
| `editar_noticia.php`  | Edição de notícias do próprio usuário   |
| `excluir_noticia.php` | Exclusão de notícias do próprio usuário |
-------------------------------------------------------------------

### 👤 CRUD de Usuários (opcional/admin)

| Arquivo                | Descrição                             |
|------------------------|---------------------------------------|
| `usuarios.php`         | Lista de todos os usuários (opcional) |
| `editar_usuario.php`   | Edição de conta                       |
| `excluir_usuario.php`  | Exclusão de conta                     |
------------------------------------------------------------------

### 🧠 Conexão e Funções

| Arquivo              | Descrição                                   |
|----------------------|---------------------------------------------|
| `conexao.php`        | Conexão com o banco de dados                |
| `funcoes.php`        | Funções auxiliares (validação, login, etc.) |
| `verifica_login.php` | Protege páginas que exigem autenticação     |
---------------------------------------------------------------------

### 🧾 Extras

| Arquivo               | Descrição                      |
|-----------------------|--------------------------------|
| `style.css`           | Estilização personalizada      |
| `dump.sql`            | Estrutura e dados do banco     |
| `README.md`           | Este arquivo com as instruções |
| `imagens/`            | Pasta de imagens das notícias  |
---------------------------------------------------------

---

## 📦 Entrega

- Disponibilizar o projeto completo no **GitHub**
- Incluir no repositório:
  - Todos os arquivos do sistema
  - Arquivo `dump.sql` do banco de dados
  - `README.md` com estas instruções
- Enviar o link do repositório via **Google Classroom**

---

## ⏳ Prazos

| Etapa           | Data limite |
|-----------------|-------------|
| Entrega Regular | 19/11/2025  |
| Prazo Extra     | 24/11/2025  |

---

## 🧮 Critérios de Avaliação

| Critério           | Peso |
|--------------------|------|
| Funcionamento      | 40%  |
| Organização        | 20%  |
| Estilização        | 15%  |
| Banco de Dados     | 15%  |
| Entrega/Formatação | 10%  |

---

## 🚀 Boa sorte, devs!

Mostrem tudo o que aprenderam e façam um projeto com a sua cara! Em caso de dúvidas, procure o professor a tempo. 😉
