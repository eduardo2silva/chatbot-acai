# Diagrama de Casos de Uso

## Ator
- Cliente
- bot

## Casos de Uso Identificados
- Exibir cardápio de produtos
- Escolher produtos
- Informar endereço de entrega
- Exibir valor total
- Escolher forma de pagamento 
- Confirmar pagamento
- Registro do pedido
- Notificar estabelecimento

## Descrição Geral
O cliente interage com o chatbot para realizar pedidos de açaí, desde a visualização do cardápio até a confirmação do pedido. O sistema processa as informações e notifica o estabelecimento.
## Diagrama de Casos de Uso (Visual)

<img width="831" height="391" alt="Diagrama de caso de Uso bot drawio" src="https://github.com/user-attachments/assets/8daebfbb-68e0-4b47-b284-5245c8504d88" />

## Descrição dos Casos de Uso

### UC1 – Exibir cardápio de produtos
O ator **Bot** exibe o cardápio de produtos disponíveis, contendo os tipos de açaí e valores.

### UC2 – Escolher produtos
O ator **Cliente** seleciona os produtos do cardápio exibido pelo sistema, escolhendo os itens e quantidades que deseja adicionar ao pedido.

### UC3 – Informar endereço
O ator **Cliente** informa o endereço de entrega do pedido para que o sistema possa registrar corretamente o local onde o pedido deverá ser entregue.

### UC4 – Exibir valor total
O ator **Bot** calcula automaticamente o valor total do pedido com base nos produtos selecionados e exibe o valor final ao cliente para conferência.

### UC5 – Selecionar forma de pagamento
O ator **Cliente** escolhe a forma de pagamento disponível no sistema, como PIX ou cartão, para dar continuidade ao processo do pedido.

### UC6 – Confirmar pagamento
O ator **Cliente** confirma o pagamento de acordo com a forma escolhida, permitindo que o sistema prossiga com a finalização do pedido.

### UC7 – Registrar o pedido 
O ator **Bot** registra o pedido no sistema após a confirmação do pagamento, armazenando todas as informações necessárias, como produtos, endereço e forma de pagamento.

### UC8 – Notificar estabelecimento
O ator **Bot** notifica o estabelecimento sobre o novo pedido realizado, enviando as informações para que o pedido possa ser preparado e entregue.
