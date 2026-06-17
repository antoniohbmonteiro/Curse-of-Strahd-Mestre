---
tipo: referencia
tags:
  - organizacao
  - vault
---

# Organização do Vault

## Regra principal

> [!note] Nota do Mestre
> Se algo pertence a uma aventura, missão ou encontro específico, fica dentro dele.  
> Se algo pode ser usado em vários lugares, fica em uma pasta global.

## Pastas

- `00_Inbox`: ideias soltas ainda sem lugar definitivo.
- `01_Controle_da_Campanha`: estado da campanha, checklist, segurança e controle geral.
- `02_Sessoes`: preparação e registro do que aconteceu em cada sessão.
- `03_Aventuras`: arcos e aventuras fechadas, como [[Casa da Morte - Hub]].
- `04_Locais`: locais globais ou recorrentes.
- `05_NPCs`: NPCs globais ou recorrentes.
- `06_Personagens_Jogadores`: fichas-resumo e ganchos dos personagens.
- `07_Monstros`: monstros custom ou variantes recorrentes.
- `08_Itens_e_Pistas_Global`: pistas/itens que podem aparecer em vários lugares.
- `09_Handouts_Global`: handouts reutilizáveis ou gerais.
- `10_Templates`: modelos do Obsidian.
- `11_Mecanicas`: mecânicas custom da campanha.
- `12_Banco_de_Encontros`: encontros soltos para encaixar na sessão.
- `13_Missoes_Custom`: missões pessoais ou criadas para sua mesa.
- `14_Referencias`: referências de preparação.
- `15_Portal_dos_Jogadores`: notas públicas para o site dos jogadores, sem spoilers.
- `99_Arquivos`: coisas antigas, testes e material que não precisa ficar na frente.

## Portal dos Jogadores

O portal público fica separado do restante do vault:

- `15_Portal_dos_Jogadores/00_Inicio.md`: home do site.
- `15_Portal_dos_Jogadores/01_Campanha`: combinados e guia público.
- `15_Portal_dos_Jogadores/02_Personagens`: versões públicas dos personagens.
- `15_Portal_dos_Jogadores/03_Mundo_Conhecido`: mundo conhecido pelos jogadores.
- `15_Portal_dos_Jogadores/04_Sessoes`: recaps públicos.
- `15_Portal_dos_Jogadores/05_Pistas_e_Handouts`: pistas, cartas e documentos revelados.

Regra: só publique notas públicas com `dg-publish: true`. Não use notas mistas com segredos de mestre.

## Casa da Morte

A Casa da Morte foi mantida como aventura própria:

- `Areas`
- `Cenas`
- `Encontros`
- `NPCs`
- `Itens_e_Pistas`
- `Handouts`
- `_assets`

## Mini-resumo no hover

Para funcionar bem com **Espiar página**, NPCs e personagens importantes têm:

```markdown
**Resumo rápido:** ...
^resumo
```

Use links assim quando quiser abrir direto no resumo:

```markdown
[[Yann Vaelor#^resumo|Yann Vaelor]]
```
