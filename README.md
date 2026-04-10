# Análise de Fundos de Crédito Privado

## Objetivo
Este projeto tem como objetivo analisar fundos de crédito privado com foco em debêntures, a partir da integração de diferentes bases de dados públicas, buscando avaliar:
* Relação risco vs retorno
* Estrutura e concentração da carteira
* Estratégia dos fundos ao longo do tempo
* Comparação entre fundos com perfis distintos

O escopo foi intencionalmente recortado para priorizar profundidade analítica, clareza na interpretação dos dados e construção de uma narrativa orientada a tomada de decisão.

## Bases de Dados Utilizadas
Foram utilizadas as seguintes fontes:
CVM (Composição e Diversificação da Carteira - CDA)
→ Estrutura detalhada dos ativos dos fundos
CVM (Informe Diário)
→ Dados de cota, patrimônio líquido e evolução temporal
Base ANBIMA
→ Informações de mercado como spread e duration

Além disso, foi desenvolvida uma rotina automatizada para download e extração dos dados diretamente das fontes oficiais.

## Metodologia
1. Seleção dos Fundos

A análise foi construída a partir da escolha de quatro fundos, sendo:
Dois fundos da Icatu com perfis distintos:
* Perfil mais conservador
* Perfil mais arriscado
* Dois fundos concorrentes com características similares

A classificação de risco foi baseada em métricas da carteira:
* Concentração máxima por emissor (peso principal)
* Número de emissores
* Número de ativos

Também foram aplicados filtros estruturais para garantir relevância da análise:
* Mais de 2 emissores
* Mais de 50 ativos

2. Análise de Performance

A performance foi avaliada com base nos dados do Informe Diário, considerando:
* Retorno
* Volatilidade
* Evolução da cota (normalizada na base 100)
* Crescimento do patrimônio líquido

Essa etapa permite avaliar não apenas o retorno, mas a qualidade da gestão sob a ótica risco-retorno.

3. Análise da Carteira

A estrutura da carteira foi analisada sob diferentes perspectivas:
* Concentração por emissor (Top 5)
* Diversificação da carteira
* Distribuição por setor
* Exposição por indexador

Os resultados indicam que a performance dos fundos está mais relacionada às características de crédito dos ativos (spread, risco do emissor e estrutura) do que à simples variação de indexadores como CDI ou inflação.

4. Métricas de Crédito

Para aprofundar a análise, foram consideradas métricas específicas de crédito:
* Spread médio
* Duration (exposição a prazo)

Essas métricas permitem entender o nível de risco assumido e a sensibilidade da carteira a fatores de mercado.

5. Análise Temporal

Foi realizada uma análise ao longo do tempo para identificar mudanças de estratégia dos fundos, permitindo avaliar:
* Consistência da gestão
* Alterações no perfil de risco
* Evolução da relação risco-retorno

## Principais Insights
* Fundos com maior concentração apresentam maior risco estrutural, mas podem capturar maior retorno
* A volatilidade da cota nem sempre reflete o risco real em crédito privado
* A performance dos fundos analisados mostrou maior dependência de fatores de crédito do que de indexadores macroeconômicos
* Estratégias dos fundos se alteram ao longo do tempo, impactando diretamente risco e retorno

## Conclusão
* O fundo Itaú apresentou o melhor equilíbrio entre risco e retorno no período analisado.
* O fundo Icatu Vanguarda Dinâmico também se destacou, principalmente pelo crescimento do patrimônio e forte performance, podendo ser uma alternativa relevante dependendo do perfil do investidor.

## Possíveis Evoluções
Como extensão da análise, poderiam ser incorporadas:
* Métricas de risco não linear (Drawdown, Sortino Ratio)
* Avaliação da qualidade de crédito (rating dos emissores)
* Análise mais detalhada de spread e duration ao longo do tempo
* Estudos de correlação entre fundos

## Tecnologias Utilizadas
* Python
* Pandas
* Requests
* Jupyter Notebook

## Considerações Finais
Este projeto foi desenvolvido com foco em demonstrar capacidade de estruturação de dados, construção de métricas e geração de insights relevantes para análise de investimentos em crédito privado.
