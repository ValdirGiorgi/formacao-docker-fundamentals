# 🐳 Desafio DIO - Docker Fundamentals

Este projeto é um desafio do curso de Docker da DIO. O objetivo é executar uma página HTML simples em um container Apache usando Docker Compose.

## Sobre o Projeto

O projeto consiste em:
- Um arquivo `docker-compose.yml` que define o serviço Apache
- Uma página `index.html` simples exibindo "Hello World! Este é um desafio da DIO - Curso de Docker."

## Tecnologias Utilizadas

- Docker
- Docker Compose
- Apache HTTP Server
- HTML5

## Estrutura do Projeto

```
docker/
├── docker-compose.yml   # Configuração do Docker Compose
├── README.md            # Documentação do projeto
└── src/
    └── index.html      # Página principal Hello World
```

## Como Executar

### Pré-requisitos
- Docker instalado
- Docker Compose instalado

### Passos

1. Clone o repositório:
   ```bash
   git clone https://github.com/ValdirGiorgi/formacao-docker-fundamentals.git
   cd formacao-docker-fundamentals/docker
   ```

2. Execute o serviço:
   ```bash
   docker-compose up -d
   ```

3. Acesse a aplicação:
   - Abra o navegador e acesse: `http://localhost:80`

4. Para parar o serviço:
   ```bash
   docker-compose down
   ```

## docker-compose.yml

Exemplo de configuração:

```yaml
version: '3.9'
services:
  apache:
    image: httpd:latest
    container_name: my-apache-web
    ports:
      - "80:80"
    volumes:
      - ./src:/usr/local/apache2/htdocs
```

## Licença

Projeto para fins educacionais.
