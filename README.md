# sistema-e-comerce-dio
📦 Projeto Conceitual de Banco de Dados – Sistema de E-commerce
Este projeto tem como objetivo a criação de um modelo conceitual de banco de dados para um sistema de e-commerce, considerando as principais entidades envolvidas no processo de compra, clientes, formas de pagamento e entregas.

O modelo foi desenvolvido como parte do desafio de projeto da DIO, com foco em boas práticas de modelagem e normalização.
🎯 Objetivo

Refinar e apresentar um modelo conceitual de banco de dados com os seguintes requisitos:

    Uma conta de cliente pode ser Pessoa Física (PF) ou Pessoa Jurídica (PJ), mas não ambas;

    O cliente pode ter múltiplas formas de pagamento cadastradas;

    Cada entrega possui um status (em andamento, entregue, cancelada...) e um código de rastreio;

    A base contempla também pedidos, produtos, categorias e histórico de compra.

🧩 Entidades e Relacionamentos (Resumo)
🧑 Cliente

    Cliente pode ser PF ou PJ, representados por entidades separadas (Relacionamento 1:1 com restrição exclusiva).

    Campos comuns: nome, e-mail, telefone.

🆔 Pessoa Física (PF)

    CPF, data de nascimento, gênero.

🏢 Pessoa Jurídica (PJ)

    CNPJ, razão social, inscrição estadual.

🛒 Pedido

    Relacionado a um cliente.

    Possui data, valor total e formas de pagamento.

💳 Forma de Pagamento

    Relacionamento N:1 com Pedido.

    Ex: cartão, boleto, pix.

📦 Entrega

    Relacionada a um pedido.

    Contém status e código de rastreio.

📦 Produto

    Pode pertencer a uma ou mais categorias.

    É associado aos pedidos por meio de uma entidade intermediária (ex: ItemPedido).

🏷️ Categoria

    Ex: Eletrônicos, Moda, Alimentos.
