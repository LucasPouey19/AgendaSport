# 3.1 Requisitos Funcionais

| ID     | Requisito | Critério de Aceite |
|---     |---        |---                 |
| RF-001 | O sistema deve permitir que usuários criem uma conta e façam login. | O usuário deve conseguir realizar seu cadastro e, posteriormente, acessar o sistema utilizando suas credenciais. |
| RF-002 | O sistema deve permitir cadastrar quadras esportivas, com informações como nome, endereço, tipo de esporte e horários. | O responsável deve conseguir cadastrar uma quadra informando todos os dados obrigatórios, que devem ser armazenados corretamente no sistema. |
| RF-003 | O usuário deve poder pesquisar e visualizar os locais disponíveis para prática esportiva. | O usuário deve conseguir pesquisar locais e visualizar as informações das quadras disponíveis. |
| RF-004 | O sistema deve permitir consultar os horários disponíveis de cada quadra. | O usuário deve conseguir selecionar uma quadra e visualizar seus horários disponíveis para reserva. |
| RF-005 | O usuário deve poder selecionar uma quadra, data e horário e realizar uma reserva. | O sistema deve permitir a seleção de uma quadra, data e horário disponíveis e confirmar a reserva realizada pelo usuário. |
| RF-006 | O usuário deve poder visualizar suas reservas e, se permitido pelas regras do sistema, cancelar ou alterar uma reserva. | O usuário deve conseguir visualizar suas reservas e realizar o cancelamento ou alteração quando permitido pelas regras definidas pelo sistema. |
| RF-007 | O sistema deve atualizar automaticamente a disponibilidade da quadra após uma reserva ou cancelamento, evitando reservas no mesmo horário. | Após uma reserva ou cancelamento, os horários disponíveis devem ser atualizados automaticamente, impedindo duas reservas para a mesma quadra no mesmo horário. |
| RF-008 | O responsável pelo estabelecimento deve poder cadastrar, alterar e remover quadras e seus horários disponíveis. | O responsável deve conseguir cadastrar, editar e remover quadras e horários, com as alterações refletidas no sistema. |
| RF-009 | Um administrador deve poder consultar e gerenciar os usuários cadastrados. | O administrador deve conseguir visualizar os usuários cadastrados e realizar as ações de gerenciamento permitidas pelo sistema. |
| RF-010 | As operações realizadas na aplicação Web e no aplicativo Mobile devem utilizar a mesma API Back-end e banco de dados, mantendo os dados sincronizados. | As operações realizadas nas plataformas Web e Mobile devem utilizar a mesma API e banco de dados, permitindo que alterações realizadas em uma plataforma sejam refletidas na outra. |

---

# 3.3 Casos de Uso

# 3.3 Casos de Uso

## UC-001: Cadastro e Login de Usuário

- **Ator:** Usuário
- **Pré-condição:** O usuário deve possuir ou desejar criar uma conta.
- **Fluxo Principal:**
  1. O usuário acessa a tela de cadastro ou login.
  2. O usuário informa seus dados.
  3. O sistema valida as informações.
  4. O sistema cria a conta ou autentica o usuário.
  5. O sistema permite o acesso à aplicação.
- **Fluxo Alternativo:**
  - Caso os dados estejam incorretos ou já estejam cadastrados, o sistema informa o erro e solicita uma nova tentativa.

## UC-002: Consultar Locais e Quadras

- **Ator:** Usuário
- **Pré-condição:** O sistema deve possuir locais e quadras cadastrados.
- **Fluxo Principal:**
  1. O usuário acessa a área de locais.
  2. O usuário pesquisa ou seleciona os filtros desejados.
  3. O sistema apresenta os locais e quadras disponíveis.
  4. O usuário seleciona uma quadra para visualizar seus detalhes e horários.
- **Fluxo Alternativo:**
  - Caso nenhum local seja encontrado, o sistema informa que não existem resultados para a pesquisa realizada.

## UC-003: Realizar Reserva de Quadra

- **Ator:** Usuário
- **Pré-condição:** O usuário deve estar autenticado e existir um horário disponível.
- **Fluxo Principal:**
  1. O usuário seleciona uma quadra.
  2. O usuário seleciona a data e o horário desejados.
  3. O sistema verifica a disponibilidade.
  4. O usuário confirma a reserva.
  5. O sistema registra a reserva.
  6. O sistema atualiza a disponibilidade da quadra.
  7. O sistema confirma a reserva.
- **Fluxo Alternativo:**
  - Caso o horário não esteja mais disponível, o sistema informa o usuário e solicita a escolha de outro horário.

## UC-004: Gerenciar Reservas

- **Ator:** Usuário
- **Pré-condição:** O usuário deve estar autenticado e possuir uma reserva cadastrada.
- **Fluxo Principal:**
  1. O usuário acessa a área de suas reservas.
  2. O sistema apresenta as reservas realizadas.
  3. O usuário seleciona uma reserva.
  4. O usuário escolhe visualizar, alterar ou cancelar a reserva.
  5. O sistema processa a ação.
  6. O sistema atualiza a disponibilidade da quadra.
- **Fluxo Alternativo:**
  - Caso a alteração ou cancelamento não seja permitido pelas regras do sistema, o sistema informa que a ação não pode ser realizada.

## UC-005: Gerenciar Quadras e Horários

- **Ator:** Responsável pelo Estabelecimento
- **Pré-condição:** O responsável deve estar autenticado e possuir permissão para gerenciar o estabelecimento.
- **Fluxo Principal:**
  1. O responsável acessa a área de gerenciamento.
  2. O responsável cadastra, altera ou remove uma quadra.
  3. O responsável informa os dados da quadra e seus horários disponíveis.
  4. O sistema valida as informações.
  5. O sistema salva as alterações.
  6. As informações atualizadas ficam disponíveis para consulta e reserva pelos usuários.
- **Fluxo Alternativo:**
  - Caso existam informações inválidas ou obrigatórias não preenchidas, o sistema informa o erro e solicita a correção.

---
---

# 3.4 Fora de Escopo


Os seguintes itens não fazem parte do escopo do projeto:

1. **Pagamento Online**
   - O sistema não realizará pagamentos de reservas, cartões de crédito, PIX ou qualquer outro meio de pagamento.

2. **Sistema de Avaliações e Comentários**
   - O sistema não permitirá que usuários avaliem quadras, estabelecimentos ou deixem comentários sobre os locais.

3. **Reservas de Equipamentos Esportivos**
   - O sistema não permitirá a reserva ou aluguel de materiais e equipamentos esportivos, como bolas, raquetes ou coletes.

4. **Sistema de Geolocalização em Tempo Real**
   - O sistema não utilizará GPS ou rastreamento em tempo real para localizar usuários ou acompanhar seus deslocamentos.

5. **Integração com Redes Sociais**
   - O sistema não possuirá integração com redes sociais para compartilhamento de reservas, login social ou publicação automática de atividades.