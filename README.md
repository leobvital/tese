# Inversão magnética radial robusta para estimar a geometria de fontes 3D

Autor: 	[Leonardo B. Vital](https://www.pinga-lab.org/people/vital.html)<sup>1</sup>
Orientador: 	[Vanderlei C. Oliveira Jr.](http://www.pinga-lab.org/people/oliveira-jr.html)<sup>1</sup>
Coorientadora:	[Valéria C. F. Barbosa](https://www.pinga-lab.org/people/barbosa.html)<sup>1</sup>

<sup>1</sup>[Observatório Nacional](http://www.gov.br/observatorio/pt-br)

Este repositório contém minha tese de doutorado, apresentada como requisito para obtenção do título de doutor em geofísica pelo Observatório Nacional.

**Este método estima a geometria de uma fonte magnética 3D a partir de dados de anomalia de campo total.**


![](complex.gif)

**Figure 1:** *Resultado de uma simulação para uma fonte com geometria complexa. Os prismas azuis representam o modelo verdadeiro enquanto os vermelhos representam o modelo estimado a cada iteração do algoritmo.*

## Resumo

Um cenário geológico geralmente inclui múltiplos corpos que produzem sinais geofísicos interferentes. Os sinais produzidos por fontes não-alvo podem ser considerados ruído geológico e devem ser suprimidos dos sinais gerados pelas fontes classificadas pelo intérprete como alvo. Uma fonte alvo pode ser considerada, por exemplo, como aquela que dá origem ao sinal geofísico mais forte, independentemente do seu valor econômico. Este trabalho apresenta um método robusto de inversão de dados magnéticos para estimar a forma e a posição de uma fonte alvo 3D na presença ou não de fontes não-alvo sem a necessidade de uma filtragem prévia. Ao assumir o conhecimento da direção de magnetização total da fonte alvo, este método recupera sua intensidade de magnetização total, posição e forma. O método aproxima a fonte alvo por um conjunto de prismas retos verticalmente justapostos, todos com o mesmo vetor magnetização total e mesma espessura. A seção horizontal de cada prisma é definida por um polígono que possui um número fixo de vértices igualmente espaçados de 0º a 360º. A posição dos vértices, a localização horizontal de cada prisma e a espessura dos prismas são os parâmetros a serem estimados durante a inversão. Esses parâmetros são obtidos por meio de uma inversão não linear regularizada em que a função desajuste é definida pela norma-1 dos resíduos. O corpo estimado neste caso é convenientemente denominado solução L1. Testes com dados sintéticos mostram uma melhor performance da solução L1 quando comparada à solução L2 (obtida usando uma função desajuste definida pelo quadrado da norma-2 dos resíduos) em recuperar a forma da fonte alvo 3D na presença de fontes não-alvo. Na ausência de sinais interferentes, as soluções L1 e L2 mostram um comportamento similar. Além disso, o método foi aplicado a um conjunto de dados produzidos por uma fonte sintética inclinada com e sem a influência de um campo regional e ambas as soluções L1 e L2 foram bem sucedidas em estimar a geometria da fonte alvo. Aplicações a dados magnéticos reais sobre os complexos alcalinos de Anitápolis, SC, e Diorama, GO, sugerem que ambos são controlados por falhas compatíveis com informações disponíveis na literatura. Diferentemente das soluções L1 e L2 obtidas para o complexo de Diorama, que sugerem a presença de fontes não-alvo relativamente grandes, aquelas obtidas para o complexo de Anitápolis indicam a presença de fontes não-alvo pequenas. Estes resultados mostram que o método pode ser uma alternativa muito eficiente na interpretação de dados magnéticos contaminados com ruído geológico.


## Publicações

Esta tese resultou em um artigo entitulado "Magnetic radial inversion for 3-D source geometry estimation" publicado na revista Geophysical Journal International.

DOI: [10.1093/gji/ggab195](http://doi.org/10.1093/gji/ggab195)

Além disso, todo o conteúdo do artigo incluindo códigos e dados utilizados encontram-se no repositório público: [![DOI](https://zenodo.org/badge/63806238.svg)](https://zenodo.org/badge/latestdoi/63806238).
