# Comparação entre Testes Paramétricos e Não Paramétricos

Este projeto apresenta uma comparação entre o teste t de Student e o teste de Mann-Whitney, avaliando o desempenho dos dois métodos em diferentes cenários estatísticos.

Foram realizadas 1.000 simulações com amostras geradas a partir de distribuições normais e distribuições Gama. Nos cenários simulados, foram analisados o poder empírico dos testes, sua capacidade de detectar diferenças entre grupos e o controle do erro tipo I quando não existe diferença real entre as populações.

Nas simulações com dados normais, os dois testes apresentaram desempenho semelhante, embora o teste t de Student seja o mais indicado quando as suposições paramétricas são satisfeitas. Nos cenários com distribuições assimétricas, o teste de Mann-Whitney foi considerado uma alternativa mais robusta por não depender da hipótese de normalidade.

Também foi realizada uma aplicação com dados históricos das ações da Amazon, comparando os preços de fechamento antes e depois da crise financeira de 2008. A normalidade dos grupos foi avaliada pelo teste de Shapiro-Wilk e as diferenças foram investigadas pelos testes t de Welch e Mann-Whitney.

O projeto demonstra como o formato da distribuição, o tamanho amostral e a magnitude da diferença entre os grupos podem influenciar o desempenho e a escolha de um teste estatístico.

## Objetivo

Comparar o desempenho de um teste paramétrico e de um teste não paramétrico em dados simulados e reais, analisando poder estatístico, taxa de rejeição, robustez à assimetria e adequação das suposições.

## Metodologia

O estudo foi desenvolvido em duas etapas:

1. Simulação de amostras normais e assimétricas, com e sem diferenças entre os grupos.
2. Aplicação dos testes em dados históricos das ações da Amazon, divididos entre os períodos anterior e posterior à crise financeira de 2008.

Em cada simulação, foram aplicados o teste t de Student e o teste de Mann-Whitney. A proporção de rejeições da hipótese nula foi utilizada para avaliar o poder empírico ou, nos cenários sem diferença real, a taxa de erro tipo I.
## Tecnologias utilizadas

- R
- ggplot2
- tidyr
- Teste t de Student
- Teste t de Welch
- Teste de Mann-Whitney
- Teste de Shapiro-Wilk
- Simulação de Monte Carlo
- Análise de poder estatístico
