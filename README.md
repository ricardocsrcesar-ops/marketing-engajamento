# Marketing e Engajamento — Sistema de Planejamento Estratégico

Sistema autocontido em HTML/CSS/JS puro (sem backend, sem build) para
planejar e avaliar marketing e engajamento em três níveis de profundidade —
**Essencial** (criador solo/MEI), **Padrão** (PME) e **Avançado** (grande
empresa) — com foco especial em **Conteúdo e Redes Sociais**: métricas reais
de performance (taxa de engajamento, salvamentos, retenção de vídeo, mix de
formato), calendário editorial por pilar, e um **painel de recomendações**
gerado automaticamente a partir dos números — nunca conselho genérico.

Cobre ainda funil RACE/AARRR, CAC/LTV, mídia paga (ROAS/CPA), RFM,
Marketing Mix Modeling, simulação Monte Carlo de aquisição, e um score de
efetividade ponderado.

Nenhum dado sai do navegador de quem preenche: tudo fica em `localStorage`,
com exportação/importação em JSON.

## Uso

Abra `index.html` diretamente no navegador — não precisa de servidor, build
ou instalação. `artifact-source.html` é a mesma aplicação, no formato exigido
para publicar como [Artifact](https://claude.ai) do Claude (sem o wrapper
`<html>/<head>/<body>` externo).

## Metodologia e sistema visual

Implementação de referência de duas skills do Claude Code, irmãs das que
implementam o [Plano de Negócios](https://github.com/ricardocsrcesar-ops/plano-de-negocios):

- **`marketing-engajamento-metodologia`** — fórmulas de métricas de
  conteúdo/redes sociais, funil, CAC/LTV, RFM, MMM, e o motor de
  recomendações (regras condicionais sobre os dados, cada uma citando a
  faixa de referência usada).
- **`marketing-engajamento-visual`** — funil, mapa perceptual, matriz RFM,
  curvas de saturação de mídia, calendário editorial, painel de
  recomendações, e a paleta de cor por assunto — estendendo o sistema de
  design `dashboard-vidro-escuro` e reaproveitando os geradores genéricos de
  `plano-de-negocios-visual`.
