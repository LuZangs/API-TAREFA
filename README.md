# Criar
curl -X POST http://localhost:8080/api/tarefas \
  -H "Content-Type: application/json" \
  -d '{"nome":"Estudar Spring","dataEntrega":"2025-09-15","responsavel":"Luciane"}'

# Listar
curl http://localhost:8080/api/tarefas

# Buscar por ID
curl http://localhost:8080/api/tarefas/1

# Atualizar
curl -X PUT http://localhost:8080/api/tarefas/1 \
  -H "Content-Type: application/json" \
  -d '{"nome":"Estudar Spring (atualizado)","dataEntrega":"2025-09-20","responsavel":"Luciane"}'

# Remover
curl -X DELETE http://localhost:8080/api/tarefas/1
