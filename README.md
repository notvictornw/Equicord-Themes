# Equicord Themes

Temas para o [Equicord](https://github.com/Equicord). Cada tema vive na sua pasta com o CSS e um README próprio. Todos suportam **atualização automática** (`@updateUrl`) — instala uma vez e o Equicord puxa as mudanças do GitHub sozinho.

```
Equicord-Themes/
├── FolderColumns/   sidebar multi-coluna (BetterFolders)
└── OperaGX/         fork otimizado do OperaGX (L-Ratio)
```

## Pré-requisitos

- Equicord instalado — https://github.com/Equicord
- [BetterFolders](https://github.com/Vendicated/BetterFolders) com a sidebar ativa (apenas para a parte multi-coluna; o resto do OperaGX funciona sem o plugin)

## Instalar

Modo recomendado — **import online** (auto-update):

1. Equicord > Settings > Themes > "Add theme" / "+".
2. Cola o URL raw do tema:
   - `https://raw.githubusercontent.com/notvictornw/Equicord-Themes/main/FolderColumns/FolderColumns.css`
   - `https://raw.githubusercontent.com/notvictornw/Equicord-Themes/main/OperaGX/OperaGX.css`
3. Ativa o tema. Quando houver mudanças no repo, o Equicord atualiza sozinho.

Modo manual (sem auto-update) — copia a pasta do tema para `%AppData%\Equicord\themes`:

```powershell
Invoke-WebRequest "https://raw.githubusercontent.com/notvictornw/Equicord-Themes/main/OperaGX/OperaGX.css" `
  -OutFile "$env:APPDATA\Equicord\themes\OperaGX.theme.css"
```

## Temas

| Tema | Plugin necessário | Notas |
|---|---|---|
| FolderColumns | BetterFolders (sidebar) | 1–4 colunas na sidebar do plugin |
| OperaGX | BetterFolders (sidebar) — só para multi-coluna | fork com perf, a11y, ~30 melhorias UX |

## Contribuir

1. Pasta nova com o nome do tema (PascalCase).
2. O `.css` lá dentro, com `@updateUrl` apontando para a raw URL.
3. Um `README.md` curto a explicar o que é, requisitos e como configurar.
4. PR.

## Autor

NotVictorNW — https://github.com/NotVictorNW
