# 6.3 Registro de Riscos

<!-- Ao menos 5 riscos identificados -->

| ID | Risco | Probabilidade (1-3) | Impacto (1-3) | Mitigação |
|---|---|---:|---:|---|
| R-01 | Atraso no desenvolvimento das funcionalidades previstas | 3 | 3 | Dividir as tarefas em etapas menores, acompanhar o cronograma e priorizar as funcionalidades essenciais. |
| R-02 | Problemas de integração entre Web, Mobile, Back-end e banco de dados | 2 | 3 | Definir previamente as interfaces da API, realizar testes de integração e manter uma comunicação constante entre os responsáveis. |
| R-03 | Indisponibilidade ou falhas no banco de dados | 2 | 3 | Realizar testes, utilizar validações no sistema e manter backups dos dados durante o desenvolvimento. |
| R-04 | Falhas de autenticação ou acesso indevido aos dados | 2 | 3 | Utilizar JWT, controlar permissões por tipo de usuário e validar as requisições realizadas pela API. |
| R-05 | Alterações nos requisitos durante o desenvolvimento | 3 | 2 | Registrar as mudanças, avaliar seu impacto no cronograma e priorizar alterações de acordo com a necessidade do projeto. |

---

# 6.4 Matriz de Riscos (3×3)

<!-- Posicione cada risco (R-01, R-02...) na célula correspondente -->

| Impacto \ Probabilidade | Baixa (1) | Média (2) | Alta (3) |
|---|---|---|---|
| **Alto (3)** | — | R-02, R-03, R-04 | R-01 |
| **Médio (2)** | — | — | R-05 |
| **Baixo (1)** | — | — | — |
