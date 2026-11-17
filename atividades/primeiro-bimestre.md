# 1º bimestre — Projeto 1 — CSV para banco de dados

Prazo final: 07/12/2026. Cada atividade vale 1,0 ponto.

## 01 — Preparar o ambiente

**Pesquisar:** Java 25, Maven, Spring Boot.

**Desenvolver:** Executar java -version, mvn -version e mvn verify no projeto 1; iniciar a aplicação.

**Comprovar:** Build e inicialização sem erro; teste inicial passa.

**Verificação prevista:** Build e teste automatizáveis; versão e execução demonstráveis.

## 02 — Modelar AtaqueCibernetico

**Pesquisar:** Java, POO.

**Desenvolver:** Representar as 25 colunas do CSV em uma classe AtaqueCibernetico, com tipos coerentes e encapsulamento.

**Comprovar:** Mostrar correspondência das 25 colunas com atributos; justificar tipos e tratamento de valores ausentes.

**Verificação prevista:** Revisão de código/modelo.

## 03 — Ler o CSV

**Pesquisar:** Java I/O, Apache Commons CSV.

**Desenvolver:** Ler o cabeçalho e os registros mediante parser CSV, inclusive campos entre aspas, vírgulas e quebras de linha internas.

**Comprovar:** Contar 40.000 registros de dados do arquivo original; não contar cabeçalho nem linhas físicas como registros.

**Verificação prevista:** Teste com arquivo original e amostra pequena.

## 04 — Converter registros em objetos

**Pesquisar:** Classes, construtores, encapsulamento.

**Desenvolver:** Converter registros em instâncias de AtaqueCibernetico; preservar os campos e tratar valores ausentes.

**Comprovar:** Demonstrar conversão de registros válidos e comparar valores com a fonte.

**Verificação prevista:** JUnit com amostras.

## 05 — Validar dados e tratar exceções

**Pesquisar:** Interfaces, classes abstratas, exceções.

**Desenvolver:** Criar e usar uma interface e uma classe abstrata próprias no mecanismo de validação; validar campos essenciais, portas (0 a 65535) e tipos numéricos/data. Não rejeitar campos opcionais apenas por estarem vazios.

**Comprovar:** Mostrar casos válidos e inválidos, implementação concreta e tratamento de exceções sem encerrar toda a importação.

**Verificação prevista:** JUnit e revisão de código.

## 06 — Configurar PostgreSQL e mapear entidades

**Pesquisar:** PostgreSQL, JPA, Hibernate.

**Desenvolver:** Adicionar dependências e configurar banco via variáveis de ambiente; mapear entidade a tabela com chave primária.

**Comprovar:** Demonstrar tabela criada ou mapeada e conexão real ao PostgreSQL, sem senha no Git.

**Verificação prevista:** Teste de integração e revisão.

## 07 — Persistir registros

**Pesquisar:** Spring Data JPA, SQL.

**Desenvolver:** Importar registros válidos para o PostgreSQL.

**Comprovar:** Consulta SQL confirma dados importados; total persistido corresponde aos aceitos da primeira importação em banco vazio.

**Verificação prevista:** Teste de integração e consulta SQL.

## 08 — Tratar falhas e gerar relatório

**Pesquisar:** Exceções, logs, Java I/O.

**Desenvolver:** Registrar totais lidos, aceitos e rejeitados e motivos de rejeição em relatório de saída; não expor payload ou dados pessoais nos logs.

**Comprovar:** Amostra com erro gera relatório e mantém processamento dos registros válidos; lidos = aceitos + rejeitados.

**Verificação prevista:** Teste com amostra controlada.

## 09 — Impedir duplicidades

**Pesquisar:** SQL, idempotência.

**Desenvolver:** Definir e documentar estratégia para reimportação do mesmo arquivo; não eliminar registros distintos apenas por terem mesmo IP.

**Comprovar:** Executar duas vezes em banco de teste: a segunda não aumenta a quantidade de registros do mesmo arquivo.

**Verificação prevista:** Teste de integração.

## 10 — Testar e documentar

**Pesquisar:** JUnit, Maven, Git.

**Desenvolver:** Criar testes próprios e documentar configuração, importação e verificação por SQL.

**Comprovar:** mvn verify passa; outra pessoa consegue repetir a importação seguindo instruções.

**Verificação prevista:** Build automatizado e revisão do README.
