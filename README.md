# PlayStyle Evo Helper - FC26 George Edition

Fork do userscript `PlayStyle Evo Helper` para o EA FC 26 web app.

## O que mudou neste fork

- A busca do clube agora carrega o elenco completo, sem bloquear cartas novas ou FUTTIES por lista fixa de raridades.
- O quarto `PlayStyle+` deixou de depender apenas de raridade Glory Hunters.
- A aba `4th PS+` agora procura slots da Academy de forma dinâmica, com fallback seguro por nome quando os dados estruturados não bastam.
- A validação final continua com a EA. O script só organiza a seleção local e tenta aplicar pelos serviços internos da web app.
- A telemetria original foi desativada neste fork para evitar envio silencioso de métricas a terceiros.

## Instalação

1. Instale o [Tampermonkey](https://www.tampermonkey.net/).
2. Abra o link raw do fork:
   [fc26-playstyle-evo-helper.user.js](https://raw.githubusercontent.com/georgeconsultor/fc26-playstyle-evo-helper/main/fc26-playstyle-evo-helper.user.js)
3. Confirme a instalação no Tampermonkey.
4. Abra o EA FC 26 web app e use o painel flutuante do Evo Helper.

## Como funciona

- `Single mode` para aplicar evoluções em um jogador por vez.
- `Bulk mode` para enfileirar vários jogadores.
- Sugestões por posição e função continuam ativas.
- `PlayStyle`, `PlayStyle+`, `4th PS+` e `Remove last evo` continuam disponíveis.
- O script ainda usa os serviços internos da web app, sem endpoint bruto nem chamadas HTTP extras.

## Riscos e limites

- Automatizar a web app pode violar os termos da EA e gerar punição na conta.
- A elegibilidade final de cada evolução continua sendo decidida pela EA.
- Mesmo com a lógica local ajustada, um slot só é considerado aplicável se a conta realmente tiver um slot ativo compatível.

## Observações

- Este fork foi preparado para continuar compatível com Tampermonkey.
- O script continua sendo um único userscript instalável.
- Se a EA alterar os nomes, slots ou regras internas, pode ser necessário um novo ajuste.
