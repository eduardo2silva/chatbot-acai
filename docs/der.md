# Diagrama Entidade-Relacionamento (DER)

## Tabela Cliente
- **id_cliente (PK)**
- nome
- telefone

---

## Tabela Pedido
- **id_pedido (PK)**
- **id_cliente (FK)**
- endereco
- forma_pagamento
- status
- total

**Relacionamento:**  
Cliente (1) —— (N) Pedido  
Pedido.id_cliente → Cliente.id_cliente

---

## Tabela Produto
- **id_produto (PK)**
- nome
- preco

---

## pedido_has_produto
- **id_item (PK)**
- **id_pedido (FK)**
- **id_produto (FK)**
- Quantidade
- Subtotal

**Relacionamentos:**  
Pedido (1) —— (N) Item_Pedido  
Item_Pedido.id_pedido → Pedido.id_pedido  

Produto (1) —— (N) Item_Pedido  
Item_Pedido.id_produto → Produto.id_produto

---

## Resumo dos Relacionamentos
- Cliente → Pedido (1:N)
- Pedido → Item_Pedido (1:N)
- Produto → Item_Pedido (1:N)

