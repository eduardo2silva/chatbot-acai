# Diagrama de Casos de Uso

## Ator
- Cliente

## Casos de Uso Identificados
- Visualizar cardápio
- Escolher produtos
- Informar endereço
- Escolher forma de pagamento
- Confirmar pedido

## Descrição Geral
O cliente interage com o chatbot para realizar pedidos de açaí, desde a visualização do cardápio até a confirmação do pedido. O sistema processa as informações e notifica o estabelecimento.
## Diagrama de Casos de Uso (Visual)

```mermaid
flowchart LR
    Cliente --> UC1[Visualizar cardápio]
    Cliente --> UC2[Selecionar produtos]
    Cliente --> UC3[Informar endereço]
    Cliente --> UC4[Escolher forma de pagamento]
    Cliente --> UC5[Confirmar pedido]
