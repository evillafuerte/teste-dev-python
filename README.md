# Teste para Desenvolvedor Python

## Descrição do Desafio

O objetivo deste desafio é criar uma API que permita o upload de um arquivo CSV, que será parseado e seus dados inseridos em um banco de dados SQLite (ou outro SGBD de sua preferência). Além disso, deve-se criar endpoints que permitam a consulta dos dados inseridos no banco.

## Requisitos

- Desenvolver uma API em Python utilizando qualquer framework de sua escolha (sugestão: [FastAPI](https://fastapi.tiangolo.com/)).
- A API deve possuir um endpoint para receber o upload de um arquivo CSV.
- O arquivo CSV deve ser parseado e seus dados inseridos em um banco de dados SQLite.
- A API deve expor endpoints para consultar os dados inseridos.

### Funcionalidades Esperadas

1. **Endpoint de Upload de CSV**
   - Método: `POST`
   - Rota: `/upload`
   - Funcionalidade: Receber o upload de um arquivo CSV, fazer o parse do arquivo e inserir seus dados em um banco de dados SQLite.

2. **Endpoint para Listar Todos os Registros**
   - Método: `GET`
   - Rota: `/data`
   - Funcionalidade: Retornar todos os registros inseridos no banco de dados em formato JSON.

3. **Endpoint para Buscar Registro por ID**
   - Método: `GET`
   - Rota: `/data/<id>`
   - Funcionalidade: Retornar um registro específico a partir de um ID em formato JSON.

### Estrutura Esperada do CSV

O arquivo CSV que será enviado à API deverá conter as seguintes colunas:

- `id`: Identificador único do registro.
- `name`: Nome do item.
- `value`: Valor associado ao item.
- `date`: Data relacionada ao registro.

Exemplo de conteúdo do CSV:

```csv
id,name,value,date
1,Item A,10.5,2024-01-01
2,Item B,7.8,2024-01-02
3,Item C,15.3,2024-01-03
```
Obs.: Gerar um csv aleatório seguindo esse layout, porém commitar junto com o projeto.

## Critérios de Avaliação

- Qualidade do código.
- Estrutura e organização do projeto.
- Tratamento de erros e validação.
- Documentação e clareza das instruções (README).
- Boa prática de uso do SQLite e manipulação de arquivos CSV.
- Testes unitários (opcional, mas será um diferencial).
- Configuração para execução com Docker Compose (opcional, mas será um diferencial).
