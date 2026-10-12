# Dashboard de Vendas – Xbox Game Pass

Dashboard em Excel que transforma dados brutos de subscrições Xbox Game Pass
(2024) em indicadores visuais para análise de faturação.

## Dados utilizados
- 295 subscrições (01/01/2024 a 16/12/2024), na folha `Bases` (tabela `Tabela1`).
- Campos: ID, nome, plano (Core/Standard/Ultimate), data de início, renovação
  automática, tipo de subscrição (Monthly/Quarterly/Annual), EA Play Season Pass,
  Minecraft Season Pass, valor do cupão e valor total.
- Total Value = preço da subscrição + EA Play + Minecraft − cupão.
- Assunção: o preço da subscrição é o mesmo para qualquer tipo de subscrição.

## Perguntas de negócio
1. Qual a faturação total de planos anuais (com subscrições agregadas)?
2. Essa faturação, separada por renovação automática e sem renovação automática.
3. Faturação total de EA Play Season Pass.
4. Faturação total de Minecraft Season Pass.

## Estrutura do ficheiro
- `Dashboard`: visão final (cartões, gráfico e segmentação por tipo de subscrição).
- `Cálculos`: tabelas dinâmicas que alimentam o dashboard.
- `Bases`: dados de origem. `Assets`: paleta de cores e imagens.
- As folhas Assets, Bases e Cálculos estão ocultas (botão direito num separador → Mostrar).

## Como reproduzir
1. Abrir `dashboard_alda.xlsx` no Excel (2016 ou superior; as segmentações exigem Excel 2010+).
2. Folha `Bases`: ver os dados. Folha `Cálculos`: ver os pivots (Dados → Atualizar tudo).
3. Folha `Dashboard`: usar a segmentação "Subscription Type" para filtrar.

## Resultado
<img width="1594" height="810" alt="image" src="https://github.com/user-attachments/assets/17674c4a-5e67-4abe-815f-4cea77a51625" />
