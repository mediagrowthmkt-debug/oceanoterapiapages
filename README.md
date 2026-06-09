# Oceano Terapia, Quiz Diagnóstico

Isca interativa (lead magnet) do e-book **Oceano Terapia**.
A pessoa responde 7 perguntas → recebe um diagnóstico personalizado de saturação mental → entrega nome e WhatsApp → baixa o e-book na tela de resultado.

## Publicação
Página estática (GitHub Pages). Arquivo principal: `index.html`.

## Integração GHL
O quiz envia os leads para o webhook n8n:
`https://mediagrowth-n8n.63kuy3.easypanel.host/webhook/quiz-oceanoterapia-lead`

Workflow n8n: `[GAIA SOUL] Oceano Terapia - Quiz → GHL`.
Fluxo: cria/atualiza contato no GHL do Instituto Gaia Soul, aplica tags do quiz e cria oportunidade na pipeline `Oceano Terapia Leads`, estágio `Novo Lead`.

Campos enviados (JSON POST): `nome`, `telefone`, `perfil`, `pontuacao`, `diagnostico_texto`, `respostas_resumo`, `tags[]`, consentimento LGPD, `q1`..`q7`.

Feito pela MediaGrowth.
