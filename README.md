# vigia

Confere a cada 15 minutos se os sites da Casa dos Fundos respondem (cardápio, sistema, caixa,
conversa do caixa e o WhatsApp automático). Se algum ficar fora depois de 3 tentativas, a
execução falha e o GitHub manda e-mail para o dono.

É público de propósito: repositório público não gasta minutos do GitHub Actions. Não tem
código da loja nem senha, só a lista de endereços em `.github/workflows/vigia.yml`.

O `manter-ativo.yml` faz um commit vazio todo dia 1: sem commit em 60 dias o GitHub desliga
o agendamento de repo público.

Conferência mais completa, feita à mão: `python3 pdv-balcao/scripts/deploy-easypanel.py --conferir`.
