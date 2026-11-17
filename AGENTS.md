# AGENTS.md — Curse of Strahd | Vault do Mestre

> **Instruções operacionais para agentes/assistentes que trabalham neste repositório.**
> Este é o vault Obsidian do mestre de uma campanha **Curse of Strahd**, D&D 5e (2024), jogada no **Foundry VTT**. Idioma de trabalho e de saída: **português brasileiro**. Prioridade: fidelidade ao que aconteceu, praticidade na mesa, continuidade, legibilidade e separação de informações.
>
> **Este arquivo não é um registro da campanha.** Consulte as notas atuais e as fontes da sessão a cada tarefa; não trate exemplos abaixo como fatos ocorridos.

## 1. Regras inegociáveis

1. **Ler antes de editar.** Verificar o estado atual do repositório, a nota de destino, notas relacionadas e referências. Nunca recriar/reescrever cegamente uma nota existente; preservar preparação, links, handouts, fatos e ajustes anteriores.
2. **Fonte curada dos PCs:** consultar primeiro o arquivo \`players.yml\` disponibilizado no projeto (ou sua versão atualizada equivalente) quando a tarefa envolve personagens jogadores, históricos, classes, ancestrais, vínculos, segredos, inventário estrutural ou builds. Se não estiver acessível, declarar a lacuna, sem inventar.
3. **Fonte de dados dinâmicos:** **Foundry VTT** — PV atual, condições, recursos/slots gastos, posição dos tokens, Inspiração aplicada e inventário em tempo de jogo. Não congelar esses números no vault como verdades permanentes; registrar apenas mudanças narrativas e itens/recursos recebidos quando confirmados.
4. **Continuidade pública:** consultar as notas e o [Diário das Sessões](https://curse-of-strahd-portal.vercel.app/sessoes/diario-das-sessoes/) quando necessário. **Só é conhecimento público aquilo que os jogadores já viram, ouviram ou descobriram** — inclusive informações de sessões que ainda não foram recapituladas.
5. **Segredo não é fato público.** Diferenciar informação do mestre, conhecimento de um PC específico, suspeitas de outros PCs e o que o grupo sabe. **Não converter hipótese em confirmação**, nem fala de jogador em fato do cenário.
6. **Transcrição não é cânone infalível.** WhisperX pode errar nomes, magias, números, falas e sobrepor vozes. Confrontar com contexto, gravações disponíveis, correções do mestre e decisões efetivamente jogadas. Se houver dúvida material, assinalar como **a confirmar**.
7. **O que aconteceu prevalece sobre o que estava preparado.** Quando os jogadores mudam a cena ou o mestre improvisa, registrar o ocorrido, não a versão prevista. Apontar diferenças relevantes sem retcon automático.
8. **Alterações pequenas.** Modificar só os arquivos necessários. Não reformatar notas alheias à tarefa, não gerar um vault completo, não publicar material público sem autorização e não alterar recaps históricos por conveniência.
9. **Separar publicação.** Uma nota com bastidores/segredos deve ter \`dg-publish: false\` ou não estar publicada. Nunca colocar segredos em arquivo dentro de \`Portal_dos_Jogadores\`.
10. **Pedir menos e entregar mais.** Quando houver fontes suficientes, produzir a nota/patch de forma prática; destacar apenas dúvidas que realmente afetem fidelidade ou cânone. Não introduzir mecânicas, motivações ou consequências novas como se já tivessem sido decididas.

## 2. Onde procurar as informações

| Necessidade | Fonte preferencial |
|---|---|
| Personagens, builds, histórias, vínculos e segredos | \`players.yml\` do projeto/versão curada mais recente; \`06_Personagens_Jogadores/\` e notas pessoais |
| Sessões ocorridas e registros internos | \`02_Sessoes/Sessao XX/\` — especialmente \`Sessao_XX_Nota_Mestre.md\` e transcrições, quando existentes |
| Eventos conhecidos pelos jogadores | \`Portal_dos_Jogadores/Sessoes/\` e o Diário das Sessões publicado |
| Notas de locais, cenas, encontros e NPCs | \`03_Aventuras/\`, \`04_Locais/\`, \`05_NPCs/\`, \`12_Banco_de_Encontros/\`, \`13_Missoes_Custom/\` |
| Itens, pistas, handouts e homebrew | \`08_Itens_e_Pistas_Global/\`, \`09_Handouts_Global/\`, \`11_Mecanicas/\` |
| Padrão de notas e callouts | \`10_Templates/\`, \`14_Referencias/Design System - Recaps Visuais.md\`, \`01_Controle_da_Campanha/Callouts - Padrão ITS para a Campanha.md\` |
| Estado do que existe no vault | GitHub do mestre: \`antoniohbmonteiro/Curse-of-Strahd-Mestre\` na branch atual |
| Estado dinâmico durante a sessão | Foundry VTT |
| Publicação pública | \`Portal_dos_Jogadores/\`, plugin Digital Garden, site em Vercel |

**Estrutura principal:** \`00_Inbox\`, \`01_Controle_da_Campanha\`, \`02_Sessoes\`, \`03_Aventuras\`, \`04_Locais\`, \`05_NPCs\`, \`06_Personagens_Jogadores\`, \`07_Monstros\`, \`08_Itens_e_Pistas_Global\`, \`09_Handouts_Global\`, \`10_Templates\`, \`11_Mecanicas\`, \`12_Banco_de_Encontros\`, \`13_Missoes_Custom\`, \`14_Referencias\`, \`99_Arquivos\`, \`Portal_dos_Jogadores\`.

**Não confiar em caminhos de documentação antiga** se contradisserem a árvore atual do repositório. Descobrir o nome/caminho real antes de inserir wikilinks.

---

## 3. Receita oficial — do áudio ao registro da sessão

**Fluxo recomendado:** transcrição → **resumo leve para revisão do mestre** → **nota do mestre completa** → seleção de pérolas → **recap visual público com pérolas no final** → aprovação → publicação/atualização do portal.

### Etapa A — Ler e reconstruir a sessão

1. Abrir o ZIP/transcrição fornecido e conferir arquivos, participantes e duração. Se houver múltiplas faixas WhisperX, **cruzar os pontos de vista**; não confundir sobreposição de falas com eventos duplicados.
2. Ler **a nota de mestre da sessão anterior** e **a preparação da cena/área** relacionada ao ponto em que o grupo parou.
3. Consultar \`players.yml\` e as notas dos PCs/NPCs quando houver relações pessoais, segredos, recursos importantes e revelações.
4. Extrair uma **linha do tempo curta** dos eventos: onde começaram, o que decidiram, o que aconteceu, quais resultados foram confirmados, onde pararam.
5. Registrar **quem presenciou o quê**. Uma cena privada de jogador não é automaticamente do conhecimento da party.
6. Registrar também **falas engraçadas, piadas internas, metagame e improvisos curiosos**, mesmo que não caibam no recap. Separar esses momentos desde a leitura para não serem esquecidos (ex.: um jogador cumprimentar o Chat).
7. Checar versões que divergem entre gravação, nota preparada e fala do mestre. **Não adivinhar**: destacar a divergência e registrar o resultado efetivamente narrado.

**Primeira entrega ao mestre (quando solicitada):** resumo direto em ordem cronológica, com acontecimentos relevantes, relações, segredos/pistas e **uma seção de bastidores e pérolas**. Essa primeira entrega **não é** ainda o recap público e não precisa ter tom literário.

### Etapa B — Criar/atualizar a NOTA DE MESTRE

**Caminho usual:** \`02_Sessoes/Sessao XX/Sessao_XX_Nota_Mestre.md\`.

- Se **não existe**, criar após confirmar na árvore do GitHub.
- Se **já existe**, ler e atualizar com cuidado. **Não apagar a preparação**. Preferir acrescentar uma seção pós-sessão ou integrar resultados verificáveis aos painéis existentes, separando \`planejado\` de \`jogado\`.
- **Uma nota principal por sessão**, fácil de consultar; não criar dezenas de subnotas sem necessidade. Cenas futuras devem continuar nas notas de área/encontro quando a consulta durante a mesa for mais rápida lá.
- Usar Markdown do Obsidian, \`[[wikilinks]]\`, callouts ITS e frontmatter. Segredos podem viver aqui porque a nota é privada.

#### Receita de conteúdo — nota concluída

**Ordem preferida** (ajustar à sessão; não forçar seções vazias):

1. **Frontmatter:** \`tipo: sessao\`, \`campanha\`, \`sessao\`, \`titulo\`, \`status: concluida\`, \`conteudo: mestre\`, \`dg-publish: false\`, local inicial/final, tags úteis.
2. **Aviso de mestre e fontes.** Identificar transcrição, notas de referência e limites de confiabilidade.
3. **PAINEL RÁPIDO — ANTES DA PRÓXIMA SESSÃO:** local exato, hora/descanso se relevante, quem está presente, NPCs, objetivos e pressões, recursos decisivos, ponto exato onde a cena parou, riscos e segredos que o mestre precisa lembrar em segundos.
4. **Linha do tempo cronológica:** tabela \`minuto do áudio → evento\` quando as marcações existirem; deixar claro que **minutos do áudio não são horas do mundo**. Priorizar ações e mudanças; evitar repetir a mesma cena em várias faixas.
5. **Cenas importantes detalhadas:** ordem de eventos, decisões, falas curtas que importam, rolagens apenas se definiram o resultado, pistas entregues, resultados da interpretação e consequências. Dar contexto suficiente para consulta meses depois, sem virar transcrição integral.
6. **Personagens e vínculos:** o que mudou entre PCs, NPCs e suas histórias pessoais; quem descobriu cada detalhe, quem apenas suspeitou e que promessa ficou sem resolução.
7. **Segredos e bastidores:** blocos **exclusivos do mestre**, identificando revelações feitas em privado, planos ainda não conhecidos, motivações ocultas e distinção entre fato/possibilidade.
8. **Mecânicas, recursos e inventário:** itens efetivamente obtidos, gastos confirmados, decisões homebrew e concessões pontuais. Marcar **a conferir no Foundry** quando necessário, em vez de inventar totais ou transformar exceção em regra.
9. **Ponto de corte e rastreador para a próxima sessão:** última cena **real** (não o plano), pendências, escolhas abertas, NPCs/ameaças, links para cenas já preparadas e o que **ainda não aconteceu**.
10. **Matéria-prima do recap público:** quais cenas merecem destaque e o que **não pode ser revelado**.
11. **Bastidores e pérolas:** candidatos com quem participou, o que ocorreu e por que foi memorável. Identificar os que podem ir à **seção final do próprio recap público da sessão**.
12. **Fontes e verificações pendentes:** referência do áudio, notas confrontadas, inconsistências e controles dinâmicos não verificados.

#### Esqueleto mínimo — nota do mestre

~~~markdown
---
tipo: sessao
campanha: Curse of Strahd
sessao: XX
titulo: "Título a confirmar"
status: concluida
conteudo: mestre
dg-publish: false
local_inicial: "[[Local Inicial]]"
local_final: "[[Local Final]]"
tags: [sessao, mestre, curse-of-strahd]
---

# Sessão XX — Título

> [!danger] CONTEÚDO DE MESTRE — NÃO PUBLICAR
> Fontes consultadas. Fatos jogados ≠ segredos ≠ hipóteses.

> [!summary] PAINEL RÁPIDO — ANTES DA SESSÃO XX+1
> **Local e momento:**
> **Quem está presente:**
> **O que acabou de acontecer:**
> **Ameaça/decisão em aberto:**
> **Estado a conferir no Foundry:**

## Linha do tempo
| Minuto do áudio | Acontecimento |
|---|---|
| 00–00 | Ação/decisão/resultados confirmados. |

## Cenas e decisões
### Cena 1
Fato jogado, ações, diálogos relevantes, consequências e links.

> [!cos-spotlight] Momento decisivo
> O que realmente mudou na história.

## Segredos e quem sabe o quê
> [!danger] SOMENTE MESTRE
> Fato privado e quem presenciou; não publicar.

## Recursos / mecânicas / itens
- Confirmados:
- Conferir no Foundry:

## Onde paramos e fios da próxima sessão
- **Última cena jogada:**
- **Ainda não aconteceu:**
- **Pendências:**

## Bastidores e pérolas
- Momento engraçado e quem participou.

## Notas para o futuro recap público
- Pode contar:
- Não revelar:
~~~

**Quando a tarefa for preparar a próxima sessão, não substitua este registro:** seguir também \`10_Templates/TEMPLATE - Sessao.md\` para objetivos, abertura/narrações, cenas prováveis, pistas, riscos, encontros e consequências **ainda não ocorridas**.

### Etapa C — PÉROLAS DA MESA no próprio recap

**Regra atual:** adicionar `## 🎭 Pérolas da Mesa` no fim do **recap público da própria sessão**, após `cos-finale` e antes da navegação. **Não criar arquivo separado para as pérolas de sessões novas.**

