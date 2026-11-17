# Como iniciar

Instale JDK 25 e Maven 3.9.x. Git já deve estar instalado. Cada projeto tem seu próprio pom.xml.

```bash
cd projeto-01-importacao
mvn verify
mvn spring-boot:run
```

Em outro terminal, a partir da raiz:

```bash
cd projeto-02-api
mvn verify
mvn spring-boot:run
```

Os esqueletos apenas inicializam o Spring; as funcionalidades são as atividades dos alunos. O CSV está em `dados/cybersecurity_attacks.csv` (a partir de cada projeto: `../dados/cybersecurity_attacks.csv`). O arquivo original contém 25 colunas e 40.000 registros de dados; campos entre aspas podem conter quebras de linha.

Adicione JPA e driver PostgreSQL nas etapas correspondentes. Use o mesmo banco nos dois projetos, credenciais por variáveis de ambiente (por exemplo SPRING_DATASOURCE_URL, SPRING_DATASOURCE_USERNAME e SPRING_DATASOURCE_PASSWORD), nunca senhas no Git. Use banco separado para testes. API local, sem necessidade de hospedagem externa.

Consulte os enunciados em `atividades/`. O GitHub Actions existente roda Maven verify em cada projeto e não atribui notas. Quando os testes exigirem PostgreSQL, será necessário configurar o ambiente de teste/CI com banco adequado. A equipe deve compreender o código mesmo quando utilizar IA.
