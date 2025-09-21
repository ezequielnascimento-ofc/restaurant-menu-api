# Cardápio de Restaurante
[![Java](https://img.shields.io/badge/Java-17-%23ED8B00?logo=openjdk)](https://jdk.java.net/17/)
[![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.1.5-%236DB33F?logo=spring)](https://spring.io/projects/spring-boot)
[![MySQL](https://img.shields.io/badge/MySQL-%234479A1?logo=mysql&logoColor=white)](https://www.mysql.com)
[![Swagger](https://img.shields.io/badge/Swagger-2.1.0-%2385EA2D?logo=swagger)](https://swagger.io/)
[![JUnit5](https://img.shields.io/badge/JUnit5-5.9.3-%25B60017?logo=junit5)](https://junit.org/junit5/)
[![codecov](https://codecov.io/gh/Ki3lMigu3l/cardapio-api/graph/badge.svg?token=6Y7LUJM8PN)](https://codecov.io/gh/Ki3lMigu3l/cardapio-api)


Sistema FullStack para gestão de cardápio de restaurantes. O objetivo foi desenvolver uma API RESTful e uma interface intuitiva para criar, editar, listar e remover itens do cardápio.
<br>
<br>

<div align="center">
  <h2>Tecnologias e Ferramentas utilizadas</h3>
  <br>
  
  [![My Skills](https://skillicons.dev/icons?i=java,spring,mysql,react,tailwind,docker,idea,postman,git&perline=9)](https://skillicons.dev)

  <br>
</div>

<h2 align="center">Backend</h2>

O backend foi desenvolvido com Spring Boot, uma escolha sólida por sua robustez, escalabilidade e forte suporte à construção de APIs RESTful. A estrutura do projeto segue uma arquitetura em camadas, com divisão clara entre controllers, services e repositórios, facilitando a manutenção e os testes. O Spring também oferece integração nativa com JPA e validações, acelerando o desenvolvimento e garantindo boas práticas desde o início.

<br><br>
<div align="center">
  <h2> Documentação Swagger (OpenAPI)</h2>
    <img src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/swagger.png" alt="Swagger" width="50"/>
</div>


<br>
O projeto utiliza Swagger, atualmente conhecido como OpenAPI, que é um framework para documentação de APIs RESTful. Ele gera uma documentação interativa de forma automática, padroniza a descrição dos endpoints e permite testar a API diretamente pela interface.

<div align="center">
  <img src="https://github.com/Ki3lMigu3l/cardapio-api/blob/main/docs/carbon-endpoint-get.png?raw=true" width="800px" />
  <p><em>Endpoint para buscar um item pelo ID.</em></p>
</div>

<h2></h2>

<br>
<div align="center">
Acesse a documentação interativa: 

[![Swagger UI](https://img.shields.io/badge/Swagger_UI-Live-%2385EA2D?logo=swagger)](http://localhost:8080/swagger-ui.html)
</div>

<div align="center">
  
  <img src="https://github.com/Ki3lMigu3l/cardapio-api/blob/main/docs/swagger-endpoints.png" width="800px" />
  <p><em>Documentação interativa dos endpoints de Food</em></p>
  
</div>

<h2></h2>

<div align="center">
  <h3>Testing | JUnit 5</h3>
  <img src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/junit.png" alt="JUnit 5" width="50"/>
</div>


Utilizamos o JUnit5 que é o principal framework para testes unitários em Java. Ele permite automatizar verificações de comportamento, assegura a qualidade do código e ajuda a prevenir regressões durante o desenvolvimento. A cobertura e qualidade do código estão sendo garantidas por meio do uso do JUnit 5, com testes implementados nas principais classes e camadas, como service e controller.

<br>

<div align="center">
  <h3>Testing Manual | Postman</h3>
  
  [![My Skills](https://skillicons.dev/icons?i=postman&perline=8)](https://skillicons.dev)


Postman é uma ferramenta amplamente utilizada para testes de APIs RESTful. Ele permite enviar requisições HTTP de forma prática, validar respostas, organizar coleções de testes e simular diferentes cenários de uso. No projeto, o Postman foi utilizado para testar manualmente os endpoints da API, garantindo que estejam funcionando conforme o esperado e facilitando o processo de depuração e validação durante o desenvolvimento.

  <img src="https://github.com/Ki3lMigu3l/cardapio-api/blob/main/docs/postman-crud.png" width="800px" />
  <p><em>Testes manuais dos endpoints da aplicação com Postman.</em></p>
</div>

<br>

<div align="center">
  <h2>FrontEnd</h2>
</div>

O frontend foi desenvolvido em React.js com Tailwind CSS para interfaces rápidas e responsivas. A navegação é feita com React Router DOM e o consumo da API é centralizado no Axios, garantindo organização e escalabilidade.

<div align="center">
<br>

  <img src="https://github.com/Ki3lMigu3l/cardapio-api/blob/main/docs/home-desktop.png" width="500px" />
  <p><em>Página Inicial do Cardápio</em></p>

<br>

  <img src="https://github.com/Ki3lMigu3l/cardapio-api/blob/main/docs/medium-adminpanel.png" width="500px" />
  <p><em>Painel Admin</em></p>


<br>


  <img src="https://github.com/Ki3lMigu3l/cardapio-api/blob/main/docs/adminpanel-add.png" width="500px" />
  <p><em>Funcionalidade de Adição de Itens ao Cardápio</em></p>


<br>


  <img src="https://github.com/Ki3lMigu3l/cardapio-api/blob/main/docs/adminpanel-update.png" width="500px" />
  <p><em>Funcionalidade de Edição de Itens do Cardápio</em></p>
</div>

<br>

<h2 align="center"> 🐳 Rodando o Projeto</h2>  

Este projeto é totalmente containerizado com Docker e Docker Compose, permitindo iniciar backend, frontend e banco de dados com um único comando, sem necessidade de instalar Java, Node.js ou dependências adicionais localmente.  

### Pré-requisitos  
- Docker instalado

### Como executar  

Na raiz do projeto (onde está o arquivo docker-compose.yml), execute:  

```
docker-compose up --build
```

Esse comando irá:  
- Construir as imagens do frontend, backend e MySQL  
- Inicializar automaticamente todos os containers necessários

  <br>

## Acesso aos Serviços  

Após a inicialização, os serviços estarão disponíveis nos seguintes endereços:  

🔙 **Backend (API - Spring Boot):** http://localhost:8080
<br>
🎨 **Frontend (React + Nginx):** http://localhost
<br>
📘 **Swagger UI (Documentação da API):** http://localhost:8080/swagger-ui.html
<br><br>
O frontend é servido pelo Nginx na porta 80, enquanto o backend opera na porta 8080. 

<br>

<h2>Objetivo</h2>
O projeto tem como finalidade o desenvolvimento de uma API RESTful para gerenciamento de cardápios de restaurantes. A aplicação permite criar, atualizar, remover e consultar itens do cardápio, oferecendo uma solução prática para administradores e uma interface simples e intuitiva para os usuários finais.