- Durante a leitura do áudio, registrar piadas internas, falas engraçadas, metagame, interações com o Chat e improvisos curiosos na nota do mestre, mesmo quando não entram na narrativa.
- Escolher apenas **momentos realmente acontecidos**; não inventar falas, expor segredos privados nem ridicularizar jogadores. Usar humor leve e contextualizado.
- Selecionar **2 a 4 entradas curtas**, caso haja material, com callouts CSS existentes. Artes cômicas enviadas pelo mestre devem ter **embed ativo e sem recorte indevido**, nunca ficar somente em comentários.
- O `cos-finale` fecha o capítulo dramático; as pérolas vêm em seguida, como extras, sem quebrar o clímax da história.
- **Legado:** `Portal_dos_Jogadores/Extras/Perolas da Mesa.md` contém uma pérola antiga da Sessão 11. Preservar esse arquivo histórico até que o mestre peça migração/remoção; **não colocar novos momentos nele**.
- Como qualquer parte do recap público, revisar e publicar somente após aprovação do mestre.

---

## 4. Receita oficial — recap CINEMATOGRÁFICO dos jogadores

**Caminho usual:** \`Portal_dos_Jogadores/Sessoes/Sessao XX - Recap dos Jogadores.md\`.

**Referências atuais:** \`10_Templates/TEMPLATE - Recap Visual.md\`, \`14_Referencias/Design System - Recaps Visuais.md\` e **a nota pública real da Sessão 11** (mais atual que o template em alguns componentes).

### Antes de escrever

1. **Fechar a nota de mestre** e corrigir erros de continuidade importantes.
2. Filtrar as cenas por **conhecimento público**. Um segredo de PC, mesmo conhecido pelo mestre e pelo jogador, não pode ser entregue ao resto do grupo pelo recap.
3. Escolher o **arco emocional central** e 3–5 cenas decisivas. Respeitar o protagonismo das decisões efetivas dos jogadores, não impor uma narrativa pré-determinada.
4. Escolher título, fio de abertura e **ponto de corte real**.
5. Levantar imagens existentes no vault. Não inventar arquivos, caminhos, artes ou retratos; para novas imagens, planejar o que será ilustrado e produzir/obter com aprovação do mestre.
6. **Revisar com o mestre antes de publicar.** Não atualizar automaticamente \`dg-publish\`, página inicial, diário ou site sem a etapa correspondente autorizada.

### Receita de conteúdo e composição

1. **Hero** — \`[!cos-hero-wide]\` para arte panorâmica ou \`[!cos-hero]\` para retrato. Número da sessão, título curto e abertura evocativa; **sem contar tudo logo na capa**.
2. **Timeline editorial** — \`[!cos-timeline]\` com **3–4 grandes marcos**, não a linha do tempo minuto a minuto do mestre.
3. **Corpo da história** — cenas em ordem compreensível, com prosa direta, transições naturais e detalhes importantes. Usar \`[!cos-scene]\`, \`[!cos-scene-right]\` para arte + 2–4 frases; \`[!cos-frame]\` para quadros panorâmicos completos sem repetir a legenda.
4. **Descobertas** — \`[!cos-discovery]\` para cartas, segredos revelados **em jogo**, itens e pistas importantes.
5. **Momento marcante** — \`[!cos-spotlight]\` para uma **escolha ou virada real**, não para decorar cada parágrafo.
6. **Os aventureiros** — **um único** \`[!cos-party-grid]\` com seis itens (Lionel, Svetlana/Vet, Oryn, Dhorak, Yann, Kael), miniaturas já existentes em \`Portal_dos_Jogadores/Imagens/Personagens/Miniaturas/*-head.webp\` e 1–2 linhas significativas por PC. Se alguém não participou, tratar sua ausência com fidelidade, sem inventar feito.
7. **Fios em aberto** — um \`[!cos-threads]\`, geralmente com **até quatro perguntas** a partir do que os personagens sabem. Uma hipótese pode aparecer como **pergunta**, não como verdade.
8. **Finale** — \`[!cos-finale]\` com o último acontecimento jogado, o perigo ou decisão ainda pendente, **sem narrar a próxima sessão**.
9. **Pérolas da Mesa** — após o `cos-finale`, incluir `## 🎭 Pérolas da Mesa` no **próprio recap**, com 2–4 momentos engraçados confirmados, usando os callouts CSS quando fizer sentido.
10. **Navegação** — links ao `[[Diario das Sessoes]]` e à home **depois das pérolas**.

