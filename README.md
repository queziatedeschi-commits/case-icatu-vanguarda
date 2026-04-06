# case-icatu-vanguarda
Analisar fundos com exposição a debêntures.
📊 Case Técnico

Coleta, Tratamento e Analytics de Fundos de Crédito Privado

 

🎯 Objetivo

Desenvolver uma solução end-to-end para coleta, tratamento e análise de dados de fundos de investimento em crédito privado, com foco específico em debêntures.

O candidato deverá construir uma aplicação (backend + frontend ou BI interativo, dependendo da abordagem escolhida) que permita:

Consolidar dados públicos de fundos
Enriquecer as carteiras com informações de mercado
Gerar análises e visualizações relevantes
Comparar fundos sob diferentes perspectivas
🧩 Escopo do Problema

O projeto consiste em três grandes etapas:

1. Coleta de Dados

Realizar a ingestão das seguintes informações públicas:

Fundos de Investimento (CVM)

Informe Diário
Cota
Patrimônio Líquido (PL)
Composição e Diversificação da Carteira
Posições em ativos (filtrar apenas debêntures)
Espera-se que o candidato implemente algum mecanismo de coleta automatizada (ex: scraping, download estruturado ou consumo de APIs públicas).

 

 

2. Enriquecimento e Tratamento de Dados

Os dados coletados deverão ser tratados e integrados com as seguintes bases auxiliares:

📁 Base 1: Cadastro de Debêntures

Contém informações estruturais dos ativos:

Código CETIP / Identificador
Emissor
Data de emissão
Indexador (CDI, IPCA, etc.)
Taxa de remuneração
Outras características relevantes
📁 Base 2: Taxas Indicativas (Anbima)

Contém histórico de mercado:

Spreads
Taxas indicativas
Duration
📁 Base 3 (a ser construída ou sugerida pelo candidato)

Classificação setorial dos emissores
Pode ser manual, baseada em regras ou enriquecida via fontes externas
3. Construção da Camada Analítica

A partir dos dados tratados, o candidato deverá estruturar análises que permitam avaliar fundos de crédito.

📈 Funcionalidades Esperadas

A solução deve permitir, no mínimo:

🔎 Análise Individual de Fundos

Para um fundo específico, apresentar:

Rentabilidade histórica (baseada na cota)
Evolução do Patrimônio Líquido (PL)
Composição da carteira (somente debêntures)
Quebras analíticas:
Por emissor
Por setor
Por indexador
Por nível de spread e/ou duration
🔄 Análise Temporal

Evolução da carteira ao longo do tempo
Movimentações relevantes:
Entrada/saída de ativos
Evolução de spreads dos ativos em carteira
Análise de abertura/fechamento de spread (mark-to-market implícito)
⚖️ Comparação entre Fundos

Permitir comparação entre dois ou mais fundos:

Rentabilidade
Diferenças na composição de carteira
Exposição por setor/emissor
Perfil de risco (ex: duration, spread médio)
💡 Geração de Insights

O candidato é incentivado a explorar os dados além do básico, por exemplo:

Identificação de concentração excessiva por emissor/setor
Relação entre spread e performance
Mudanças relevantes na estratégia do fundo
Análises que julgar pertinentes
🏗️ Requisitos Técnicos (Flexíveis, mas Avaliados)

O candidato tem liberdade de escolha tecnológica, porém será avaliado em:

Organização do código (modularização, clareza, separação de responsabilidades)
Estrutura de dados (modelagem, eficiência)
Pipeline de dados (ETL/ELT)
Qualidade das análises geradas
Clareza das visualizações
Diferenciais

Uso de APIs próprias
Interface interativa (ex: Streamlit, Dash, React, etc.)
Deploy (local ou cloud)
Documentação estruturada
📦 Entregáveis

O candidato deverá fornecer:

Código-fonte do projeto
Instruções de execução
Descrição da arquitetura e decisões técnicas
Demonstração das análises (prints, vídeo ou aplicação rodando)
🧠 O que será avaliado

Capacidade de estruturar um pipeline de dados
Qualidade da modelagem e integração das bases
Clareza na construção das análises
Capacidade de extrair insights relevantes
Organização e maturidade de engenharia
📌 Observações

Não é necessário cobrir 100% do escopo — priorização faz parte da avaliação
Assuma que os dados podem ter inconsistências
Justifique decisões técnicas sempre que possível
