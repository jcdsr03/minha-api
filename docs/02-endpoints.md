# Endpoints REST (rascunho)

Recurso: **Produto**

- GET    /produtos           → Lista paginada de produtos
- POST   /produtos           → Cria um produto
- GET    /produtos/{id}      → Detalha um produto
- PUT    /produtos/{id}      → Atualiza integralmente um produto
- DELETE /produtos/{id}      → Remove um produto

Observações:
- `PUT` é idempotente (mesmo corpo repetido mantém o mesmo estado).
- `POST` cria e retorna 201 com o recurso novo.
- `GET /produtos` aceitará `page` e `limit` (paginação).
