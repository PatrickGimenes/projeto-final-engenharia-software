# Projeto Final - Engenharia de software

## Equipe

* Gustavo — Dev
* Patrick — Dev
* Vicente — Product Owner (PO)

---

# Tema do Projeto

Sistema para barbearia com:

* Agendamento online
* Gestão de estoque
* Controle financeiro
* Gestão de clientes
* Controle de acesso

---

# Atores do Sistema

## Cliente

Usuário que realiza agendamentos e acompanha seus atendimentos.

## Barbeiro

Responsável pelos atendimentos e controle de produtos utilizados.

## Administrador

Responsável pela gestão completa do sistema.

---

# User Stories

# Cliente

| ID  | User Story                                                                                                        |
| --- | ----------------------------------------------------------------------------------------------------------------- |
| C1  | Como um cliente, eu quero agendar um horário online para evitar filas e garantir atendimento.                     |
| C2  | Como um cliente, eu quero visualizar os horários disponíveis para escolher o melhor horário para mim.             |
| C3  | Como um cliente, eu quero usar inteligência artificial para sugerir cortes baseados no formato do meu rosto.      |
| C4  | Como um cliente, eu quero experimentar cortes virtualmente usando realidade aumentada antes do atendimento.       |
| C5  | Como um cliente, eu quero um assistente virtual com voz para marcar meus horários por comando de áudio.           |
| C6  | Como um cliente, eu quero receber recomendações de barba e cabelo baseadas nas tendências dos famosos do momento. |
| C7  | Como um cliente, eu quero desbloquear conquistas e medalhas por frequência na barbearia.                          |
| C8  | Como um cliente, eu quero receber notificações sobre promoções para aproveitar descontos.                         |
| C9  | Como um cliente, eu quero cancelar ou remarcar um horário para ter mais flexibilidade.                            |
| C10 | Como um cliente, eu quero criar uma conta no sistema para acompanhar meus agendamentos.                           |

---

# Barbeiro

| ID | User Story                                                                                                               |
| -- | ------------------------------------------------------------------------------------------------------------------------ |
| B1 | Como um barbeiro, eu quero visualizar o histórico do cliente para oferecer um atendimento personalizado.                 |
| B2 | Como um barbeiro, eu quero visualizar minha agenda diária para organizar meus atendimentos.                              |
| B3 | Como um barbeiro, eu quero registrar o uso de produtos durante os atendimentos para atualizar o estoque automaticamente. |
| B4 | Como um barbeiro, eu quero realizar login no sistema para acessar minha agenda.                                          |

---

# Administrador

| ID  | User Story                                                                                                               |
| --- | ------------------------------------------------------------------------------------------------------------------------ |
| A1  | Como um administrador, eu quero cadastrar produtos no estoque para controlar os itens disponíveis.                       |
| A2  | Como um administrador, eu quero atualizar a quantidade de produtos para manter o estoque correto.                        |
| A3  | Como um administrador, eu quero receber alertas de estoque baixo para evitar falta de produtos.                          |
| A4  | Como um administrador, eu quero cadastrar clientes para manter um histórico de atendimentos.                             |
| A5  | Como um administrador, eu quero enviar lembretes automáticos de agendamento para reduzir faltas.                         |
| A6  | Como um administrador, eu quero cadastrar serviços e duração dos atendimentos para melhorar o controle dos agendamentos. |
| A7  | Como um administrador, eu quero registrar entradas e saídas financeiras para controlar o caixa.                          |
| A8  | Como um administrador, eu quero gerar relatórios financeiros para analisar o faturamento da barbearia.                   |
| A9  | Como um administrador, eu quero visualizar os serviços mais vendidos para apoiar decisões de negócio.                    |
| A10 | Como um administrador, eu quero registrar formas de pagamento para organizar as vendas.                                  |
| A11 | Como um administrador, eu quero prever o faturamento do mês utilizando aprendizado de máquina.                           |
| A12 | Como um administrador, eu quero que o sistema preveja automaticamente os produtos que faltarão no estoque usando IA.     |
| A13 | Como um administrador, eu quero controlar os níveis de acesso dos usuários para garantir segurança.                      |

---

# Priorização MoSCoW

# Must Have (M)

| ID  | História                                |
| --- | --------------------------------------- |
| C1  | Agendar horário online                  |
| C2  | Visualizar horários disponíveis         |
| C9  | Cancelar ou remarcar horário            |
| B2  | Visualizar agenda diária                |
| C10 | Criar conta no sistema                  |
| A1  | Cadastrar produtos no estoque           |
| A2  | Atualizar quantidade de produtos        |
| A7  | Registrar entradas e saídas financeiras |
| A13 | Controlar níveis de acesso              |
| A8  | Gerar relatórios financeiros            |
| B4  | Realizar login no sistema               |
| B3  | Registrar uso de produtos               |

