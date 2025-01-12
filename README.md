# Projeto de Ecommerce com Laravel

Este repositório contém o código-fonte de um projeto de ecommerce desenvolvido com o framework Laravel.

## Requisitos

- PHP >= 7.3
- Composer
- PostgreSQL
- Extensão PHP para PostgreSQL

## Instalação

1. Clone o repositório:
    ```sh
    git clone https://github.com/seu-usuario/seu-repositorio.git
    ```
2. Navegue até o diretório do projeto:
    ```sh
    cd seu-repositorio
    ```
3. Instale as dependências do Composer:
    ```sh
    composer install
    ```
4. Copie o arquivo `.env.example` para `.env` e configure suas variáveis de ambiente, especialmente as configurações do banco de dados PostgreSQL:
    ```sh
    cp .env.example .env
    ```
    Exemplo de configuração do banco de dados no arquivo `.env`:
    ```
    DB_CONNECTION=pgsql
    DB_HOST=127.0.0.1
    DB_PORT=5432
    DB_DATABASE=nome_do_banco
    DB_USERNAME=seu_usuario
    DB_PASSWORD=sua_senha
    ```
5. Gere a chave da aplicação:
    ```sh
    php artisan key:generate
    ```
6. Execute as migrações do banco de dados:
    ```sh
    php artisan migrate
    ```

## Uso

Para iniciar o servidor de desenvolvimento, execute:
```sh
php artisan serve
```