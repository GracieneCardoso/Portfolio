# 📘 Dicionário de Dados - Rede de Varejo

## Cliente
| Campo | Tipo | Descrição |
|-------|------|-----------|
| id_cliente | INT | Chave primária |
| nome | VARCHAR | Campo de dados |
| cpf | VARCHAR | Campo de dados |
| endereco | VARCHAR | Campo de dados |
| telefone | VARCHAR | Campo de dados |

## Vendedor
| Campo | Tipo | Descrição |
|-------|------|-----------|
| id_vendedor | INT | Chave primária |
| nome | VARCHAR | Campo de dados |
| id_loja | INT | Chave estrangeira |

## Produto
| Campo | Tipo | Descrição |
|-------|------|-----------|
| id_produto | INT | Chave primária |
| nome | VARCHAR | Campo de dados |
| descricao | VARCHAR | Campo de dados |
| preco | VARCHAR | Campo de dados |
| id_categoria | INT | Chave estrangeira |

## Categoria
| Campo | Tipo | Descrição |
|-------|------|-----------|
| id_categoria | INT | Chave primária |
| nome | VARCHAR | Campo de dados |

## Loja
| Campo | Tipo | Descrição |
|-------|------|-----------|
| id_loja | INT | Chave primária |
| nome | VARCHAR | Campo de dados |
| endereco | VARCHAR | Campo de dados |
| telefone | VARCHAR | Campo de dados |

## Transacao
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
| Campo | Tipo | Descrição |
|-------|------|-----------|
| id_pagamento | INT | Chave primária |
| metodo | VARCHAR | Campo de dados |

## Promocao
| Campo | Tipo | Descrição |
|-------|------|-----------|
| id_promocao | INT | Chave primária |
| descricao | VARCHAR | Campo de dados |
| data_inicio | VARCHAR | Campo de dados |
| data_fim | VARCHAR | Campo de dados |
| id_categoria | INT | Chave estrangeira |

## Estoque
| Campo | Tipo | Descrição |
|-------|------|-----------|
| id_estoque | INT | Chave primária |
| id_loja | INT | Chave estrangeira |
| id_produto | INT | Chave estrangeira |
| quantidade | VARCHAR | Campo de dados |