---

# Should Have (S)

| ID  | História                          |
| --- | --------------------------------- |
| A3  | Alertas de estoque baixo          |
| A4  | Cadastro de clientes              |
| A5  | Lembretes automáticos             |
| A10 | Registrar formas de pagamento     |
| A9  | Visualizar serviços mais vendidos |

---

# Could Have (C)

| ID | História                       |
| -- | ------------------------------ |
| C7 | Conquistas e medalhas          |
| C8 | Notificações de promoções      |
| A6 | Cadastro de serviços e duração |
| B1 | Histórico do cliente           |

---

# Won't Have (W)

| ID  | História                          |
| --- | --------------------------------- |
| C3  | Sugestão de cortes com IA         |
| C4  | Realidade aumentada para cortes   |
| C5  | Assistente virtual com voz        |
| C6  | Recomendações baseadas em famosos |
| A11 | Previsão de faturamento com ML    |
| A12 | Previsão de estoque com IA        |

---

# Valor vs. Esforço

| ID  | História                          | Valor | Esforço |
| --- | --------------------------------- | ----- | ------- |
| C1  | Agendar horário online            | 5     | 4       |
| C2  | Visualizar horários disponíveis   | 5     | 2       |
| C9  | Cancelar/remarcar horário         | 4     | 3       |
| B2  | Visualizar agenda diária          | 5     | 2       |
| C10 | Criar conta no sistema            | 5     | 3       |
| A1  | Cadastrar produtos                | 4     | 2       |
| A2  | Atualizar estoque                 | 5     | 3       |
| A7  | Controle financeiro               | 5     | 5       |
| A13 | Controle de acesso                | 5     | 4       |
| A8  | Relatórios financeiros            | 4     | 4       |
| B4  | Login do barbeiro                 | 5     | 2       |
| B3  | Registrar uso de produtos         | 4     | 3       |
| A3  | Alertas de estoque baixo          | 4     | 3       |
| A4  | Cadastro de clientes              | 4     | 2       |
| A5  | Lembretes automáticos             | 3     | 3       |
| A10 | Formas de pagamento               | 4     | 2       |
| A9  | Serviços mais vendidos            | 3     | 3       |
| C7  | Conquistas e medalhas             | 2     | 4       |
| C8  | Promoções                         | 3     | 2       |
| A6  | Cadastro de serviços              | 4     | 2       |
| B1  | Histórico do cliente              | 3     | 3       |
| C3  | Sugestão de cortes com IA         | 2     | 5       |
| C4  | Realidade aumentada               | 1     | 5       |
| C5  | Assistente virtual                | 1     | 5       |
| C6  | Recomendações baseadas em famosos | 2     | 4       |
| A11 | Previsão de faturamento com IA    | 2     | 5       |
| A12 | Previsão de estoque com IA        | 2     | 5       |

## Legenda

### Valor

* 1 = Baixo impacto
* 2 = Pouco importante
* 3 = Importância média
* 4 = Muito importante
* 5 = Essencial para o sistema

### Esforço

* 1 = Muito fácil
* 2 = Fácil
* 3 = Médio
* 4 = Difícil
* 5 = Muito complexo


---

# Fila Única (Backlog Priorizado)

| Prioridade | ID  | História                        |
| ---------- | --- | ------------------------------- |
| 1          | C1  | Agendar horário online          |
| 2          | C2  | Visualizar horários disponíveis |
| 3          | B4  | Realizar login no sistema       |
| 4          | C10 | Criar conta no sistema          |
| 5          | B2  | Visualizar agenda diária        |
| 6          | C9  | Cancelar/remarcar horário       |
| 7          | A13 | Controle de níveis de acesso    |
| 8          | A1  | Cadastro de produtos            |
| 9          | A2  | Atualização de estoque          |
| 10         | B3  | Registrar uso de produtos       |
| 11         | A7  | Controle financeiro             |
| 12         | A8  | Relatórios financeiros          |
| 13         | A4  | Cadastro de clientes            |
| 14         | A10 | Formas de pagamento             |
| 15         | A3  | Alertas de estoque baixo        |
| 16         | A5  | Lembretes automáticos           |
| 17         | A9  | Serviços mais vendidos          |
| 18         | A6  | Cadastro de serviços            |
| 19         | B1  | Histórico do cliente            |
| 20         | C8  | Promoções                       |
| 21         | C7  | Conquistas e medalhas           |
| 22         | C3  | Sugestão de cortes com IA       |
| 23         | C4  | Realidade aumentada             |
| 24         | C5  | Assistente virtual              |
| 25         | C6  | Recomendações de famosos        |
| 26         | A11 | Previsão de faturamento com IA  |
| 27         | A12 | Previsão de estoque com IA      |
