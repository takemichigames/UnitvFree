# Player IPTV — Samsung Tizen

Projeto web adaptado para navegação por:
- Controle remoto Samsung (setas, OK/Enter, Voltar e teclas de mídia quando suportadas).
- Teclado (setas, Enter, Escape/Backspace e teclas de mídia).
- Mouse e toque.

## Conteúdo
- `index.html`: player adaptado.
- `config.xml`: manifesto do aplicativo Tizen.
- `icon.png`: ícone provisório.

## Observações importantes
1. O aplicativo ainda precisa ser empacotado e assinado como `.wgt` usando o fluxo oficial do Samsung Tizen Studio/CLI.
2. `required_version` está definido para Tizen 5.5 como base inicial; confirme a versão/plataforma exata do seu modelo antes de publicar.
3. O suporte de reprodução depende dos formatos/codecs e dos servidores da playlist. HLS.js depende de MSE no navegador da TV; quando o navegador aceitar HLS nativamente, o player usa essa opção.
4. A playlist precisa permitir acesso CORS quando for carregada por `fetch()`; o app não contorna bloqueios CORS.
5. Use apenas playlists e transmissões que você tenha autorização para acessar.
