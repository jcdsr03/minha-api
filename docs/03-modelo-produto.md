# Modelo de Dados — Produto

Exemplo de resposta (GET/POST/PUT):
{
  "id": 1,
  "nome": "Chaveiro Rinoceronte",
  "preco": 29.90,
  "disponivel": true,
  "criadoEm": "2025-09-16T12:00:00Z",
  "atualizadoEm": "2025-09-16T12:05:00Z"
}

Regras:
- Obrigatórios no POST: `nome` (string min 2), `preco` (> 0).
- O sistema gera: `id`, `criadoEm`, `atualizadoEm`.
- `disponivel` padrão: `true` (pode ser enviado no POST).
