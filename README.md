# Pipeline

## Objetivo

Este projeto tem como objetivo extrair dados sobre o Bolsa Família por município utilizando seu código ibge para coleta de dados através da api do gov

### Iniciando a aplicação

- crie o .env dentro da pasta do notebook

```bash
copy .env.example notebooks\.env
```

- preecha os dados no .env
```bash
api_key=
PGUSER=
PGPASSWORD=
```

- Inicíe com docker compose

```bash
docker compose up --build
```

- Acesse o notebook em:

> [localhost:8888](http://localhost:8888)
> Login: 12345678

- Notebooks

Untitled.ipynb: este notebook é o pipeline elt do projeto

Save_neondb.ipynb: este notebook salva os dados coletados pelo pipeline no neondb

Em Save_neondb.ipynb no campo neon_url deve ser alterada a url para salvar no DB desejado

