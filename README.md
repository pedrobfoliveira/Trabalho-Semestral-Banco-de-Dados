# Trabalho Semestral – Banco de Dados

Projeto desenvolvido em **grupo** como trabalho semestral da disciplina de **Banco de Dados**, com foco em **modelagem relacional**, **SQL** e **PL/SQL** utilizando **Oracle Database**.

O sistema modela o funcionamento de um **posto de combustíveis com loja de conveniência**, abrangendo controle de clientes, funcionários, produtos, vendas, estoque e regras de negócio implementadas via **triggers** e **procedures**.

---

## 👥 Integrantes do Grupo

- Pedro Oliveira
- José Auto
- Matheus Sena
- Ulisses Veiga
---

## 🎯 Objetivo do Projeto

Aplicar os conceitos estudados na disciplina, incluindo:

- Modelagem de banco de dados relacional
- Criação de tabelas, chaves primárias e estrangeiras
- Uso de **sequences**
- Implementação de **triggers** para regras de negócio
- Implementação de **procedures** em PL/SQL
- Garantia de integridade e validações no nível do banco

---

## 🧱 Modelagem do Sistema

O banco de dados contempla, entre outros, os seguintes domínios:

- Clientes e funcionários
- Endereços e telefones
- Produtos de loja e combustíveis
- Bombas, bicos e aferições
- Compras e vendas
- Formas de pagamento
- Controle de estoque
- Alertas e gratificações

A integridade dos dados é garantida por meio de **constraints**, **triggers** e **procedures**.

---

## ⚙️ Regras de Negócio Implementadas

### 🔔 Regra 1 – Ponto de Reabastecimento
- Gera automaticamente um alerta quando o estoque de um produto da loja cai abaixo do valor mínimo definido.

### 📦 Regra 2 – Controle de Estoque
- **2a:** Impede a venda caso não haja estoque suficiente.
- **2b:** Atualiza automaticamente o estoque após a venda.

### 💰 Regra 3 – Limite de Redução de Preço
- Impede reduções de preço acima de um percentual máximo permitido (ex: 10%).

### 🎁 Regra 4 – Gratificação de Fim de Ano
- Procedure que registra gratificações para todos os funcionários ativos.

### ⛽ Regra 5 – Validação de Aferição de Bico
- Apenas funcionários com cargo específico podem registrar aferições.

---

## ▶️ Como Executar o Projeto

A ordem recomendada de execução dos scripts no Oracle é:

1. esquema.sql
2. triggers.sql
3. procedures.sql

---

## 🛠️ Tecnologias Utilizadas

- Oracle Database
- SQL
- PL/SQL

---

## 📌 Observações

- Projeto desenvolvido exclusivamente para fins **acadêmicos**.
- Não utiliza dados reais.
- Estrutura focada em regras de negócio no nível do banco de dados.
