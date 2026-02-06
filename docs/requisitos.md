<div alig="center">
<h1> DOCUMENTO DE REQUISITOS <h1>
<br>
<h3>Equipe do Projeto</h3>
<p>
Eduardo da silva mugo <br>
Diego dos santos lopes<br>
Renato silva rodrigues<br>
</p>
</div>
<hr>
  
   
## 1. Visão Geral
Este documento descreve os requisitos do sistema de chatbot para pedidos em uma loja de açaí, desenvolvido utilizando n8n. 
## 2. Requisitos Funcionais (RF)
Os requisitosfuncionais referem-se aos requisitos que estão relacionados com a maneira com que o sistema deve operar, onde se especificam as entradas e saídas do sistema e o relacionamento comportamental entre elas, assim como a iteração com o usuário. 
Desta forma, os requisitos encontrados para o primeiro ciclo do projeto exemplificado neste template são:
| Código | Nome | Descrição |
|---|--------|---------|
|	RF01 | Exibir cardápio de produtos | Permitir que o sistema apresente ao usuário a lista de produtos disponíveis para venda, contendo nome e preço dos açaís. Esse requisito é essencial para que o cliente conheça as opções antes de realizar o pedido. |
|	RF02 | Escolher o produtos | O sistema deve permitir que o usuário selecione os produtos do cardápio por meio da digitação do número correspondente ao produto, seguido de um espaço e da quantidade desejada (exemplo: “1 3”). Esse recurso é necessário para viabilizar a composição do pedido de acordo com a preferência do cliente, garantindo praticidade e agilidade no processo de solicitação. |
|	RF03 | Informar endereço de entrega e dados | O sistema deve permitir que o usuário informe o endereço onde o pedido deverá ser entregue, contendo rua, número da residência e bairro (exemplo: “Nome, telefone, Rua, número da residência – bairro”). Esse requisito é fundamental para que o estabelecimento saiba corretamente para onde encaminhar o pedido. |
|	RF04 | Exibir o valor total do pedido | O sistema deve calcular automaticamente o valor total do pedido com base nos itens selecionados pelo usuário e apresentar esse valor de forma clara antes da finalização da compra. |
| RF05 | Selecionar forma de pagamento | Após a apresentação do valor total do pedido, o sistema deve solicitar ao usuário a escolha da forma de pagamento, permitindo a seleção entre PIX (P) ou Cartão digitado (C), orientando o cliente sobre o processo de pagamento escolhido. |
|	RF06 | confirmação de pagamento | Permitir que o sistema simule o processo de pagamento de acordo com a forma escolhida pelo usuário. Caso a opção selecionada seja PIX, o sistema deverá enviar a chave PIX do estabelecimento, aguardar o envio do comprovante de pagamento e, após a confirmação, registrar e confirmar o pedido. Caso a opção selecionada seja Cartão, o sistema deverá exibir uma mensagem informando que o pagamento será realizado no momento da entrega. Esse requisito atende ao escopo acadêmico do projeto, não realizando integração real com serviços financeiros, e é responsável por concluir o fluxo de pagamento e confirmação do pedido.|
|	RF07 | Registro do pedido | Permitir que o sistema registre as informações do pedido no banco de dados, incluindo itens, valor total, endereço e forma de pagamento. Esse requisito é necessário para controle e rastreabilidade dos pedidos. |
| RF08 | Notificar estabelecimento | Permitir que o sistema envie uma notificação por email ao dono do estabelecimento contendo os dados do pedido realizado. Esse requisito assegura que o pedido seja visualizado e preparado para entrega. |
## 3. Requisitos Não Funcionais (RNF)
Os requisitos não funcionais definem as características de qualidade e as restrições do sistema, como desempenho, usabilidade, confiabilidade e tecnologias utilizadas. Esses requisitos não descrevem funcionalidades específicas, mas estabelecem como o sistema deve se comportar e quais padrões devem ser seguidos durante o seu funcionamento.
| Código| Nome | Descrição |
|---|-----|----------|
|	RNF01 | Usabilidade | O sistema deve possuir uma interface simples e intuitiva, permitindo que usuários com diferentes níveis de familiaridade com tecnologia consigam realizar pedidos sem dificuldades. Esse requisito é importante para garantir uma boa experiência do usuário. |
|	RNF02 | Tempo de resposta | O sistema deve responder às interações do usuário em tempo adequado, evitando atrasos excessivos nas mensagens do chatbot. Esse requisito assegura fluidez na conversação e evita frustração do usuário. |
|	RNF03 | Disponibilidade | O sistema deve estar disponível para uso durante o período de funcionamento do estabelecimento, permitindo a realização de pedidos sempre que necessário. Esse requisito garante confiabilidade no atendimento automatizado. |
|	RNF04 | Tecnologia de automação | O sistema deve utilizar a ferramenta n8n para orquestração do fluxo de conversação e automação dos processos. Esse requisito define a tecnologia base adotada no projeto. |
| RNF05 | Banco de dados | O sistema deve utilizar o banco de dados PostgreSQL para armazenamento das informações de produtos e pedidos. Esse requisito garante organização, persistência e integridade dos dados. |
| RNF06 | Segurança dos dados | O sistema deve armazenar os dados dos pedidos de forma organizada e protegida, evitando acessos não autorizados. Esse requisito é necessário para preservar a integridade das informações. |
| RNF07 | Escopo acadêmico (MVP) | O sistema deve funcionar como um protótipo mínimo viável (MVP), com funcionalidades simplificadas e simulações, sem integração real com serviços externos de pagamento. Esse requisito delimita o escopo do projeto conforme os objetivos acadêmicos. |

