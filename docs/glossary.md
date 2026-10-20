# Glossary

## Customer

Representa um cliente que acessa a plataforma com um perfil autenticado e pode realizar compras no e-commerce.

## Merchant

Representa o comerciante responsável pela loja virtual. O gerenciamento da loja é realizado por meio de um perfil autenticado e autorizado a atuar em seu nome.

## Cart

Representa a intenção de compra do cliente, reunindo os produtos selecionados e suas respectivas quantidades. Pode ser alterado e é preservado entre sessões quando a jornada de compra não é concluída. O carrinho dá origem a um pedido quando o cliente confirma a intenção de compra no checkout, antes da aprovação do pagamento.

## Order

Representa o registro da compra solicitada pelo cliente a partir do carrinho, com os itens, as quantidades e os preços acordados no momento da confirmação.

Os estados abaixo indicam a conclusão da compra quanto ao pagamento, sem representar o andamento do envio ou da entrega:

- **`FINISHED`** - Pedido com pagamento aprovado.
- **`UNFINISHED`** - Pedido sem pagamento aprovado, incluindo os casos de pagamento pendente ou recusado.

## Product

Representa um produto oferecido no catálogo da loja, identificado por um nome e associado a um preço de venda. Sua quantidade em estoque representa as unidades disponíveis para venda, distinta da quantidade selecionada pelo cliente no carrinho ou registrada no pedido.

## Payment

Representa uma tentativa de pagamento de um pedido, processada por um gateway externo. Um pedido pode ter mais de uma tentativa de pagamento, por exemplo, quando o cliente tenta novamente após uma recusa.

- **`PENDING`** - Tentativa de pagamento aguardando confirmação do resultado pelo gateway.
- **`APPROVED`** - Tentativa de pagamento aprovada pelo gateway.
- **`REFUSED`** - Tentativa de pagamento recusada pelo gateway.
