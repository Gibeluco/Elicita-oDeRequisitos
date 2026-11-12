Processo: Pedido em uma cafeteria.

Piscinas: Cliente e Cafeteria.

Raias da cafeteria: Atendente e Preparação.
Fluxo do processo
1. Início: cliente escolhe os produtos e faz o pedido.
2. Atendente recebe e registra o pedido no sistema.
3. Gateway exclusivo: os produtos solicitados estão disponíveis?
4. Se não estiverem disponíveis, o atendente informa o cliente e o pedido é cancelado.
5. Se estiverem disponíveis, o atendente confirma o pedido.
6. Gateway paralelo: o pagamento é processado e os produtos começam a ser preparados ao mesmo tempo.
7. Após finalizar as duas atividades, o atendente recebe a informação de que o pedido está pronto.
8. O cliente recebe uma notificação para retirar o pedido.
9. Cliente comparece ao balcão e retira os produtos.
10. Fim: pedido entregue ao cliente.
Elementos BPMN utilizados
Elemento	Aplicação
Evento de início	Cliente realiza o pedido
Evento de fim	Pedido entregue ou cancelado
Tarefas	Registrar, confirmar, pagar e preparar
Piscinas	Cliente e Cafeteria
Raias	Atendente e Preparação
Gateway exclusivo	Verificar disponibilidade
Gateway paralelo	Pagamento e preparação simultâneos
Fluxo de mensagem	Envio do pedido e aviso de retirada

Mensagens entre piscinas
- Cliente envia o pedido para a cafeteria.
- Cafeteria envia a confirmação do pedido.
- Cafeteria avisa quando os produtos estiverem prontos.
