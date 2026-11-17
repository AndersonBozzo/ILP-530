# FATEC Santos - ILP-530

Linguagem de Programação III - 5º semestre

**Prazo final: 07/12/2026.** Cada atividade vale 1,0 ponto. Atividades 1–10: primeiro bimestre; 11–20: segundo bimestre.

## Materiais

- [Instruções técnicas](INSTRUCOES.md)
- [Base de dados CSV](dados/cybersecurity_attacks.csv)
- [Critérios de avaliação](atividades/criterios.md)

## Projeto 1 — CSV para banco de dados

Aplicação Java que importa, valida e persiste registros no PostgreSQL.

[Enunciados detalhados — 1º bimestre](atividades/primeiro-bimestre.md)

| Nº | Atividade | Tecnologia principal |
|---|---|---|
| 01 | Preparar o ambiente | Java 25, Maven, Spring Boot |
| 02 | Modelar AtaqueCibernetico | Java, POO |
| 03 | Ler o CSV | Java I/O, Apache Commons CSV |
| 04 | Converter registros em objetos | Classes, construtores, encapsulamento |
| 05 | Validar dados e tratar exceções | Interfaces, classes abstratas, exceções |
| 06 | Configurar PostgreSQL e mapear entidades | PostgreSQL, JPA, Hibernate |
| 07 | Persistir registros | Spring Data JPA, SQL |
| 08 | Tratar falhas e gerar relatório | Exceções, logs, Java I/O |
| 09 | Impedir duplicidades | SQL, idempotência |
| 10 | Testar e documentar | JUnit, Maven, Git |

## Projeto 2 — API REST e aplicação Web

Aplicação Web que consulta, filtra e gerencia os dados do primeiro projeto.

[Enunciados detalhados — 2º bimestre](atividades/segundo-bimestre.md)

| Nº | Atividade | Tecnologia principal |
|---|---|---|
| 11 | Criar aplicação HTTP | Spring Boot, REST |
| 12 | Integrar API ao banco | JPA, JSON |
| 13 | Implementar CRUD | HTTP, REST, JPA |
| 14 | Criar filtros combinados | Spring Data JPA, SQL |
| 15 | Paginar e gerar estatísticas | Pageable, SQL |
| 16 | Autenticar e autorizar | Spring Security |
| 17 | Tratar erros HTTP | Exceções, HTTP |
| 18 | Gerar relatório assíncrono | Threads, CompletableFuture ou ExecutorService |
| 19 | Internacionalizar e criar página Web | Java i18n, HTML, JavaScript |
| 20 | Integrar, testar e documentar | Java, Maven, Git, OpenAPI |

## Avaliação

O GitHub Actions existente verifica build e testes, mas não calcula notas. A avaliação das atividades segue os critérios publicados e a validação do docente. IA é permitida; os alunos devem compreender e explicar o código.
