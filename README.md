# Langchain Perguntando ao PDF (Tutorial)

Esta é uma aplicação em Python que permite carregar um PDF e fazer perguntas sobre ele usando linguagem natural. A aplicação usa um LLM para gerar uma resposta sobre seu PDF. O LLM não responderá a perguntas não relacionadas ao documento.

## Como funciona

A aplicação lê o PDF e divide o texto em pedaços menores que podem então ser alimentados em um LLM. Ela usa os embeddings da OpenAI para criar representações vetoriais dos pedaços. A aplicação então encontra os pedaços que são semanticamente semelhantes à pergunta feita pelo usuário e alimenta esses pedaços ao LLM para gerar uma resposta.

A aplicação usa Streamlit para criar a GUI e Langchain para lidar com o LLM.

## Instalação

Para instalar o repositório, clone este repositório e instale os requisitos:

```
pip install -r requirements.txt
```

Você também precisará adicionar sua chave da API OpenAI ao arquivo `.env`.

## Uso

Para usar a aplicação, execute o arquivo `main.py` com o CLI do streamlit (após ter instalado streamlit):

```
streamlit run app.py
```
