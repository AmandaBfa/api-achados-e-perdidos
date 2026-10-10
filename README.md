# API de Achados e Perdidos

Atividade da disciplina de Tecnologia e Construção de Software.

API desenvolvida em Python com Flask para cadastrar, consultar,
atualizar e excluir objetos de achados e perdidos.

## Tecnologias utilizadas

- Python
- Flask
- Google Colab

## Dados dos objetos

Cada objeto possui os seguintes campos:

- id: identificador gerado automaticamente.
- descricao: descrição do objeto.
- local: local relacionado ao objeto.
- data: data informada no cadastro.
- status: situação do objeto.

## Rotas implementadas

| Método | Rota | Função |
|--------|------|--------|
| GET | /objetos | Listar todos os objetos |
| GET | /objeto?id=1 | Consultar um objeto pelo ID |
| POST | /objeto | Cadastrar um objeto |
| PUT | /objeto?id=1 | Atualizar um objeto |
| DELETE | /objeto?id=1 | Excluir um objeto |

O ID 1 nas rotas é apenas um exemplo.

## Como executar

1. Abra o notebook pelo link abaixo.
2. Execute a célula de instalação do Flask.
3. Execute a célula com a implementação da API.
4. Execute a célula de testes para visualizar os resultados.

[Abrir no Google Colab](https://colab.research.google.com/drive/1c1VQrWMePXn_xHnBDblUt9Z2UGAqWr1n?usp=sharing)

## Testes realizados

- Cadastro de um objeto.
- Listagem de todos os objetos.
- Consulta pelo ID.
- Atualização do status.
- Exclusão do objeto.
- Consulta após a exclusão.
- Consulta sem ID.
- Consulta com ID inválido.
- Cadastro com campos obrigatórios faltando.

Os testes utilizam o cliente de testes do Flask, sem iniciar
um servidor acessível por uma URL pública.

## Armazenamento

Os dados são armazenados em memória, sem banco de dados.
Ao executar novamente a célula de implementação da API
ou reiniciar o ambiente, os registros são apagados.
