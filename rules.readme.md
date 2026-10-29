# rules.json

Três regras. Uma mexe em headers de resposta, as outras duas bloqueiam anúncios.

A **regra 1** remove `Content-Security-Policy` e `X-Frame-Options` das respostas de habblet.city. Sem ela, o renderizador de avatar do Bananablet (usado pra função de gerar visual aleatório) esbarra no CSP do hotel e não carrega, e o editor do Bananablet também não abre como iframe. Só atua em habblet.city.

As **regras 2, 3 e 4** bloqueiam pagead2.googlesyndication.com, fundingchoicesmessages.google.com e static.cloudflareinsights.com dentro do hotel. É o que faz a opção "Remover anúncios" funcionar.

Não coleta nada, não envia nada, não mexe em outros domínios.
