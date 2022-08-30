# TDD Domínio ORM e Autorizações
Implementação das funcionalidades necessárias para que os testes escritos utilizando o JUnit5 sejam cobertos. Este é um sistema de catálogo de filmes que somente o usuário MEMBER pode inserir avaliação.
Exercício desenvolvido durante o Bootcamp Spring React da [DevSuperior](https://devsuperior.com.br/) como requisito obrigatório para obtenção do certificado.

## Especificações
O sistema MovieFlix consiste em um banco de filmes, os quais podem ser listados e avaliados pelos usuários. Usuários podem ser visitantes (VISITOR) e membros (MEMBER). Apenas usuários membros podem inserir avaliações no sistema.

Ao acessar o sistema, o usuário deve fazer seu login. Apenas usuários logados podem navegar nos filmes. Logo após fazer o login, o usuário vai para a listagem de filmes, que mostra os filmes de forma paginada, ordenados alfabeticamente por título. O usuário pode filtrar os filmes por gênero.

Ao selecionar um filme da listagem, é mostrada uma página de detalhes, onde é possível ver todas informações do filme, e também suas avaliações. Se o usuário for MEMBER, ele pode ainda registrar uma avaliação nessa tela.

Um usuário possui nome, email e senha, sendo que o email é seu nome de usuário. Cada filme possui um título, subtítulo, uma imagem, ano de lançamento, sinopse, e um gênero. Os usuários membros podem registrar avaliações para os filmes. Um mesmo usuário membro pode deixar mais de uma avaliação para o mesmo filme.


## Competências

  - Domínio e ORM
    - Implementação de um modelo de domínio complexo (projeto DSLearn)
    -Instanciação (seed) de um modelo de domínio com SQL
  - Autorizações
    - Autorização customizada em nível de serviço
    - Conteúdo customizado para o usuário logado
    - Refresh token
    - Pré-autorização de métodos


## Requisitos para aprovação
  - Implementar o modelo conceitual proposto, com seed do banco de dados.
  - Incluir a infraestrutura de exceções, validação e segurança ao projeto.
  - Implementar o endpoint mostrado abaixo.
  - Seu seed deve conter dois usuários:
      - Usuário somente com perfil VISITOR:
        - email: bob@gmail.com
        - senha: 123456
      - Usuário com perfil MEMBER:
        - email: ana@gmail.com
        - senha: 123456


### Modelo conceitual
![Modelo Conceitual](https://github.com/vanessa-maganhoto/assets/blob/main/cap5-bds-movieflix/modelo-conceitual.png)

## Tecnologias utilizadas
### Back end
- Java
- Spring Boot
- JPA / Hibernate
- Maven
- JUnit5
- Postman
- JWT

## Como executar o projeto

### Back end
Pré-requisitos: Java 11

```bash
# clonar repositório
git clone git@github.com:vanessa-maganhoto/bds05-desafio-dominio-orm-autorizacoes-TDD.git

# executar o projeto
./mvnw spring-boot:run
```

## Autor

Vanessa Matos

https://www.linkedin.com/in/vanessaammatos



