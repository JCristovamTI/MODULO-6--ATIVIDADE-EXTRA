**PLANEJAMENTO ESTRATÉGICO ANALÍTICOS ((PEA)**

Projeto:\_**\_** Equipe: \_**\_**\____  
Data: \_**\_**\__/ \_**\_** / \_**\_**_

**1 · ENTENDER**

| **1\. Contexto e Problema <br>**Operação com vendas volumosas mas prejuízos severos e recorrentes concentrados em subcategorias específicas (ex: Cadeiras/Mesas) causados por políticas de descontos excessivos que chegam a 50%. | **2\. Objetivo e Decisão <br>**Identificar os limites saudáveis de desconto por subcategoria e região para subsidiar a nova política comercial e estancar a erosão de margem de lucro sem sacrificar volume crítico. | **3\. Perguntas Analíticas (Resumo) <br>**• Quais subcategorias têm margem negativa? <br>• Qual o impacto financeiro real do frete/envio? <br>• Que faixa de desconto maximiza o lucro real? <br>• Quais clientes concentram as perdas? |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

**2 · CONSTRUIR**

| **4\. Dados e Fontes <br>**• D1: Histórico de Vendas Superstore (CSV) <br>• Situação: Estruturado, contendo Sales, Profit, Discount, Region e Ship Mode. Necessita saneamento de outliers e classificação de margem. | **5\. Indicadores Principais <br>**• I1: Margem de Lucro (%) <br>Cálculo: \[Profit\] / \[Sales\] <br>• I2: Desconto Médio (%) <br>Cálculo: Média de \[Discount\] <br>• I3: Lucro Acumulado (\$) <br>Cálculo: Soma de \[Profit\] | **6\. Entregas Prometidas <br>**• E1: Painel Interativo de Rentabilidade Comercial (Power BI) com árvore de decomposição. <br>• E2: Relatório de Recomendações de Alocação de Desconto por Região. |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

**3 · ADOTAR**

| **7\. Público e Uso <br>**• Quem usa: Diretoria Comercial, Controladoria e Gerentes Regionais. <br>• Como: Ajustes mensais de metas e travas automáticas de desconto no ERP para fretes não saudáveis. | **8\. Riscos e Premissas <br>**• Risco: Resistência da força de vendas ao corte de descontos. <br>• Premissa: O volume de vendas não cairá drasticamente se o desconto for reduzido em subcategorias líderes. | **9\. Próximos Passos (Ações) <br>**☐ Tratamento e carga no Power BI \[BI/Analista\] \[Prazo: D+3\] <br>☐ Homologação dos cálculos com Controladoria \[Finanças\] \[Prazo: D+5\] <br>☐ Workshop de adoção do painel \[Todos\] \[Prazo: D+10\] |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

**MATRIZ DE PERGUNTAS ANALÍTICAS (Focada em Rentabilidade Crítica)**

| **#** | **Pergunta Analítica**                                                                           | **Página/Seção**   | **Indicador Principal**               | **Filtros Recomendados**     | **Visualização Provável**                       |
| ----- | ------------------------------------------------------------------------------------------------ | ------------------ | ------------------------------------- | ---------------------------- | ----------------------------------------------- |
| **1** | Quais subcategorias e produtos específicos acumulam o maior prejuízo operacional da base?        | Visão Geral        | Soma de Profit (Lucro)                | Categoria, Subcategoria, Ano | Gráfico de Barras (Ranking Pior para Melhor)    |
| **2** | Existe correlação direta entre o aumento do desconto e a queda vertical da margem de lucro?      | Análise Comercial  | % Margem de Lucro vs % Desconto Médio | Região, Segmento             | Dispersão (Scatter Plot) com Linha de Tendência |
| **3** | Quais estados ou cidades combinam alto volume de vendas (Sales) com margens altamente negativas? | Mapa de Perdas     | Soma de Sales e Lucro Médio           | Subcategoria, Ano            | Mapa de Calor Coroplético (Cores divergentes)   |
| **4** | Qual é o impacto financeiro dos modos de envio (Ship Mode) no lucro de itens pesados?            | Logística & Frete  | Custo Estimado e Lucro por Envio      | Ship Mode, Região            | Gráfico de Colunas Agrupadas                    |
| **5** | Qual o perfil de segmento de cliente (Segment) que mais usufrui de descontos nocivos à margem?   | Segmentação        | Ticket Médio e Taxa de Desconto       | Segmento, Categoria          | Gráfico de Rosca ou Treemap                     |
| **6** | Qual o valor limite ideal de desconto (%) antes que o produto passe a gerar prejuízo real?       | Simulação / Margem | Ponto de Equilíbrio (Break-even %)    | Subcategoria, Região         | Gráfico de Linhas (Sensibilidade de Desconto)   |

**Checklist de Revisão Estratégica:**

**☐ Impacto Comercial:** A pergunta analítica expõe claramente o gargalo que reduz a margem?

**☐ Viabilidade do Indicador**: Os dados de entrada (Sales/Profit) estão saneados e batem com o balanço controladoria?

**☐ Acionabilidade Prática:** A decisão gerada pela resposta pode ser automatizada via regra de negócio ou trava no ERP?

**☐ Adoção Garantida:** O usuário final (Gerente/Diretor) validou se o formato visual proposto é de fácil e rápida leitura?