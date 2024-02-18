Thaylon Ramon Ramos Ribeiro
# Mangás API
**Objetivo** - Criar um api que disponibiliza a consulta, criação, edição e exclusão de mangás.

## Tecnologias Utilizadas
- PYTHON
- FLASK

## INICIAR
    Apos baixar o baixar o repositorio , abra a pasta com o vscode e de run python file ou no terminal :
```
   cd apii python
```

 ```json
     python app.py
```
    Assim agora você poderá utilizar a API com os links abaixos.
## URL API

http://localhost:5000
- localhost:5000/livros (GET)
- localhost:5000/livros (POST)
- localhost:5000/livros/id (GET)
- localhost:5000/livros/id (PUT)
- localhost:5000/livros (DELETE)

## [GET] /livros

**Descrição**: Retorna todos os livros.

**Exemplo de Resposta**:
```json
[
    {
        "id": 1,
        "titulo": "Naruto - Shipuuden",
        "autor": "Masashi Kishimoto"
    },
    {
        "id": 2,
        "titulo": "One Piece",
        "autor": "Echiro Oda"
    },
    {
        "id": 3,
        "titulo": "Dragon Ball Z",
        "autor": "Akira Toryama"
    }
]
```

## [GET] /livros/{id}
**Descrição**: Retorna um único livro pelo ID.

Exemplo de Resposta:
```json
    {
    "id": 1,
    "titulo": "Naruto - Shipuuden",
    "autor": "Masashi Kishimoto"
    }

```

## [POST] /livros
**Descrição**: Cadastra um novo livro.

Exemplo de Resposta:
```json
    {
    "titulo": "Título do Novo Livro",
    "autor": "Autor do Novo Livro"
    }

```
**Exemplo de Resposta**:
```json
   [
    {
        "id": 1,
        "titulo": "Naruto - Shipuuden",
        "autor": "Masashi Kishimoto"
    },
    {
        "id": 2,
        "titulo": "One Piece",
        "autor": "Echiro Oda"
    },
    {
        "id": 3,
        "titulo": "Dragon Ball Z",
        "autor": "Akira Toryama"
    },
    {
        "id": 4,
        "titulo": "Título do Novo Livro",
        "autor": "Autor do Novo Livro"
    }
]

```

## [PUT] /livros/{id}
**Descrição**: Atualiza dados do livro.
**Observações**: É necessário token de acesso via header(x-access-token)

Exemplo de Resposta:
```json
   {
    "titulo": "Novo Título do Livro",
    "autor": "Novo Autor do Livro"
    }


```
**Exemplo de Resposta**:
```json
   {
    "id": 1,
    "titulo": "Novo Título do Livro",
    "autor": "Novo Autor do Livro"
}


```
## [DELETE] /livros/{id}
**Descrição**: Exclui um único livro.

```json
   [
    {
        "id": 1,
        "titulo": "Naruto - Shipuuden",
        "autor": "Masashi Kishimoto"
    },
    {
        "id": 2,
        "titulo": "One Piece",
        "autor": "Echiro Oda"
    },
    {
        "id": 3,
        "titulo": "Dragon Ball Z",
        "autor": "Akira Toryama"
    }
]

```
**Exemplo de Resposta**:
```json
   [
    {
        "id": 2,
        "titulo": "One Piece",
        "autor": "Echiro Oda"
    },
    {
        "id": 3,
        "titulo": "Dragon Ball Z",
        "autor": "Akira Toryama"
    }
]



```
Pode utilizar o programa "Postman" para testar e fazer a manipulação e testes na api.
[Postman](https://www.postman.com/downloads/)

Exemplos : 
    **localhost:5000/livros (GET)**
    ![get](https://i.imgur.com/FnLAxJQ.png)

Agora pode usar os outros endpoist para usar a api.

## - Créditos - Fontes de referência utilizadas
[![Badge](https://img.shields.io/badge/Leia%20mais-Programa%C3%A7%C3%A3o%20em%20Python%20com%20Flask-blue?style=for-the-badge&logo=python)](https://blog.debugeverything.com/pt/programacao-em-python-aplicativo-flask/)
[![youtube](https://img.shields.io/badge/YouTube-red?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@pycodebr)

## Licença

[MIT](https://choosealicense.com/licenses/mit/)

