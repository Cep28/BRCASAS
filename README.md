# BRCASAS · Painel de Fluxo de Caixa do Portfólio

Aplicação web para **acompanhamento dos resultados** e **inserção de novas premissas** do
fluxo de caixa de um portfólio de 9 incorporações imobiliárias (MCMV / Crédito Associativo),
na ótica **já incorrido × a incorrer** (data-base 08/06/2026, base nominal).

## Como usar

Abra o arquivo [`index.html`](index.html) no navegador — não precisa instalar nada, roda
100% offline. Também pode ser publicado no GitHub Pages.

### Funcionalidades

- **Visão geral** — KPIs consolidados (unidades, VGV, receita, saídas, resultado líquido,
  exposição máxima) e gráficos por obra (resultado, exposição de caixa, receita × saídas, unidades).
- **Obras & premissas** — quadro resumo + cartões editáveis. Edite qualquer premissa
  (unidades, VGV, receita, saídas, já incorrido, exposição, TIR, cronograma) ou
  **adicione uma nova obra**. O resultado (`Receita − Saídas − Já incorrido`) e o
  múltiplo (`Resultado ÷ Exposição + 1`) recalculam automaticamente.
- **Curva de caixa** — modelo mês a mês (curva S) a partir das premissas: gráfico do caixa
  acumulado no tempo por obra ou consolidado, com o pico de exposição calibrado à exposição
  oficial do relatório e a TIR do modelo como estimativa ilustrativa.
- **Acompanhamento** — lance o realizado (% de obra, unidades vendidas, receita e saídas
  realizadas) e compare previsto × realizado, incluindo **meta de vendas acumulada** até o
  mês de referência (velocidade × meses desde o início das vendas).
- **Parâmetros** — premissas globais editáveis (INCC, velocidade de vendas, taxa SAC, repasse
  CEF), parâmetros da curva de caixa e o modelo de venda MCMV.

### Dados

Os dados ficam salvos no **navegador (localStorage)**. Use os botões do topo para
**Exportar** / **Importar** (JSON) ou **Restaurar padrão** (recarrega as 9 obras originais).

## Portfólio (data-base 08/06/2026)

9 empreendimentos · 5.603 unidades · VGV R$ 1,49 bi · Receita R$ 1,81 bi ·
Resultado líquido projetado R$ 488 mi · Exposição máx. somada R$ 68,2 mi.

Fonte: relatórios de viabilidade econômico-financeira (RExSoft).
