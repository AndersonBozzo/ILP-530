# Critérios de avaliação

Cada atividade vale até 1,0 ponto. Proposta de régua: 1,0 = critério integralmente demonstrado; 0,5 = parcialmente demonstrado, com evidência funcional; 0,0 = não demonstrado. Cada bimestre soma até 10,0. A nota oficial depende de validação docente.

| Nº | Evidência para 1,0 | Verificação prevista |
|---|---|---|
| 01 | Build e inicialização sem erro; teste inicial passa. | Build e teste automatizáveis; versão e execução demonstráveis. |
| 02 | Mostrar correspondência das 25 colunas com atributos; justificar tipos e tratamento de valores ausentes. | Revisão de código/modelo. |
| 03 | Contar 40.000 registros de dados do arquivo original; não contar cabeçalho nem linhas físicas como registros. | Teste com arquivo original e amostra pequena. |
| 04 | Demonstrar conversão de registros válidos e comparar valores com a fonte. | JUnit com amostras. |
| 05 | Mostrar casos válidos e inválidos, implementação concreta e tratamento de exceções sem encerrar toda a importação. | JUnit e revisão de código. |
| 06 | Demonstrar tabela criada ou mapeada e conexão real ao PostgreSQL, sem senha no Git. | Teste de integração e revisão. |
| 07 | Consulta SQL confirma dados importados; total persistido corresponde aos aceitos da primeira importação em banco vazio. | Teste de integração e consulta SQL. |
| 08 | Amostra com erro gera relatório e mantém processamento dos registros válidos; lidos = aceitos + rejeitados. | Teste com amostra controlada. |
| 09 | Executar duas vezes em banco de teste: a segunda não aumenta a quantidade de registros do mesmo arquivo. | Teste de integração. |
| 10 | mvn verify passa; outra pessoa consegue repetir a importação seguindo instruções. | Build automatizado e revisão do README. |
| 11 | Executar localmente e verificar status e corpo. | Teste HTTP automatizável. |
| 12 | Retornar um registro existente em JSON, coerente com consulta SQL. | Teste HTTP e banco. |
| 13 | Demonstrar criação, leitura, atualização e exclusão lógica; registro excluído não aparece em consultas normais. | Teste HTTP e banco de teste. |
| 14 | Testar filtros isolados e combinados e ausência de resultados, comparando com SQL. | Teste HTTP com dados conhecidos. |
| 15 | Página respeita tamanho solicitado; estatísticas conferem com SQL e ignoram exclusões lógicas. | Teste HTTP e SQL. |
| 16 | Usuário de leitura consulta, mas não altera; usuário de escrita autorizado altera; sem autenticação recebe 401 em recurso protegido. | Teste HTTP com credenciais de teste. |
| 17 | Demonstrar HTTP 400, 401, 403 e 404, sem stack trace nem dados sensíveis na resposta. | Teste HTTP. |
| 18 | Demonstrar execução em outra thread, resultado final e tratamento de falha; documentar como solicitar e consultar. | Teste de concorrência e demonstração. |
| 19 | Demonstrar mudança de mensagens e consulta real pela interface no navegador. | Teste de idioma e demonstração da interface. |
| 20 | Demonstrar importação, consulta e operações web; builds passam e equipe explica seu código. | Build, integração e validação humana. |

## Limites da automação

O workflow atual executa os testes presentes nos projetos. Não é um corretor das 20 atividades. Testes oficiais independentes serão necessários para atribuir notas automaticamente. Revisão de código, documentação e demonstração continuam sob responsabilidade docente.
