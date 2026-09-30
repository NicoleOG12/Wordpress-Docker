# 🐳 WordPress + MariaDB

Projeto desenvolvido para a atividade de Docker Compose, com o objetivo de subir um ambiente de Gerenciamento de Conteúdo utilizando WordPress e MariaDB.

## 📦 Serviços

O ambiente é composto por dois serviços:

* **WordPress:** utiliza a imagem oficial `wordpress:latest`
* **MariaDB:** utiliza a imagem oficial `mariadb:10.6`

O WordPress depende do serviço MariaDB para armazenar os dados da aplicação.

## 🚀 Como executar

Clone o repositório:

```bash
git clone URL_DO_REPOSITORIO
```

Entre na pasta:

```bash
cd docker-wordpress
```

Suba os containers:

```bash
docker compose up -d
```

Verifique os serviços:

```bash
docker compose ps
```

## 🌐 Acesso

Após os containers iniciarem, o WordPress pode ser acessado em:

```text
http://localhost:8000
```

## 🛑 Parar os containers

```bash
docker compose down
```

## 💾 Persistência

O MariaDB utiliza um volume Docker chamado `db_data`, garantindo a persistência dos dados do banco mesmo quando os containers são removidos.
