# 🥇 Primeiro Contato com Docker

Este projeto marcou meu primeiro contato prático com o Docker, desde a instalação da ferramenta até a execução bem-sucedida da minha primeira aplicação containerizada. Foi uma experiência inicial para entender na prática como criar, empacotar e rodar aplicações em ambientes isolados usando containers.

## 🧪 Projeto: Hello World com Spring Boot em Container Docker

Este projeto é um exemplo simples de uma aplicação Spring Boot containerizada com Docker. Ele exibe a tradicional mensagem **"Hello World"** e tem como objetivo demonstrar a criação, execução e acesso a uma aplicação Java dentro de um contêiner Docker.

### 🔧 Tecnologias Utilizadas

- Java 17+
- Spring Boot
- Maven
- Docker

### 🚀 Como funciona

A aplicação foi desenvolvida utilizando o Spring Boot e configurada para rodar na porta `8080` dentro do contêiner. Para permitir o acesso via navegador a partir da máquina host, foi realizado o mapeamento de portas entre o contêiner e o host.

### 🔄 Mapeamento de porta

O contêiner foi executado com o seguinte comando:

```bash
docker run -p 8080:8080 hello-world-springboot
```

Isso permite acessar a aplicação através do seguinte endereço:

```
http://localhost:8080
```

Ao acessar, você verá a mensagem:

```
Hello World
```

### 📁 Estrutura básica

- `src/main/java` – Contém a classe principal e o controlador responsável pela mensagem.
- `Dockerfile` – Define a imagem personalizada usada para construir o contêiner.
- `pom.xml` – Gerenciador de dependências do Maven.
