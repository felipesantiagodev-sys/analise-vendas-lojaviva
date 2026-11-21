# Briefing do Projeto: Análise de Vendas da LojaViva

> Este documento simula o pedido que um analista recebe de uma área de negócio.
> Leia com calma. Parte do trabalho de um analista é entender o que está sendo pedido.

## Contexto

A **LojaViva** é um e-commerce brasileiro que vende produtos de 6 categorias
(Eletrônicos, Casa, Moda, Esporte, Beleza e Livros) para clientes de todo o país.
A empresa existe há ~2 anos e nunca teve uma análise estruturada dos seus dados.

Quem pede a análise: **Mariana, Diretora Comercial.**

## Mensagem da Mariana

> "Oi! Estamos planejando o orçamento de 2027 e preciso entender melhor o nosso negócio.
> Hoje eu sei o faturamento total, mas não sei **de onde** ele vem nem **o que está
> funcionando**. Quero tomar decisões com base em dados, não em achismo.
> Consegue me ajudar até o fim do mês?"

## Perguntas de negócio

1. **Como estão as vendas ao longo do tempo?** Estamos crescendo? Existe sazonalidade (ex.: Black Friday)?
2. **Quais categorias e produtos geram mais faturamento e mais lucro?** (Atenção: faturamento ≠ lucro.)
3. **De quais estados e canais vêm os melhores clientes?** Onde vale investir em marketing?
4. **Qual o perfil de recompra?** Quantos clientes compram mais de uma vez?
5. **Quanto perdemos com cancelamentos e devoluções?**

## Entregáveis esperados

- Dados limpos e documentados (o que foi encontrado de errado e o que foi feito).
- Análises respondendo às 5 perguntas, com gráficos legíveis.
- Um **relatório executivo de 1 a 2 páginas** com conclusões e recomendações, escrito para quem NÃO é técnico.
- Repositório organizado e reproduzível (qualquer pessoa consegue rodar do zero).

## Sobre os dados

Os dados foram exportados do sistema da empresa por um colega, às pressas.
**Ninguém garante que estejam corretos.** Em empresas reais isso é a regra, não a exceção.

| Arquivo | O que representa |
|---|---|
| `clientes.csv` | Um cliente cadastrado por linha |
| `produtos.csv` | Catálogo de produtos (com preço e custo) |
| `pedidos.csv` | Um pedido por linha (data, status, pagamento, frete) |
| `itens_pedido.csv` | Os produtos dentro de cada pedido (um pedido pode ter vários itens) |

## Regras de negócio combinadas com a Mariana

- **Faturamento** conta apenas pedidos com status `entregue`.
- Pedidos `cancelado` e `devolvido` NÃO entram no faturamento, mas devem ser analisados como perda.
- Pedidos `em_transito` ainda não devem ser contados em nada financeiro.
- **Lucro bruto** = (preço unitário − custo do produto) × quantidade. O frete não entra.
- Esta é uma base **fictícia** criada para fins educacionais.
