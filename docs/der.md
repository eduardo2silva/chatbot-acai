# Diagrama Entidade-Relacionamento

## Entidade Produto
- id_produto
- nome
- preco

## Entidade Pedido
- id_pedido
- endereco
- forma_pagamento
- status

## Entidade Item_Pedido
- id_item
- id_pedido(FK)
- id_produto(FK)
- Quantidade
- Subtotal

## Relacionamento
Um pedido pode conter um ou mais produtos.

### ✏️ No final do arquivo, cole:

```md
## Diagrama Entidade-Relacionamento (Visual)

```mermaid
erDiagram
    PRODUTO {
        int id_produto
        string nome
        float preco
    }

    PEDIDO {
        int id_pedido
        string itens
        float total
        string endereco
        string forma_pagamento
        string status
    }

    PEDIDO }o--o{ PRODUTO : contem
