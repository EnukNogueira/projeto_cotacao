# Currency Data Pipeline

API desenvolvida em Python com FastAPI para consulta de cotações do dólar (USD/BRL) através de uma API financeira externa.

---

## Sobre o projeto

O projeto foi desenvolvido para praticar integração entre uma aplicação Python e uma fonte externa de dados financeiros.

A aplicação realiza uma requisição para obter as cotações do dólar e disponibiliza um endpoint que permite pesquisar se determinado valor de cotação foi registrado nas últimas 30 cotações disponíveis.

---

## Funcionalidades

- Consulta de cotações do dólar
- Integração com API financeira externa
- Pesquisa de um valor específico de cotação
- Retorno da data em que o valor foi encontrado
- Tratamento básico para valores não encontrados
- Documentação automática dos endpoints através do FastAPI

---

## Tecnologias utilizadas

- **Python 3**
- **FastAPI** — criação da API REST
- **Requests** — requisições HTTP
- **AwesomeAPI** — fonte dos dados de cotação
- **Uvicorn** — servidor para execução da aplicação

---

## Endpoint principal

### `GET /cotacao-dolar?pesquisa={valor}`

Pesquisa um determinado valor de cotação do dólar entre as últimas 30 cotações.

Exemplo:

```text
/cotacao-dolar?pesquisa=5.72
```

Quando o valor é encontrado, a API retorna a data e a cotação correspondente.

---

## Estrutura do projeto

- `projeto_dolar.py` — aplicação FastAPI
- `README.md` — documentação do projeto

---

## Como executar

Clone o repositório:

```bash
git clone https://github.com/EnukNogueira/currency-data-pipeline.git
cd currency-data-pipeline
```

Instale as dependências:

```bash
pip install fastapi requests uvicorn
```

Execute a aplicação:

```bash
uvicorn projeto_dolar:app --reload
```

A documentação interativa estará disponível em:

```text
http://127.0.0.1:8000/docs
```

---

## Conceitos praticados

- [x] Criação de API REST
- [x] FastAPI
- [x] Requisições HTTP
- [x] Consumo de API externa
- [x] Manipulação de dados JSON
- [x] Parâmetros de consulta
- [x] Tratamento de respostas
- [x] Documentação automática de API

---

## Objetivo do estudo

O objetivo foi praticar o consumo de APIs externas utilizando Python e entender como disponibilizar esses dados através de uma API própria.

O projeto também serviu como base para meus estudos sobre integração e manipulação de dados.

---

## Autor

**Enuk Nogueira**

Estudante de Análise e Desenvolvimento de Sistemas pela PUCPR, com foco em Análise de Dados e Ciência de Dados.

[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/enuknogueira/)

[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/EnukNogueira)
