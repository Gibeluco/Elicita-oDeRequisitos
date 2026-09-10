# Atividade — Elicitação de Requisitos

**Contexto:** Sistema para empresa que vende produtos por telefone ou em encontros presenciais. Três processos principais: registro de pedidos (vendedores), cadastro/remoção de produtos (administrador) e controle de estoque (time de estoque).

---

## Processo 1 — Registro de Pedidos (Vendedores)

**Requisito 1.** O sistema deve permitir que o vendedor registre um novo pedido informando cliente, produtos, quantidades e canal de venda (telefone ou presencial).

- **Fonte 1.** Entrevista com o vendedor. Fonte humana, nível operacional, classe de usuário vendedor.
- **Fonte 2.** Script de atendimento telefônico utilizado pela equipe comercial. Fonte não humana, categoria documentação.

**Requisito 2.** O sistema deve registrar a forma de pagamento escolhida no momento da venda.

- **Fonte 1.** Entrevista com o vendedor. Fonte humana, nível operacional, classe de usuário vendedor.
- **Fonte 2.** Política comercial sobre formas de pagamento aceitas. Fonte não humana, categoria documentação.

**Requisito 3.** O sistema deve impedir o registro de um pedido cujos itens não possuam quantidade disponível em estoque no momento da venda.

- **Fonte 1.** Entrevista com o gerente comercial. Fonte humana, nível tático.
- **Fonte 2.** Sistema legado de vendas atualmente em uso pela empresa. Fonte não humana, categoria sistema legado.

---

## Processo 2 — Cadastro e Remoção de Produtos (Administrador)

**Requisito 1.** O sistema deve permitir que o administrador cadastre um novo produto informando nome, descrição, preço e categoria.

- **Fonte 1.** Entrevista com o administrador do sistema. Fonte humana, nível operacional, classe de usuário administrador.
- **Fonte 2.** Catálogo de produtos de empresas concorrentes do mesmo segmento. Fonte não humana, categoria concorrência.

**Requisito 2.** O sistema deve permitir que o administrador remova (ou inative) um produto que não esteja mais disponível para venda.

- **Fonte 1.** Entrevista com o administrador do sistema. Fonte humana, nível operacional, classe de usuário administrador.
- **Fonte 2.** Sistema legado de cadastro de produtos utilizado antes da nova solução. Fonte não humana, categoria sistema legado.

**Requisito 3.** O sistema deve impedir a remoção definitiva de um produto que possua pedidos já registrados, permitindo apenas sua inativação.

- **Fonte 1.** Entrevista com o diretor administrativo-financeiro. Fonte humana, nível estratégico.
- **Fonte 2.** Norma de auditoria contábil que exige rastreabilidade de itens vendidos. Fonte não humana, categoria norma.

---

## Processo 3 — Controle de Estoque (Time de Estoque)

**Requisito 1.** O sistema deve dar baixa automática na quantidade em estoque de um produto sempre que um pedido for confirmado.

- **Fonte 1.** Entrevista com o operador de estoque. Fonte humana, nível operacional, classe de usuário estoquista.
- **Fonte 2.** Sistema legado de controle de estoque atualmente em uso. Fonte não humana, categoria sistema legado.

**Requisito 2.** O sistema deve permitir o registro de entradas de mercadorias, informando fornecedor, quantidade e data de recebimento.

- **Fonte 1.** Entrevista com o supervisor de estoque. Fonte humana, nível tático.
- **Fonte 2.** Nota fiscal de entrada emitida pelo fornecedor. Fonte não humana, categoria documentação.

**Requisito 3.** O sistema deve emitir um alerta ao time de estoque quando a quantidade disponível de um produto atingir o nível mínimo definido.

- **Fonte 1.** Entrevista com o operador de estoque. Fonte humana, nível operacional, classe de usuário estoquista.
- **Fonte 2.** Norma interna de gestão de estoque mínimo/máximo da empresa. Fonte não humana, categoria norma.