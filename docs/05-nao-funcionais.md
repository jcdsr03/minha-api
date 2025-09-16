# Requisitos Não-Funcionais (NFRs)

- Autenticação: JWT Bearer em Authorization (obrigatório para POST/PUT/DELETE; GETs públicos).
- Autorização: papel `admin` para mutações (futuro).
- Validação: schema (ex.: Zod) garantindo `nome` e `preco`.
- Logs: access log (morgan) + error log estruturado (JSON).
- Testes: integração (Supertest) para todos os endpoints; unitários para validação.
- Documentação: OpenAPI 3.0 + Swagger UI em `/docs`.
- Paginação: `page` (default 1), `limit` (default 20, máx 100) em `GET /produtos`.
- Versionamento: prefixo `/v1` para rotas.
- Padrão de datas: ISO-8601 (UTC). Moeda trafega como número (BRL fica para o front).
