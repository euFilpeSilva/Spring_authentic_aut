# Projeto Spring Boot com Autenticação Básica

Este é um projeto Spring Boot com autenticação básica implementada usando Spring Security. O projeto utiliza JPA (Java Persistence API) para a camada de persistência e Lombok para reduzir a verbosidade do código.

## Pré-requisitos
Antes de executar este projeto, verifique se você tem os seguintes pré-requisitos instalados:

Java Development Kit (JDK) versão 8 ou superior
Maven (https://maven.apache.org/) instalado
MySQL Server (https://www.mysql.com/) instalado
Certifique-se de ter criado um banco de dados no MySQL para o projeto.

### Configuração do Banco de Dados
Abra o arquivo application.properties localizado na pasta src/main/resources.
Substitua os valores de spring.datasource.url, spring.datasource.username e spring.datasource.password pelas informações do seu banco de dados MySQL.

###### Ex:

- spring.datasource.url=jdbc:mysql://localhost:3306/meu_banco_de_dados
- spring.datasource.username=seu_usuario
- spring.datasource.password=sua_senha




## Passo a passo

1 - Clonar o repositório `git clone https://github.com/danileao/spring_auth_youtube.git`

2 - Rodar `mvn clean install` para instalar as dependências

3 - Rodar `mvn spring-boot:run` para subir a aplicação

4 - A aplicação estará disponível na port `8080`

### Endpoints
O projeto possui os seguintes endpoints:

- /api/user/create: Cria um novo usuário com nome de usuário e senha fornecidos.
- /api/users/role: Vincula roles a um usuario.
- /api/products: Lista todos os produtos cadastrados no sistema.

### Tecnologias Utilizadas
- Spring Boot: Framework Java para criar aplicativos web.
- Spring Security: Framework de segurança para autenticação e controle de acesso.
- JPA (Java Persistence API): API de persistência para mapeamento objeto-relacional.
- Lombok: Biblioteca Java para reduzir a verbosidade do código.
- MySQL: Banco de dados relacional utilizado.
- Postman pra fazer os testes com os endpoints.
