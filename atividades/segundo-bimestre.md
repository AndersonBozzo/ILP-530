# 2º bimestre — Projeto 2 — API REST e aplicação Web

Prazo final: 07/12/2026. Cada atividade vale 1,0 ponto.

## 11 — Criar aplicação HTTP

**Pesquisar:** Spring Boot, REST.

**Desenvolver:** Implementar GET /api/v1/health retornando HTTP 200 e JSON {"status":"UP"}.

**Comprovar:** Executar localmente e verificar status e corpo.

**Verificação prevista:** Teste HTTP automatizável.

## 12 — Integrar API ao banco

**Pesquisar:** JPA, JSON.

**Desenvolver:** Conectar ao mesmo banco do projeto 1 e implementar GET /api/v1/events/{id}.

**Comprovar:** Retornar um registro existente em JSON, coerente com consulta SQL.

**Verificação prevista:** Teste HTTP e banco.

## 13 — Implementar CRUD

**Pesquisar:** HTTP, REST, JPA.

**Desenvolver:** Implementar GET e POST /api/v1/events, PATCH e DELETE /api/v1/events/{id}; DELETE deve realizar exclusão lógica.

**Comprovar:** Demonstrar criação, leitura, atualização e exclusão lógica; registro excluído não aparece em consultas normais.

**Verificação prevista:** Teste HTTP e banco de teste.

## 14 — Criar filtros combinados

**Pesquisar:** Spring Data JPA, SQL.

**Desenvolver:** Permitir filtros combináveis em GET /api/v1/events: attackType, severity, sourceIp, from e to (datas ISO-8601 locais, sem fuso).

**Comprovar:** Testar filtros isolados e combinados e ausência de resultados, comparando com SQL.

**Verificação prevista:** Teste HTTP com dados conhecidos.

## 15 — Paginar e gerar estatísticas

**Pesquisar:** Pageable, SQL.

**Desenvolver:** Usar page (início em zero) e size em GET /api/v1/events; expor GET /api/v1/statistics/attacks para contagem por tipo.

**Comprovar:** Página respeita tamanho solicitado; estatísticas conferem com SQL e ignoram exclusões lógicas.

**Verificação prevista:** Teste HTTP e SQL.

## 16 — Autenticar e autorizar

**Pesquisar:** Spring Security.

**Desenvolver:** Usar autenticação básica HTTP para ambiente local; distinguir perfil de leitura e escrita. Não enviar senhas ao Git.

**Comprovar:** Usuário de leitura consulta, mas não altera; usuário de escrita autorizado altera; sem autenticação recebe 401 em recurso protegido.

**Verificação prevista:** Teste HTTP com credenciais de teste.

## 17 — Tratar erros HTTP

**Pesquisar:** Exceções, HTTP.

**Desenvolver:** Padronizar respostas de erro para requisição inválida, falta de autenticação, falta de permissão e recurso inexistente.

**Comprovar:** Demonstrar HTTP 400, 401, 403 e 404, sem stack trace nem dados sensíveis na resposta.

**Verificação prevista:** Teste HTTP.

## 18 — Gerar relatório assíncrono

**Pesquisar:** Threads, CompletableFuture ou ExecutorService.

**Desenvolver:** Executar geração de relatório em tarefa assíncrona e permitir acompanhar conclusão ou falha, sem bloquear a requisição até terminar.

**Comprovar:** Demonstrar execução em outra thread, resultado final e tratamento de falha; documentar como solicitar e consultar.

**Verificação prevista:** Teste de concorrência e demonstração.

## 19 — Internacionalizar e criar página Web

**Pesquisar:** Java i18n, HTML, JavaScript.

**Desenvolver:** Usar recursos de mensagens PT-BR e EN com seleção de idioma; criar página com tabela e filtros que consulte efetivamente a API via HTTP.

**Comprovar:** Demonstrar mudança de mensagens e consulta real pela interface no navegador.

**Verificação prevista:** Teste de idioma e demonstração da interface.

## 20 — Integrar, testar e documentar

**Pesquisar:** Java, Maven, Git, OpenAPI.

**Desenvolver:** Executar os dois projetos integrados; criar testes próprios, instruções reproduzíveis e descrição OpenAPI dos endpoints.

**Comprovar:** Demonstrar importação, consulta e operações web; builds passam e equipe explica seu código.

**Verificação prevista:** Build, integração e validação humana.
