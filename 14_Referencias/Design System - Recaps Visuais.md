---
tipo: referencia
conteudo: mestre
status: ativo
tags:
  - css
  - obsidian
  - digital-garden
  - recaps
---

# Design System — Recaps Visuais

> [!summary] Objetivo
> Apresentação editorial moderna para os recaps dos jogadores, inspirada em layouts de cartões, cenas ilustradas e momentos de destaque. **Sem substituir o ITS Theme** e sem alterar o visual das outras notas.

## Arquivos e repositórios

| Onde | Arquivo |
|---|---|
| **Vault de mestre** \`Curse-of-Strahd-Mestre\` | \`.obsidian/snippets/cos-recaps.css\` |
| **Site Digital Garden** \`Curse-of-Strahd\` | \`src/site/styles/_cos-recaps.scss\` |
| **Importação do site** | \`src/site/styles/custom-style.scss\` (linha \`@use "./cos-recaps";\`) |
| **Modelo de recap** | [[TEMPLATE - Recap Visual]] |
| **Protótipo Sessão 11** | [[Sessao 11 - Versao Cinematografica - REVISAO]] |

> [!important] Dois repositórios, um mesmo estilo
> O snippet CSS do Obsidian e o arquivo SCSS do Digital Garden contêm as mesmas regras. Alterações futuras precisam ser refletidas **nos dois**, para preservar a aparência.
>
> **Não editar** \`src/site/styles/style.scss\`: é gerado pelo template e pode ser sobrescrito.

## Ativar no Obsidian

1. Atualize/sincronize o vault para receber o arquivo \`.obsidian/snippets/cos-recaps.css\`.
2. Abra **Configurações → Aparência → Fragmentos CSS**.
3. Clique em **recarregar fragmentos**, se necessário.
4. Ative **cos-recaps**.
5. Abra o protótipo [[Sessao 11 - Versao Cinematografica - REVISAO]] em **modo Leitura**.

A propriedade opcional usada nas notas novas é:

\`\`\`yaml
cssclasses:
  - cos-recap
\`\`\`

As regras principais também reconhecem os próprios callouts \`cos-*\`, evitando que o restante do vault seja alterado.

## Publicar no Digital Garden

- Os arquivos de estilo do repositório **Curse-of-Strahd** são compilados a partir de \`custom-style.scss\` durante o build.
- Não é preciso copiar o CSS para cada nova sessão.
- Publicar a nota através do fluxo Digital Garden habitual; somente então marcar \`dg-publish: true\` e sincronizar com o repositório do site.
- Uma nota existente só muda de visual se contiver os callouts \`cos-*\`; os recaps antigos ficam iguais.
- **Protótipo da Sessão 11 permanece \`dg-publish: false\`**, não publicado no site.
- A nota oficial da Sessão 11 também permanece sem substituição até aprovação.

## Biblioteca de componentes

| Componente | Sintaxe | Melhor uso |
|---|---|---|
| **Hero** | \`> [!cos-hero] Capa\` | Abertura com arte e título |
| **Cena ilustrada** | \`> [!cos-scene] ...\` | Imagem à esquerda e texto curto |
| **Cena invertida** | \`> [!cos-scene-right] ...\` | Imagem à direita para alternância |
| **Spotlight** | \`> [!cos-spotlight] ...\` | Escolha heroica, anomalia, fala |
| **Party** | \`> [!cos-party] Nome\` | Até seis minicartões consecutivos |
| **Descoberta** | \`> [!cos-discovery] ...\` | Carta, pista, item |
| **Timeline** | \`> [!cos-timeline] ...\` | Lista numerada de três a quatro marcos |
| **Finale** | \`> [!cos-finale] ...\` | Última cena e decisão da sessão |

### Exemplo de cena

\`\`\`markdown
> [!cos-scene] O reencontro
> ![[Portal_dos_Jogadores/Imagens/Sessao11/01-aldren-na-entrada.jpg]]
>
> ### Aldren na entrada da caverna
>
> Lionel reconheceu o antigo amigo. **Mas Aldren veio prendê-lo.**
\`\`\`

**Por que callouts:** ao contrário de muitos blocos HTML, permitem que **Markdown, links \`[[wikilink]]\`, imagens \`![[arquivo]]\` e edição de conteúdo** continuem funcionando normalmente. As classes CSS cuidam da composição, não do conteúdo.

## Regras editoriais

- **Capa:** uma única frase de contexto, sem contar a sessão inteira.
- **Cenas:** geralmente 2 a 4 frases. **Evitar paredões.**
- **Spotlight:** reservar para um acontecimento que realmente mereça atenção.
- **Destaques da party:** um feito por personagem e no máximo duas linhas por cartão.
- **Timeline:** mostrar a progressão, não repetir todas as cenas.
- **Nada de duplo resumo:** não repetir a mesma descrição em três lugares diferentes.
- **Nada de segredos de mestre, voz do Oryn ou retorno do lobo previstos:** publicar só aquilo que os jogadores sabem.
- **Imagens:** usar personagens reais do projeto; nunca trocar suas identidades visuais por retratos genéricos.
- **Responsividade:** as cenas se empilham em telas pequenas; os cartões também.
- **Sem spoiler:** primeira versão privada para revisão antes de publicar.

## Sessão 11 — as quatro artes planejadas

Os comentários HTML dentro da nota de revisão guardam os locais de inserção. Quando as imagens existirem, substituir as referências pelo caminho real:

1. \`Portal_dos_Jogadores/Imagens/Sessao11/01-aldren-na-entrada.jpg\`
2. \`Portal_dos_Jogadores/Imagens/Sessao11/02-lionel-e-aldren.jpg\`
3. \`Portal_dos_Jogadores/Imagens/Sessao11/03-oryn-fogo.jpg\`
4. \`Portal_dos_Jogadores/Imagens/Sessao11/04-severin-fuga.jpg\`

**Não criar imagem fictícia nem caminho quebrado antes de os arquivos existirem.**

## Checklist de publicação

- [ ] Testar no **Obsidian / modo leitura** (desktop e janela estreita).
- [ ] Confirmar imagens reais e links.
- [ ] Conferir se os textos são públicos e fielmente baseados na sessão.
- [ ] Aprovar a versão editorial.
- [ ] Substituir a nota oficial sem perder seu permalink.
- [ ] Publicar/sincronizar pelo plugin Digital Garden.
- [ ] Conferir o link público no Vercel, incluindo mobile.
