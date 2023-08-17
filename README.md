# Monolito

## Como rodar o projeto?

### Requisitos

- [poetry](https://python-poetry.org/docs/#installation), para gerenciar as dependências do projeto.
- [pyenv](https://github.com/pyenv/pyenv#installation), para gerenciar as versões do Python.

> Para que o Poetry use a versão do Python do Pyenv você vai precisar rodar o comando:
>
> > `poetry config virtualenvs.prefer-active-python true`

### Passo a passo

#### Instale a versão correta do Python

```sh
pyenv install
```

> Esse comando vai ler o arquivo `.python-version` na raiz do projeto.

#### Instale as dependências

```sh
poetry install
```

> Esse comando vai criar um ambiente virtual e instalar as dependências do projeto.

#### Rode o projeto

```sh
poetry shell
uvicorn src.main:app --reload
```
