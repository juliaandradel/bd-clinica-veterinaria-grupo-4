# 🐾 Sistema de Clínica Veterinária – Banco de Dados Relacional

Este repositório contém os scripts SQL do projeto de banco de dados da disciplina, desenvolvidos a partir da normalização e do modelo relacional final do sistema de **clínica veterinária**.

---

## 📂 Estrutura dos Arquivos

| Arquivo | Descrição |
|----------|------------|
| `sql/01_create_tables.sql` | Contém os comandos `CREATE TABLE`, com `PRIMARY KEY`, `FOREIGN KEY`, `CHECK` e `CONSTRAINTS` conforme o modelo relacional. |
| `sql/02_sequences.sql` | Contém as `CREATE SEQUENCE` utilizadas para gerar identificadores automáticos das tabelas. |
| `sql/03_insert_data.sql` | Contém os comandos `INSERT INTO` para povoamento do banco com dados coerentes e realistas. |

---

## 🧱 Modelo Relacional Base

As principais entidades modeladas após a normalização são:

- **Pessoa**, **Tutor**, **Veterinário**, **Telefone**
- **Animal** e **Alergia_Animal**
- **Serviço** e **Atendimento**
- **Medicamento**, **Vacina**, **Prescrição**
- **Pagamento** e **Parcela_Pagamento**
- **Endereço**

Cada tabela foi normalizada até a **4ª Forma Normal**, garantindo ausência de dependências parciais, transitivas e multivaloradas.

---

## 🚀 Como Executar no Oracle Live SQL

1. Acesse [https://livesql.oracle.com](https://livesql.oracle.com)
2. Crie uma nova **Worksheet** (folha de código)
3. Copie e execute **nesta ordem:**
   ```sql
   @01_create_tables.sql
   @02_sequences.sql
   @03_insert_data.sql
