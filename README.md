# 📚 API de Gerenciamento de Livros

Esta é uma API REST simples construída com **Flask** que permite realizar operações CRUD (Criar, Ler, Atualizar e Deletar) em uma lista de livros fictícia.

## 🚀 Tecnologias utilizadas

- Python 3  
- Flask

## 📦 Instalação

1. Clone este repositório:

```bash
git clone https://github.com/xXWilliaN12Xx/API-com-python.git
cd API-com-python
```

2. Crie e ative um ambiente virtual (opcional, mas recomendado):

```bash
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate     # Windows
```

3. Instale as dependências:

```bash
pip install flask
```

4. Execute a aplicação:

```bash
python app.py
```

A API estará disponível em: `http://localhost:5000`

## 🔄 Endpoints disponíveis

### 📖 Obter todos os livros
**GET** `/livros`  
Retorna a lista completa de livros.

### 🔍 Obter livro por ID
**GET** `/livros/<id>`  
Retorna os dados de um livro específico.

### ➕ Adicionar novo livro
**POST** `/livros`  
Corpo da requisição (JSON):

```json
{
  "id": 4,
  "título": "Nome do Livro",
  "autor": "Nome do Autor"
}
```

### ✏️ Editar livro existente
**PUT** `/livros/<id>`  
Corpo da requisição (JSON):

```json
{
  "título": "Novo Título",
  "autor": "Novo Autor"
}
```

### ❌ Remover livro
**DELETE** `/livros/<id>`  
Remove o livro com o ID correspondente.

## ⚠️ Observações

- Os dados estão armazenados em memória, ou seja, sempre que o servidor é reiniciado, os dados voltam ao estado inicial.  
- Ideal para fins de aprendizado e testes com APIs REST.
