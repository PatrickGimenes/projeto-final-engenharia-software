# Projeto Final - Gaio

## Etapa 2 - Sprint 1 (MVP)

### Equipe

| Nome    | Função        |
| ------- | ------------- |
| Gustavo | Desenvolvedor |
| Patrick | Desenvolvedor |
| Vicente | Product Owner |

---

# Objetivo da Sprint 1

Modelar o núcleo do sistema de gestão para barbearia utilizando UML, contemplando apenas os requisitos classificados como **Must Have**.

**Duração:** 7 dias

---

# Backlog da Sprint 1

## Cliente

* Criar conta no sistema 
* Agendar horário online 
* Visualizar horários disponíveis
* Cancelar ou remarcar horário

## Barbeiro

* Realizar login
* Visualizar agenda diária
* Registrar uso de produtos

## Administrador

* Cadastrar produtos
* Atualizar estoque 
* Registrar entradas financeiras
* Registrar saídas financeiras 
* Gerar relatórios financeiros 
* Controlar níveis de acesso

---

# Diagrama de Contexto

```mermaid
flowchart LR

Cliente([Cliente])
Barbeiro([Barbeiro])
Administrador([Administrador])

Sistema([Sistema de Gestão da Barbearia])


Cliente -->|Agendamento| Sistema
Cliente -->|Consulta Horários| Sistema
Cliente -->|Remarcação| Sistema

Barbeiro -->|Consulta Agenda| Sistema
Barbeiro -->|Registro de Produtos| Sistema

Administrador -->|Gestão Estoque| Sistema
Administrador -->|Gestão Financeira| Sistema
Administrador -->|Controle de Acesso| Sistema
```

---

# Diagrama de Casos de Uso

```mermaid
flowchart LR

Cliente([Cliente])
Barbeiro([Barbeiro])
Administrador([Administrador])

subgraph Sistema

UC1((Criar Conta))
UC2((Agendar Horário))
UC3((Visualizar Horários))
UC4((Cancelar Agendamento))
UC5((Remarcar Agendamento))

UC6((Realizar Login))
UC7((Visualizar Agenda))
UC8((Registrar Uso de Produtos))

UC9((Cadastrar Produto))
UC10((Atualizar Estoque))
UC11((Registrar Movimentação Financeira))
UC12((Gerar Relatório Financeiro))
UC13((Gerenciar Permissões))

end

Cliente --> UC1
Cliente --> UC2
Cliente --> UC3
Cliente --> UC4
Cliente --> UC5
Cliente --> UC6

Barbeiro --> UC6
Barbeiro --> UC7
Barbeiro --> UC8

Administrador --> UC6
Administrador --> UC9
Administrador --> UC10
Administrador --> UC11
Administrador --> UC12
Administrador --> UC13
```

---

# Diagrama de Sequência

## Fluxo Principal - Agendamento de Horário

```mermaid
sequenceDiagram

actor Cliente
participant Sistema
participant Agenda
participant Banco

Cliente->>Sistema: Solicita horários disponíveis

Sistema->>Agenda: Consultar horários

Agenda-->>Sistema: Horários livres

Sistema-->>Cliente: Exibe horários

Cliente->>Sistema: Seleciona horário

Sistema->>Agenda: Validar disponibilidade

Agenda-->>Sistema: Horário disponível

Sistema->>Banco: Salvar agendamento

Banco-->>Sistema: Confirmação

Sistema-->>Cliente: Agendamento realizado
```

---

# Diagrama de Classes

```mermaid
classDiagram

class Usuario{
+id:int
+nome:string
+email:string
+senha:string
+perfil:string
+login()
+logout()
}

class Cliente{
+telefone:string
+agendarHorario()
+cancelarHorario()
+remarcarHorario()
}

class Barbeiro{
+visualizarAgenda()
+registrarConsumoProduto()
}

class Administrador{
+cadastrarProduto()
+atualizarEstoque()
+gerarRelatorio()
+controlarPermissoes()
}

class Agendamento{
+id:int
+data:date
+horario:string
+status:string
+criar()
+cancelar()
+remarcar()
}

class Produto{
+id:int
+nome:string
+quantidade:int
+estoqueMinimo:int
+atualizarQuantidade()
}

class MovimentacaoFinanceira{
+id:int
+tipo:string
+valor:decimal
+data:date
+registrar()
}

Usuario <|-- Cliente
Usuario <|-- Barbeiro
Usuario <|-- Administrador

Cliente "1" --> "*" Agendamento
Barbeiro "1" --> "*" Agendamento

Barbeiro --> Produto

Administrador --> Produto
Administrador --> MovimentacaoFinanceira
```

---
