# Status Codes e Erros

- 200 OK              → Sucesso (GET/PUT)
- 201 Created         → Recurso criado (POST)
- 204 No Content      → Remoção sem corpo (DELETE)
- 400 Bad Request     → Validação falhou (payload inválido)
- 401 Unauthorized    → Falta token
- 403 Forbidden       → Sem permissão para a ação
- 404 Not Found       → Recurso não existe
- 409 Conflict        → Conflito de regra (ex.: nome único)
- 422 Unprocessable   → Dados válidos sintaticamente, mas quebram regra de negócio
- 500 Internal Error  → Erro inesperado

Formato de erro (JSON):
{
  "error": "ValidationError",
  "message": "preco deve ser positivo",
  "details": { "preco": ["must be > 0"] }
}
