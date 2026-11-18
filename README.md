# Poker Privado — Texas Hold'em

Protótipo multiplayer para até 8 pessoas, com fichas virtuais, dealer automático, chat, sala privada e painel de administrador.

## Executar localmente

Instale Node.js 20+, abra o terminal na pasta e execute:

```bash
npm install
npm start
```

Acesse http://localhost:3000.

## Publicar no Render

1. Coloque esta pasta em um repositório privado no GitHub.
2. No Render, crie um **Web Service** conectado ao repositório.
3. Runtime: Node. Build command: `npm install`. Start command: `npm start`.
4. Compartilhe a URL HTTPS com os amigos; o primeiro jogador cria a sala e envia o código.

## Importante antes de usar em torneios longos

- Este é um **MVP experimental**. Faça testes de regras e jogadas antes de confiar em uma partida completa.
- As salas e fichas ficam em memória: reiniciar o servidor apaga as partidas. Para uso permanente, adicionar persistência em banco de dados.
- A identidade do administrador é guardada por um token no navegador: não compartilhe esse token.
- O serviço gratuito do Render pode dormir por inatividade, interrompendo uma partida.
- Não oferece apostas ou movimentação de dinheiro real.
