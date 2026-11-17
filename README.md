# FATEC Santos - ILP-530

Linguagem de Programação III - 5º semestre

## Projeto 1 - Importação de dados
Importação, validação e persistência de arquivos CSV em PostgreSQL.

## Projeto 2 - API REST
Desenvolvimento de uma aplicação Web integrada ao banco de dados.

## Avaliação
- Primeiro bimestre: atividades 01 a 10.
- Segundo bimestre: atividades 11 a 20.
- Cada atividade vale 1,0 ponto.

## Prazo final
07/12/2026.

Descrição:

Projeto 1 — CSV para Banco de Dados
Primeiro bimestre — Atividades 1 a 10
Nº	Atividade	 - Tecnologia principal
1	Preparar o ambiente e criar um projeto que compile e execute - Java 25, Maven, Spring Boot
2	Analisar as 25 colunas do CSV e modelar a classe AtaqueCibernetico - Java, POO
3	Ler corretamente o arquivo CSV e contar os registros - Java I/O, Apache Commons CSV
4	Converter os registros do CSV em objetos Java	Classes, - construtores, encapsulamento
5	Validar os dados e tratar exceções -	Interfaces, classes abstratas
6	Configurar PostgreSQL e mapear as classes para tabelas -	PostgreSQL, JPA, Hibernate
7	Persistir os registros no banco e conferir por SQL -	Spring Data JPA
8	Tratar falhas de importação e gerar relatório de erros -	Exceptions, logs
9	Impedir duplicidades ao executar novamente a importação -	SQL, idempotência
10	Testar o processo completo e documentar sua execução -	JUnit, Maven, Git
Entrega: aplicação Java que importa o arquivo cybersecurity_attacks.csv, valida os registros e os armazena no PostgreSQL.


Projeto 2 — API REST e Aplicação Web
Segundo bimestre — Atividades 11 a 20
Nº	Atividade	 - Tecnologia principal
11	Criar uma aplicação que responda a uma requisição HTTP - Spring Boot, REST
12	Conectar a API ao banco e retornar um registro real em JSON -	JPA, JSON
13	Implementar operações CRUD, incluindo exclusão lógica -	HTTP, REST, JPA
14	Criar consultas com filtros combinados - Spring Data JPA, SQL
15	Implementar paginação e estatísticas por tipo de ataque -	Pageable, SQL
16	Implementar autenticação e autorização básica -	Spring Security
17	Tratar erros com códigos HTTP adequados -	Exceptions, HTTP
18	Gerar relatórios utilizando processamento assíncrono	Threads, CompletableFuture
19	Internacionalizar mensagens e criar uma página Web que consuma a API -	Java i18n, HTML, JavaScript
20	Integrar, testar, documentar e demonstrar os dois projetos -	Java, Maven, Git, OpenAPI
Entrega: aplicação Web com API REST capaz de consultar, filtrar e gerenciar os dados armazenados pelo primeiro projeto.
