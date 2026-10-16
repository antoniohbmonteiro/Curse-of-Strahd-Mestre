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
| **Party grid** | \`> [!cos-party-grid] Destaques\` | Um único callout com lista de seis itens; grid responsivo |
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
- **Destaques da party:** um feito por personagem e no máximo duas linhas por cartão. Use **um único callout `cos-party-grid` com seis itens de lista**. Não use seis callouts separados, pois o Obsidian os empilha.
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

## Cards com retratos (versão atual)

Use **um único `cos-party-grid`** com uma lista de seis itens e a imagem no começo da linha. As miniaturas ficam em `Portal_dos_Jogadores/Imagens/Personagens/Miniaturas/`, com sufixo `-head.webp`.

```markdown
> [!cos-party-grid] Destaques dos aventureiros
> - ![[Portal_dos_Jogadores/Imagens/Personagens/Miniaturas/lionel-head.webp|84]] **🛡️ Lionel** — Convenceu Aldren a guardar a espada.
> - ![[Portal_dos_Jogadores/Imagens/Personagens/Miniaturas/oryn-head.webp|84]] **🔥 Oryn** — O gelo se transformou em fogo.
```

**Imagem de avatar inline:** o CSS a posiciona à esquerda do texto com bordas arredondadas. Os cards são responsivos e não devem usar seis callouts isolados. O site precisa ter os arquivos em `src/site/img/user/Portal_dos_Jogadores/Imagens/Personagens/Miniaturas/` quando a nota for publicada.


## Novos componentes panorâmicos

O componente **cos-hero-wide** coloca a imagem horizontal 16:9 em toda a largura do card de abertura, seguida de título e subtítulo. O **cos-frame** insere uma imagem cinematográfica 16:9 entre as cenas, sem exibir título de callout. Ambos mantêm a cor e a largura do tema e não afetam outros recaps.

## Quatro quadros — Sessão 11

Na nota [[Sessao 11 - Versao Cinematografica - REVISAO]], usar estes quatro arquivos de Portal_dos_Jogadores/Imagens/Sessao11/:

1. 01-aldren-na-entrada.jpg — capa panorâmica.
2. 02-lionel-e-aldren.jpg — após a decisão de Lionel.
3. 03-oryn-fogo.jpg — após a magia inesperada de Oryn.
4. 04-severin-fuga.jpg — antes do encerramento.

Antes de publicar, confirmar que os quatro JPGs estão versionados no repositório de mestre e foram sincronizados para o site via Digital Garden. A nota de revisão permanece com dg-publish: false.
