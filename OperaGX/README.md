# OperaGX (NotVictorNW Fork)

Fork do OperaGX do [Hawk/L-Ratio](https://github.com/L-Ratio/OperaGXTheme) com otimizações de performance, acessibilidade e ~30 melhorias de UX.

## O que mudou face ao original

- Animar só `transform` / `opacity` / `filter` (GPU), nada de `box-shadow` ou `width` animados.
- Sem `backdrop-filter`. `will-change` só no hover.
- `@layer` para organizar o cascade — `!important` só onde o Discord obriga.
- `prefers-reduced-motion` e `prefers-contrast: more` tratados.
- `content-visibility: auto` nas listas longas (mensagens, canais).
- FolderColumns integrado nativamente (precisa do BetterFolders com sidebar).
- Status indicator com ring, account panel redesenhado, popout/modal de perfil estilo GX, tudo arredondado, replies com accent, mentions pill animada, unread pulse, call ring, toasts com slide, etc.

## Requisitos

- Equicord.
- BetterFolders com a sidebar ativa — só para a parte multi-coluna. O resto funciona sem o plugin.

## Instalação

Recomendado — import online (auto-update): em Equicord > Settings > Themes cola
`https://raw.githubusercontent.com/VictorNieworld/Equicord-Themes/main/OperaGX/OperaGX.css`

Ou copia o `OperaGX.css` para `%AppData%\Equicord\themes` e ativa em Settings > Themes (sem auto-update).

(Opcional) Ativa o BetterFolders e liga a sidebar para ter colunas.

## Configurar

Pelo modal Edit:

- **server_listing_width_s** — 62 / 126 / 184 / 242 = 1–4 colunas
- **guildsize_s** — tamanho do ícone (50)
- **guildgap_s** — gap entre ícones (3)

Cores, fontes, transparências e raios ficam em `:root` no topo do CSS — edita diretamente se quiseres mudar o vermelho GX ou a fonte.

## Créditos

Original: Hawk/L-Ratio — https://github.com/L-Ratio/OperaGXTheme
Fork: NotVictorNW