### Padrão de linguagem

- Português brasileiro natural, imersivo mas **sem rebuscamento artificial** ou pretérito mais-que-perfeito simples.
- Capítulos curtos com títulos que ajudem a ler; cenas descritas por **ações, escolhas e consequências**, não por fichas ou uma lista de rolagens.
- Evitar **repetição** de uma mesma informação na timeline, no corpo, no destaque individual e no final.
- Não exibir resultados secretos da transcrição com frases como “sem que eles soubessem...”, se isso entregar o spoiler.
- Não assumir que algo aconteceu só porque estava preparado. **Nada de Tarokka, encontro, magia, item ou destino inventado.**
- No recap público, evitar discutir quem jogou mal, expor jogador ou ridicularizar sustos/traumas de personagem.

### Esqueleto mínimo — recap público

~~~markdown
---
dg-publish: false
dg-home: false
dg-permalink: sessoes/sessao-XX-recap-dos-jogadores
cssclasses:
  - cos-recap
tags: [recap, sessao, curse-of-strahd]
---

> [!cos-hero-wide] Capa do capítulo
> ![[CAMINHO_DE_IMAGEM_VERIFICADO]]
>
> **CURSE OF STRAHD · SESSÃO XX**
>
> ## Título
>
> Uma frase de abertura.

