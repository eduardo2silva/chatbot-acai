# Documentação de Requisitos 

## 1. Visão Geral
Este documento descreve os requisitos do sistema de chatbot para pedidos em uma loja de açaí, desenvolvido utilizando n8n. 
## 2. Requisitos Funcionais (RF)
| Código | Nome | Descrição |
|---|--------|---------|
|	RF01 | Exibir cardápio de produtos | Permitir que o sistema apresente ao usuário a lista de produtos disponíveis para venda, contendo nome e preço dos açaís. Esse requisito é essencial para que o cliente conheça as opções antes de realizar o pedido. |
|	RF02 | Selecionar produto | Permitir que o usuário selecione um ou mais produtos do cardápio apresentado. Esse requisito é necessário para viabilizar a composição do pedido de acordo com a preferência do cliente. |
|	RF03 | Informar endereço de entrega | Permitir que o usuário informe o endereço onde o pedido deverá ser entregue. Esse requisito é fundamental para que o estabelecimento saiba para onde encaminhar o pedido. |
|	RF04 | Escolher forma de pagamento | Permitir que o usuário escolha a forma de pagamento entre PIX ou Cartão. Esse requisito organiza o fluxo do pedido e define a simulação do pagamento a ser realizada pelo sistema. |
|	RF05 | Calcular valor total do pedido | Permitir que o sistema calcule automaticamente o valor total do pedido com base nos produtos selecionados. Esse requisito garante precisão nos valores informados ao cliente. |
|	RF06 | Registrar pedido | Permitir que o sistema registre as informações do pedido no banco de dados, incluindo itens, valor total, endereço e forma de pagamento. Esse requisito é necessário para controle e rastreabilidade dos pedidos. |
|	RF07 | Simular pagamento | Permitir que o sistema simule o processo de pagamento de acordo com a forma escolhida, exibindo mensagens pré-definidas para PIX ou Cartão. Esse requisito atende ao escopo acadêmico do projeto, sem integração real com serviços financeiros. |
| RF08 | Notificar estabelecimento | Permitir que o sistema envie uma notificação ao dono do estabelecimento contendo os dados do pedido realizado. Esse requisito assegura que o pedido seja visualizado e preparado para entrega. |
## 3. Requisitos Não Funcionais (RNF)
| Código | Descrição |
|---|-----------|
|	RNF01 | O sistema deve ser simples e intuitivo. |
|	RNF02 | O sistema deve funcionar em ambiente local. |
|	RNF03 | O banco de dados deve ser relacional (PostgreSQL). |
|	RNF04 | O chatbot deve responder em tempo aceitável ao usuário. |

