# Mandantes e MANDT

## O que é um Mandante?

Um Client (Mandante) é uma separação lógica de dados dentro de um mesmo sistema SAP.

Exemplo:

Client 100 = Treinamento

Client 200 = Homologação

Client 300 = Produção

---

## O que é MANDT?

Campo utilizado para identificar o Client.

MANDT = Client ID

---

## Como o SAP separa os dados?

Quando um usuário entra no Client 300:

O SAP automaticamente filtra:

SELECT *
FROM tabela
WHERE MANDT = '300'

---

## Tabela T000

Lista dos mandantes existentes.

Transação:

SE16 → T000

---

## Transações Relacionadas

### SCC4

Configuração de mandantes

### SCCL

Client Copy

## 📌 Memorize

- Client e Mandante representam a mesma ideia.
- Cada Client possui um número chamado MANDT.
- O SAP utiliza o MANDT para separar os dados entre os clientes.
### SCC1

Transporte entre Clients