> [!cos-timeline] A sessão em três momentos
> 1. **Primeiro** — Mudança.
> 2. **Segundo** — Decisão.
> 3. **Terceiro** — Consequência.

## Primeira cena
Texto curto, com os fatos públicos.

> [!cos-scene] Uma cena real
> ![[OUTRO_CAMINHO_VERIFICADO]]
>
> ### Título
>
> Duas a quatro frases.

> [!cos-spotlight] O momento
> ### Uma escolha que importou
> Consequência.

## ⭐ Os aventureiros
> [!cos-party-grid] Destaques dos aventureiros
> - ![[Portal_dos_Jogadores/Imagens/Personagens/Miniaturas/lionel-head.webp|84]] **🛡️ Lionel** — Feito.
> - ... completar as seis entradas com as miniaturas reais ...

## 🧩 Fios em aberto
> [!cos-threads] Fios em aberto
> - **🌫️ Mistério** Uma pergunta pública ainda sem resposta.

> [!cos-finale] Próximo capítulo
> ### Onde paramos
> Última cena realmente jogada.

## 🎭 Pérolas da Mesa
> [!cos-discovery] 🪓 Uma história engraçada da sessão
> Um momento realmente registrado, sem spoilers.

[[Diario das Sessoes|← Diário das Sessões]]
~~~

