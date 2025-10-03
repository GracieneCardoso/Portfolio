# 📘 Dicionário de Dados - Rede de Varejo

## Cliente
### Definição: Indivíduo ou entidade que compra produtos. Pode possuir informações como nome, CPF, endereço, telefone, histórico de compras, etc.

| Campo | Tipo | Descrição |
|-------|------|-----------|
| id_cliente | INT | Chave primária |
| nome | VARCHAR | Campo de dados |
| cpf | VARCHAR | Campo de dados |
| endereco | VARCHAR | Campo de dados |
| telefone | VARCHAR | Campo de dados |

## Vendedor
### Definição: Funcionário da rede de varejo responsável por auxiliar o cliente durante o processo de compra, seja oferecendo informações sobre os produtos ou conduzindo transações de venda. Pode ter dados como nome, identificação de funcionário, histórico de vendas, etc.

| Campo | Tipo | Descrição |
|-------|------|-----------|
| id_vendedor | INT | Chave primária |
| nome | VARCHAR | Campo de dados |
| id_loja | INT | Chave estrangeira |

## Produto
### Definição: Item que está à venda na loja. Cada produto pode ter informações como código de barras, nome, descrição, preço, quantidade em estoque, entre outros.

| Campo | Tipo | Descrição |
|-------|------|-----------|
| id_produto | INT | Chave primária |
| nome | VARCHAR | Campo de dados |
| descricao | VARCHAR | Campo de dados |
| preco | VARCHAR | Campo de dados |
| id_categoria | INT | Chave estrangeira |

## Categoria
### Definição: Classificação dos produtos de acordo com sua natureza ou características. Por exemplo, eletrodomésticos, vestuário, alimentos, etc. Uma categoria pode ter muitos produtos.

| Campo | Tipo | Descrição |
|-------|------|-----------|
| id_categoria | INT | Chave primária |
| nome | VARCHAR | Campo de dados |

## Loja
### Definição: Unidade física onde os produtos são vendidos. Pode ser identificada por um código de loja, nome, endereço, telefone e outras informações relevantes. Além disso, cada loja pode ter um ou vários vendedores associados.

| Campo | Tipo | Descrição |
|-------|------|-----------|
| id_loja | INT | Chave primária |
| nome | VARCHAR | Campo de dados |
| endereco | VARCHAR | Campo de dados |
| telefone | VARCHAR | Campo de dados |

## Transacao
### Definição: Registro de uma venda concluída. Envolve detalhes como ID da transação, data e hora, produtos vendidos, quantidade, valor total, vendedor responsável, etc.

| Campo | Tipo | Descrição |
|-------|------|-----------|
| id_transacao | INT | Chave primária |
| data_hora | VARCHAR | Campo de dados |
| id_cliente | INT | Chave estrangeira |
| id_vendedor | INT | Chave estrangeira |
| id_loja | INT | Chave estrangeira |
| id_pagamento | INT | Chave estrangeira |
| valor_total | VARCHAR | Campo de dados |

## Pagamento
### Definição: Modo como o cliente opta por pagar sua compra. Pode incluir opções como dinheiro, cartão de crédito, cartão de débito, transferência, entre outros.

| Campo | Tipo | Descrição |
|-------|------|-----------|
| id_pagamento | INT | Chave primária |
| metodo | VARCHAR | Campo de dados |

## Promocao
### Definição: Descontos ou ofertas especiais que podem ser aplicados a produtos ou
categorias específicas durante um período determinado.

| Campo | Tipo | Descrição |
|-------|------|-----------|
| id_promocao | INT | Chave primária |
| descricao | VARCHAR | Campo de dados |
| data_inicio | VARCHAR | Campo de dados |
| data_fim | VARCHAR | Campo de dados |
| id_categoria | INT | Chave estrangeira |

## Estoque
### Definição: Refere-se à quantidade de produtos disponíveis em uma loja ou no armazém
central da rede. Envolve o controle de entradas (compras de fornecedores) e saídas (vendas para
clientes).

| Campo | Tipo | Descrição |
|-------|------|-----------|
| id_estoque | INT | Chave primária |
| id_loja | INT | Chave estrangeira |
| id_produto | INT | Chave estrangeira |
| quantidade | VARCHAR | Campo de dados |

