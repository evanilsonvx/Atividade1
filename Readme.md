# 📊 Desafio: Transformando Dados em Informação com Planilhas

**Acesso aos arquivos:**
- 🔗 [Link para a Planilha no Google Sheets](https://github.com/evanilsonvx/Atividade1/blob/main/vendas_auto_pecas.xlsx)
- 📄 [Apresentação em PDF](NOME_DO_SEU_ARQUIVO_DE_APRESENTACAO.pdf)
- 📁 [Base de dados bruta (XLSX)](vendas_auto_pecas.xlsx)

---

## 1. O Tema Escolhido
**Que situação você decidiu registrar?**
Decidi registrar o controle de vendas de uma loja de autopeças (comercialização de itens de motor, freios, suspensão e parte elétrica) no período de um mês.

**Por que escolheu esse tema?**
Escolhi esse tema porque o mercado automotivo trabalha com um volume grande de peças e categorias diferentes. É um excelente cenário para mostrar como organizar o giro de estoque, diferenciar o faturamento bruto do lucro líquido e identificar quais peças sustentam o negócio.

## 2. O Usuário da Planilha
**Quem usaria essa planilha?**
O proprietário, o gerente da loja de autopeças ou o responsável pelas compras de reposição.

**O que essa pessoa precisa descobrir?**
Essa pessoa precisa descobrir quais categorias de peças giram mais rápido, quais produtos oferecem a maior margem de lucro real (já descontando o custo da peça) e o volume total faturado no mês.

## 3. Organização dos Dados
**Como você estruturou a tabela?**
Estruturei a tabela com as seguintes colunas: `ID da Venda`, `Data`, `Produto`, `Categoria`, `Custo Unitário`, `Preço Unitário`, `Quantidade`, `Faturamento Total` e `Lucro Total`.

**Quais problemas encontrou e como os resolveu?**
Para garantir que os dados de entrada fizessem sentido e não fossem preenchidos com erros de digitação, padronizei a coluna de *Categorias* (Freios, Motor, Suspensão, Elétrica) e automatizei o cálculo de *Faturamento* e *Lucro* multiplicando a quantidade pelos seus respectivos valores de preço e custo através de fórmulas.

## 4. Perguntas e Cálculos
**Quais perguntas você respondeu?**
1. Qual foi o faturamento bruto e o lucro total da loja no mês?
2. Quais são as categorias que mais vendem em quantidade?
3. Qual produto gera o maior lucro individual?

**Quais funções usou em cada uma?**
- Usei uma função matemática de multiplicação: `=(Preço - Custo) * Quantidade` para calcular o lucro por venda em cada linha.
- Apliquei a função `=SOMA()` para descobrir o Faturamento e Lucro Totais do mês.
- Criei uma Tabela Dinâmica agrupando os produtos por `Categoria` e somando a `Quantidade` e o `Lucro Total` para análise rápida.

## 5. Personalização
**Que formatações e destaques você aplicou e por quê?**
- Apliquei formato de **Moeda (R$)** em todas as colunas financeiras (Custo, Preço, Faturamento, Lucro) para facilitar a leitura.
- Congelei a primeira linha (cabeçalho) e utilizei cores de destaque para a tabela ficar legível mesmo ao rolar a página.
- Adicionei botões de **Filtro** nos cabeçalhos, permitindo filtrar facilmente todas as vendas de apenas uma categoria (como "Suspensão", por exemplo).

## 6. Conclusões
**O que os dados mostram?**
Os dados mostram a importância de balancear as vendas de alto ticket e de alta margem. Itens como baterias e amortecedores elevam muito o faturamento bruto, mas itens de manutenção recorrente (como filtros e óleo) possuem uma saída muito constante.

**Que decisão alguém poderia tomar a partir deles?**
Ao ver que os itens de manutenção giram rápido, o gerente pode decidir manter um estoque de segurança mais alto para esses itens a fim de não perder vendas do dia a dia, enquanto trabalha com um estoque mais enxuto de peças caras (sob demanda) para não prender o fluxo de caixa.

## 7. Reflexão
**O que mudou na forma de enxergar os dados depois de organizá-los?**
Percebi que olhar apenas para o faturamento total é olhar para uma "métrica de vaidade". A planilha organizada evidenciou que vender muito em volume ou preço não significa obrigatoriamente um lucro alto, pois o custo da peça pesa significativamente. Organizar os dados mudou a visão de "dinheiro no caixa" para o verdadeiro "lucro do negócio".
