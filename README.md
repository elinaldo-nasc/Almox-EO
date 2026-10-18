# Almox EO

Controle de estoque feito só no Excel, com fórmulas, validação de dados, formatação condicional e gráficos. Não usa macros nem VBA.

![Dashboard do Almox EO](images/dashboard.png)

## O que ele faz

O projeto simula o almoxarifado de uma empresa fictícia, a Conecta Log Serviços e Telecom. Dá para:

- cadastrar produtos com estoque mínimo e máximo;
- registrar entradas e saídas;
- ver o saldo e o status de cada item (CRÍTICO, REPOR ou OK);
- saber o que repor e quanto comprar;
- acompanhar tudo no dashboard, com seletor de mês.

A planilha tem as abas Dashboard, Produtos, Movimentações, Estoque, Relatórios e Leia-me. Na aba Leia-me estão o guia de uso e as fórmulas explicadas.

## Como calculei

- Saldo = estoque inicial + entradas − saídas
- Valor em estoque = saldo × custo unitário
- CRÍTICO quando o saldo é 0 ou menos, REPOR quando é menor ou igual ao mínimo, OK nos outros casos
- Sugestão de compra = estoque máximo − saldo

## Como usar

1. Baixe o `Almox_EO.xlsx` e abra no Excel.
2. Se aparecer o Modo de Exibição Protegido, clique em Habilitar Edição. Sem isso as fórmulas não calculam.
3. Cadastre produtos na aba Produtos e registre entradas e saídas na aba Movimentações.
4. Veja o resultado nas abas Estoque e Dashboard.

As células brancas são para digitar. As cinza-azuladas têm fórmula e não devem ser editadas.

## O que quero melhorar

- Proteger as células com fórmula
- Bloquear saídas maiores que o saldo
- Fazer a curva ABC

## Aviso

Todos os dados (empresa, produtos, pessoas, valores e datas) são fictícios e servem só para demonstração.

Projeto pessoal de portfólio de Elinaldo Oliveira do Nascimento.
