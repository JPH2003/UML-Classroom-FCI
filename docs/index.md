<h2><a href= "https://www.mackenzie.br">Universidade Presbiteriana Mackenzie</a></h2>
<h3><a href= "https://www.mackenzie.br/graduacao/sao-paulo-higienopolis/sistemas-de-informacao">Sistemas de Informação</a></h3>


<font size="+12"><center>
*Pizzaria*
</center></font>

>*Observação 1: A estrutura inicial deste documento é só um exemplo. O seu grupo deverá alterar esta estrutura de acordo com o que está sendo solicitado na disciplina.*

>*Observação 2: O índice abaixo não precisa ser editado se você utilizar o Visual Studio Code com a extensão **Markdown All in One**. Essa extensão atualiza o índice automaticamente quando o arquivo é salvo.*

**Conteúdo**

- [Autores](#nome-alunos)
- [Descrição do projeto](#introdução-do-projeto)
- [Análise de requisitos funcionais e não-fucionais](#descrição-dos-requisitos)
- [Diagrama de casos de uso](#diagrama-de-comportamento-atores)
- [Descrição dos casos de uso](#descrição-das-funcões)
- [Diagrama de senquencia](#diagrama-de-ordem-interações)
- [Diagrama de classes](#diagrama-orientado-objetos)
- [Diagrama de componentes](#diagrama-estrutura-componente)
- [Decisões de arquitetura](#decisões-de-arquitetura)
- [Diagrama de implantação](#diagrama-de-hardware-software)
- [Referências](#referências)


# Autores

* Julio Piffer Harada<br>


# Descrição do projeto

*O projeto visa otimizar o processo de entregas das 40 lojas da Pizza-Express otimizando o tempo de entrega num tempo menor que 30 minutos,e o progresso de lojas que não teriam espaço no varejo por falta de conhecimento dos usuários e da sua localização.*

# Análise de requisitos funcionais e não-funcionais
**Requisitos Funcionais**
*Cadastro do cliente: O cliente deve criar uma conta para poder efetuar o pedido.<br>
*Visualização do menu: O cliente deve ter acesso ao menu e as informações presentes.<br>
*Registro de pedido: O sistema deve permitir que os pedidos dos clientes sejam registrados no sistema<br>
*Atulização em tempo real do pedido: O sistema deve transmitir ao usuário a situação do pedido em tempo real.<br>
*Registro de pagamento: O sistema deve registrar que foi efetuado o pagamento do pedido.<br>
*Cancelamento do pedido: O sistema deve permitir que o cliente altere ou cancele o pedido.<br>


**Requisitos Não-Funcionais**

*Acessibilidade: O sistema deve ser acessível a todos os usuários, incluindo pessoas com deficiências. Deve ter recursos de acessibilidade como tamanho de fonte ajustável.<br>
*Compatibilidade com navegadores web: O sistema deve ser compatível com todos os principais navegadores web, incluindo navegadores para dispositivos móveis.<br>
*Desempenho: O sistema deve ser capaz de lidar com a alta demanda de pedidos sem ser afetado negativamento ou apresentar mal funcionamento.<br>
*Segurança: O sistema deve aderir às melhores práticas de segurança para proteger os dados dos clientes.<br>
*Facilidade de acesso e uso: O sistema deve ter um sistema fácil acesso à todas as idades,já que assim o alcance e lucro das lojas será maior.<br>

# Diagrama de casos de uso

![diagrama-casos-de-uso](https://github.com/JPH2003/UML-Classroom-FCI/assets/131881941/b05f75e3-18e6-4aa0-b18f-84d018f1f629)

# Descrição dos casos de uso

### Fazer pedido:

**Ator: Cliente**

**Pré condições: Cliente precisa ter feito o cadastro no sistema**

**Descrição: O cliente pede o pedido**

**Fluxo básico:**

- O cliente acessa a funcionalidade "Menu".
- O sistema apresenta o tamanho e a lista de sabores das pizzas.
- O cliente seleciona o tamanho e até 2 sabores das pizzas
- O sistema registra o tamanho e os sabores selecionados.
- O sistema pergunta ao cliente se deseja acompanhar com uma bebida
- O cliente seleciona "sim" e o sistema mostra as opções disponiveis,ou "não" e o sistema direciona para o pagamento.

### Realizar pagamento:

**Ator: Cliente**

**Descrição: O cliente efetua o pagemento do pedido**

**Fluxo básico:**

- O sistema apresenta o valor do pedido e as formas de pagamento.
- O cliente seleciona a forma de pagamento desejada.
- O sistema pede os dados e informações da conta do cliente.
- O cliente coloca os dados no sistema,entra no aplicativo do banco e efetua o pagamento.
- O sistema confirma o pedido e direciona para o atendente.

### Confirmar pedido:

**Ator: Atendente**

**Pré condições: Atendente precisa acessar o sistema**

**Descrição: O atendente recebe a informação que o pagamento do pedido foi feito e confirma o pedido**

**Fluxo básico:**

- O atendente recebe a informação do pedido
- O atendente informa sobre o pedido para o pizzaiolo.
- O atendente atualiza as informações de preparo.
- Quando o pedido estiver pronto o atendente comunica ao entregador.

### Receber pedido:

**Ator: Entregador**

**Pré condições: Entregador precisa acessar o sistema**

**Descrição: O entregar recebe os dados do pedido**

**Fluxo básico:** 

- O entregador recebe as informações do pedido.
- O entregador acessa o localizador.
- O entregador coloca o endereço do cliente e vai em direção ao destino.

### Entregar pedido:

**Ator: Entregador**

**Descrição: O entregador chega ao destino e entrega o pedido ao cliente**

**Fluxo básico:**
- O entregador chega no local registrado e entrega o pedido ao cliente.

### Ativar localização:

**Ator: Localizador**

**Descrição: O localizador é ativado e acessa o gps**

**Fluxo básico:**

### Exibir mapa:

**Ator: Localizador**

**Descrição: O localizador exibe o mapa para o entregar**

**Fluxo básico:**
- O entregador acessa o sistema de localização e o localizador exibe o mapa.

### Escolher o melhor trajeto:

**Ator: Localizador**

**Descrição: O localizador seleciona o melhor trajeto**

**Fluxo básico:**

- O localizador recebe as informações do endereço do cliente e de todas as 40 lojas da Pizza-Express.
- O localizador calcula qual a rota que levará menos tempo a ser executada.
- O localizador seleciona a loja que levará menos tempo para a entrega.

# Diagrama de sequencia

*&lt;Diagrama de ordem e interação dos objetos&gt;*

# Diagrama de classes

*&lt;Diagrama de relacionamento entre classes para os seus atributos e operações&gt;*

# Diagrama de Componentes

*&lt;Diagrama para exibir a relação estrutural dos componentes de um sistema de software

# Decisões de arquitetura

*&lt;Descrever a infraestrutura escolhida para arquitetura do projeto&gt;*

# Diagrama de implantação

*&lt;Diagrama para exibir o relacionamento de hardware e software no projeto&gt;*

# Referências

*&lt;Lista de referências&gt;*
