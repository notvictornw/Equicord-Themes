# OperaGX (NotVictorNW Fork)

Fork do OperaGX do [Hawk/L-Ratio](https://github.com/L-Ratio/OperaGXTheme) com otimizações de performance, acessibilidade e ~30 melhorias de UX.

## Pré-requisitos

- Equicord instalado — https://github.com/Equicord
- [BetterFolders](https://github.com/Vendicated/BetterFolders) com a sidebar ativa — só para a parte multi-coluna. O resto do tema funciona sem o plugin.
- **Internet** — o tema carrega a base do L-Ratio via CDN e a fonte Chakra Petch do Google Fonts. Sem internet, só a camada de overrides aparece.

## O que mudou face ao original

**Performance**
- Animar só `transform` / `opacity` / `filter` (GPU); nada de `box-shadow` ou `width` animados.
- Sem `backdrop-filter`. `will-change` só no hover.
- `content-visibility: auto` em listas longas (mensagens, canais).

**Acessibilidade**
- `@layer` para organizar o cascade — `!important` só onde o Discord obriga.
- `prefers-reduced-motion` e `prefers-contrast: more` tratados.

**UX**
- FolderColumns integrado nativamente (multi-coluna na sidebar do BetterFolders).
- Status indicator com ring, account panel redesenhado, popout/modal de perfil estilo GX, tudo arredondado, replies com accent, mentions pill animada, unread pulse, call ring, toasts com slide, etc.

## Instalação

Recomendado — import online (auto-update): em Equicord > Settings > Themes cola
`https://raw.githubusercontent.com/notvictornw/Equicord-Themes/main/OperaGX/OperaGX.css`

Ou copia o `OperaGX.css` para `%AppData%\Equicord\themes` e ativa em Settings > Themes (sem auto-update).

(Opcional) Ativa o BetterFolders e liga a sidebar para ter colunas.

## Configuração

Pelo modal Edit:

| Variável | Descrição | Default | Min | Max |
|---|---|---|---|---|
| `server_listing_width_s` | Largura da barra (62/126/184/242 = 1–4 colunas) | 126 | 62 | 242 |
| `guildsize_s` | Tamanho do ícone do servidor | 50 | 10 | 200 |
| `guildgap_s` | Gap entre ícones | 3 | 0 | 25 |

Cores, fontes, transparências e raios ficam em `:root` no topo do CSS — edita diretamente se quiseres mudar o vermelho GX ou a fonte.

## Suporte

Discord: [9EqSdYTyCK](https://discord.gg/9EqSdYTyCK)

## Créditos

Original: Hawk/L-Ratio — https://github.com/L-Ratio/OperaGXTheme
Fork: NotVictorNW
