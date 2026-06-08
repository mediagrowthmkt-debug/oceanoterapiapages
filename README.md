# Oceano Terapia — Quiz Diagnóstico

Isca interativa (lead magnet) do e-book **Oceano Terapia**.
A pessoa responde 7 perguntas → recebe um diagnóstico personalizado de saturação mental → entrega os dados → recebe o e-book por e-mail.

## Publicação
Página estática (GitHub Pages). Arquivo principal: `index.html`.

## Integração GHL
Editar `CONFIG.GHL_WEBHOOK_URL` no `index.html` com a URL do Inbound Webhook/Form do GHL da Oceano Terapia.
Enquanto vazio, roda em modo demonstração (não envia, só mostra o resultado).

Campos enviados (JSON POST): `nome`, `email`, `telefone`, `perfil`, `pontuacao`, `tags[]`, `q1`..`q7`.

Feito pela MediaGrowth.