**Importante:** caminhos \`CAMINHO_DE_IMAGEM_VERIFICADO\` e \`OUTRO_CAMINHO_VERIFICADO\` acima são **marcadores de instrução**, não devem ser colocados numa nota final. Se a arte não existe, **omitir o embed ou planejar antes de publicar**.

---

## 5. Visual e CSS: ITS Theme + WOTC/D&D Beyond

O Obsidian usa o **ITS Theme** com a opção visual **WOTC/D&D Beyond**. **Dar preferência aos componentes CSS personalizados já existentes no vault** sempre que melhorarem organização, leitura ou apresentação, também nas notas de mestre. Usar Markdown limpo e wikilinks; recorrer aos callouts tradicionais do ITS como complemento para informações técnicas, avisos e segredos. **Não criar CSS customizado novo por padrão**: primeiro verificar o que o tema e os snippets já oferecem.

**Arquivos de estilo atuais:**

- Vault/Obsidian: \`.obsidian/snippets/cos-recaps.css\`
- Digital Garden/site (repositório \`antoniohbmonteiro/Curse-of-Strahd\`): \`src/site/styles/_cos-recaps.scss\`, importado por \`src/site/styles/custom-style.scss\`.
- Guia: \`14_Referencias/Design System - Recaps Visuais.md\`.

**Componentes \`cos-*\` existentes** (verificar código antes de usar variantes novas):
\`cos-hero\`, \`cos-hero-wide\`, \`cos-hero-portrait\`, \`cos-scene\`, \`cos-scene-right\`, \`cos-frame\`, \`cos-spotlight\`, \`cos-discovery\`, \`cos-timeline\`, \`cos-party-grid\`, \`cos-threads\`, \`cos-finale\` (há também \`cos-party\` legado).

**REGRAS DE USO:**

- **Para recap público visual:** aplicar os componentes \`cos-*\` deliberadamente, como na Sessão 11, e \`cssclasses: [cos-recap]\` no frontmatter. Preferir poucos componentes bem escolhidos a excesso de cartões.
- **Para nota do mestre:** **priorizar o Design System e os callouts personalizados `cos-*` quando contribuírem para a leitura e a consulta rápida** — não reservar os estilos novos apenas aos recaps públicos. Usar `\`[!cos-timeline]\`` para marcos de orientação (3–4 eventos), `\`[!cos-spotlight]\`` para decisões importantes e `\`[!cos-discovery]\`` para pistas ou revelações, conforme o conteúdo. Complementar com os callouts tradicionais `\`[!summary]\``, `\`[!warning]\``, `\`[!danger]\``, `\`[!note]\``, `\`[!recite]\`` e `\`[!info]\`` para controle de mesa, avisos e bastidores. **Legibilidade e consulta rápida vencem decoração**: não forçar hero, miniaturas ou grid da party numa nota técnica, nem encher a página de cartões redundantes. O CSS dos callouts `\`cos-*\`` se aplica mesmo sem `\`cssclasses: cos-recap\``.
- **Não embutir tabelas gigantes dentro de \`cos-timeline\`**: a cronologia detalhada pertence a uma tabela Markdown normal; o callout visual pode apresentar um resumo de 3–4 marcos separado.
- **Usar seções recolhíveis** \`[!danger]-\` para segredos de mestre quando facilitar consulta e segurança visual. Não confundir o recolhimento com proteção de acesso: ele **não torna pública uma nota segura**.
- **Não inventar componente sem CSS**. Evitar HTML/CSS ad hoc se um callout existente cumpre a função.
- **Não criar imagens só para preencher layout**; verificar que o embed realmente aponta a arquivo existente. Para imagens de personagens, preservar identidade visual e retratos estabelecidos.
- **Imagens entregues pelo mestre via ZIP/arquivo local:** quando o arquivo final e seu caminho no vault já foram definidos, inserir **embed ativo** `![[caminho/arquivo.jpg]]` diretamente no Markdown (inclusive dentro de callouts). **Nunca deixar a imagem apenas em comentário HTML ou placeholder e dizer que ela já foi integrada.** Se a imagem ainda não estiver no GitHub, avisar separadamente que precisa ser extraída/sincronizada; a ausência temporária no repositório não justifica esconder o embed no rascunho.
- **CSS do site e snippet devem continuar equivalentes** quando houver alteração de estilo; não modificar apenas um lado. **Não editar** \`src/site/styles/style.scss\`, que é gerado.
- O guia de design e o CSS atuais são a referência quando algum exemplo antigo deste arquivo ficar desatualizado.

## 6. Notas de áreas, encontros, NPCs e homebrew

- Preparação de sessão **não deve duplicar notas de áreas**. Quando a informação será necessária durante uma cena específica, preferir adicioná-la em \`04_Locais/\`, \`03_Aventuras/\` ou no encontro correspondente, com links na nota da sessão.
- Para cenas, preparar: **gatilho → narração curta → opções dos PCs → testes/mecânicas → pistas → consequências → estado após a cena**. Manter segredos em blocos de mestre.
- Recompensar soluções inesperadas e escolhas significativas. Preparação não obriga resultado.
- Mudanças de regra/homebrew só são regras permanentes quando aprovadas pelo mestre; concessões da mesa podem ser casos isolados.
- Consultar a **D&D 5e (2024)** correta, e não misturar com regra 2014 sem avisar; Foundry é referência do que está configurado na mesa.
- Imagens, tokens, mapas, som, combate e handouts visuais ficam no Foundry. O Obsidian serve como **caderno de mestre e wiki viva**, não substitui o estado atual do jogo.

## 7. Checklist obrigatório antes de entregar qualquer arquivo

- [ ] Li a versão **atual** de cada arquivo modificado no GitHub?
- [ ] Conferi a **fonte primária** da sessão e a continuidade das sessões anteriores?
- [ ] Mantive separação entre **fato, hipótese, segredo e preparação**?
- [ ] O ponto em que a sessão parou está **exato** e sem antecipações?
- [ ] As revelações só estão no material que o respectivo público pode ver?
- [ ] A nota de mestre possui **painel rápido**, cronologia, consequências e pendências?
- [ ] Registrei **pérolas e interações metagame** em seção própria para o mestre avaliar?
- [ ] As pérolas aprovadas ficaram **no final do próprio recap**, após o finale, sem duplicação em documento separado?
- [ ] **Priorizei os componentes CSS personalizados existentes** quando melhoram a nota, usando callouts ITS tradicionais como complemento e sem sacrificar a consulta rápida?
- [ ] Todos os \`[[wikilinks]]\`, caminhos de imagens e referências existem ou foram marcados como pendentes?
- [ ] Conferi se o status **\`dg-publish\`** corresponde à intenção?
- [ ] Evitei sobrescrever preparação, reescrever arquivos históricos e criar conteúdo fora de escopo?
- [ ] Verifiquei o **resultado do commit/escrita** antes de afirmar que foi salvo?

## 8. Publicação e atualização do portal

**Somente depois de aprovação do mestre**, conforme a tarefa:

1. Finalizar e revisar o recap público, incluindo imagens/callouts e exclusão de spoilers.
2. Garantir frontmatter e **permalink estável**; não alterar URL de sessão já publicada sem necessidade.
3. Se solicitado, atualizar \`Portal_dos_Jogadores/Sessoes/Diario das Sessoes.md\` e \`Portal_dos_Jogadores/00_Inicio.md\` com a nova sessão.
4. Publicar/sincronizar via **plugin Digital Garden do Obsidian** e verificar Vercel quando possível. **Um commit só no vault de mestre não implica que o portal foi publicado automaticamente.**
5. Conferir visual desktop/mobile, miniaturas, títulos, callouts, links e se não vazou segredo de mestre.
6. Reportar objetivamente: **o que mudou, em quais arquivos, o que está publicado e o que ainda depende de sincronização**.

**Prioridade final:** uma sessão bem documentada permite ao mestre entender rapidamente **o que aconteceu, o que cada personagem sabe e qual decisão vem agora**. O recap público permite aos jogadores **reviver a sessão sem spoilers**, com **Pérolas da Mesa ao final do mesmo recap**, sem arquivo paralelo por sessão.
