🧠 Feature Design & Technical Analysis Workflow
Template para orquestração entre agentes especializados

🔹 FASE 1 – Planejamento, PRD e Arquitetura Inicial (Agente 1)
📥 Input:
Nome da feature:

Problema a resolver:

Objetivo de negócio:

Stakeholders envolvidos:

📤 Output:
yaml
Copiar
Editar
PRD:
  - User Stories (BDD):
      - Given:
      - When:
      - Then:
  - Requisitos Funcionais:
  - Requisitos Não-Funcionais:
  - Métricas de sucesso:
  - Restrições:
  - Critérios de aceitação:

RFC:
  - Contexto técnico atual:
  - Soluções possíveis:
    - Solução A:
    - Solução B:
  - Trade-offs:
  - Recomendação:

Arquitetura inicial:
  - Componentes envolvidos:
  - Fluxo básico de dados:
  - Tecnologias sugeridas:
🔹 FASE 2 – Validação Lógica (Agente 2)
📥 Input:
Regras de negócio do PRD

Fluxos condicionais dos stories

📤 Output:
yaml
Copiar
Editar
Lógica formal:
  - Predicados identificados:
  - Expressões booleanas:
  - Tabelas de verdade (se necessário):

Simplificações:
  - Regras redundantes removidas:
  - Fluxos alternativos otimizados:

Erros ou contradições detectadas:
  - [x] Inconsistência lógica
  - [ ] Fluxo ambíguo
  - [ ] Falta de cobertura
🔹 FASE 3 – Modelagem de Entidades e Fluxo de Dados (Agente 3)
📥 Input:
User stories + regras validadas

RFC técnica

📤 Output:
yaml
Copiar
Editar
Entidades:
  - Nome: [Ex: Pedido]
    - Atributos:
        - id: string (PK)
        - status: enum
        - valor: float

Relacionamentos:
  - Pedido -> Cliente [1:N]
  - Pedido -> Produto [N:N]

Fluxo de dados:
  - Entrada: [API, UI]
  - Processamento: [Serviço A → B]
  - Armazenamento: [Banco relacional]
  - Saída: [Webhook, export, relatório]

Eventos:
  - pedido_criado
  - pagamento_confirmado
🔹 FASE 4 – Testes Profissionais (Agente 4)
📥 Input:
Critérios de aceitação

Estrutura de dados e entidades

Regras validadas

📤 Output:
yaml
Copiar
Editar
Casos de teste:
  - TC001: Cenário de sucesso
  - TC002: Falha por input inválido
  - TC003: Fluxo alternativo
  - TC004: Teste de regressão

Testes automatizáveis:
  - Framework sugerido: [Vitest, Cypress, etc.]
  - Tipo: [Unitário, Integração, E2E]
  - Cobertura esperada: 85%

Riscos e gaps:
  - Falta de testes de borda em fluxo X
  - Cenário não coberto: [XYZ]
🔹 FASE 5 – Otimização de Processo (Agente 5 – Programação Linear)
📥 Input:
Backlog de tarefas + estimativa de esforço

Recursos disponíveis (tempo, devs, orçamento)

Objetivo (maximizar entrega, minimizar custo, etc.)

📤 Output:
yaml
Copiar
Editar
Modelo de PL:
  - Variáveis:
      - x = tempo dev A
      - y = tempo dev B
  - Função objetivo:
      - max(5x + 3y)
  - Restrições:
      - x + y <= 40
      - x >= 10, y >= 10

Resultado ótimo:
  - x = 30h
  - y = 10h
  - Valor total = 180 pontos

Trade-offs:
  - Ganho marginal por hora adicional: X
  - Sugestão de replanejamento: mover tarefa Y para depois da sprint
🔁 FASE FINAL – Handoff / Execução
📤 Entregáveis consolidados:
yaml
Copiar
Editar
- PRD validado
- Arquitetura lógica
- Modelo de dados
- Casos de teste prontos
- Prioridade das tarefas
- Alocação ótima de recursos
- Riscos mapeados