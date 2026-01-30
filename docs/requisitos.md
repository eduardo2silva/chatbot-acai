<div alig="center">
<h1> DOCUMENTO DE REQUISITOS <h1>
<p><strong>Versão 1.0</strong></p>
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
|	RF02 | selecionar produtos | Permitir que o usuário selecione um ou mais produtos do cardápio apresentado. Esse requisito é necessário para viabilizar a composição do pedido de acordo com a preferência do cliente. |
|	RF03 | Informar endereço de entrega | Permitir que o usuário informe o endereço onde o pedido deverá ser entregue. Esse requisito é fundamental para que o estabelecimento saiba para onde encaminhar o pedido. |
|	RF04 | Escolher forma de pagamento | Permitir que o usuário escolha a forma de pagamento entre PIX ou Cartão. Esse requisito organiza o fluxo do pedido e define a simulação do pagamento a ser realizada pelo sistema. |
|	RF05 | Calcular valor total do pedido | Permitir que o sistema calcule automaticamente o valor total do pedido com base nos produtos selecionados. Esse requisito garante precisão nos valores informados ao cliente. |
|	RF06 | Registrar pedido | Permitir que o sistema registre as informações do pedido no banco de dados, incluindo itens, valor total, endereço e forma de pagamento. Esse requisito é necessário para controle e rastreabilidade dos pedidos. |
|	RF07 | Simular pagamento | Permitir que o sistema simule o processo de pagamento de acordo com a forma escolhida, exibindo mensagens pré-definidas para PIX ou Cartão. Esse requisito atende ao escopo acadêmico do projeto, sem integração real com serviços financeiros. |
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

