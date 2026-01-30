# Diagrama Entidade-Relacionamento

## Entidade Produto
- id_produto
- nome
- preco

## Entidade Pedido
- id_pedido
- itens
- total
- endereco
- forma_pagamento
- status

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
