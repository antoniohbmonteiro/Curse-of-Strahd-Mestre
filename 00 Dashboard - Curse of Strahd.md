---
tipo: dashboard
campanha: Curse of Strahd
sistema: D&D 5e 2024
vtt: Foundry
tags:
  - cos
  - dashboard
---

# Curse of Strahd — Dashboard

> [!recite] Tom da campanha
> A névoa não leva os personagens para outro lugar. Ela os leva para uma resposta que ninguém queria receber.

## Abrir antes da sessão

- [[01_Controle_da_Campanha/Estado Atual da Campanha]]
- [[02_Sessoes/Log de Campanha]]
- [[02_Sessoes/Sessao 00 - Setup e Entrada na Névoa]]
- [[03_Aventuras/Casa da Morte/Casa da Morte - Hub]]
- [[06_Personagens_Jogadores/Grupo - Personagens]]
- [[01_Controle_da_Campanha/Checklist Foundry]]
- [[01_Controle_da_Campanha/Linhas, Veus e Intensidade]]

## Portal dos Jogadores

- [[00_Inicio|Home do Portal dos Jogadores]]
- [[01_Controle_da_Campanha/Setup - Digital Garden e Portal dos Jogadores]]
- [[Diario das Sessoes|Diário Público das Sessões]]
- [[Personagens do Grupo|Personagens Públicos]]

## Sessão atual

> [!info] Foco imediato
> **Objetivo:** apresentar Baróvia, reunir o grupo e iniciar a Casa da Morte.  
> **Tom:** frio, confusão, perda de controle, crianças assustadas, uma casa que parece esperar.  
> **Promessa da cena:** eles podem escolher como entrar, mas Baróvia cobra o preço de ignorar pedidos de socorro.

## Casa da Morte

- [[03_Aventuras/Casa da Morte/Casa da Morte - Hub]]
- [[03_Aventuras/Casa da Morte/Cenas/00 - Entrada na Névoa]]
- [[03_Aventuras/Casa da Morte/Cenas/01 - Rose and Thorn na Rua]]
- [[03_Aventuras/Casa da Morte/Cenas/02 - Fachada da Casa]]
- [[03_Aventuras/Casa da Morte/Cenas/03 - Primeira Exploracao]]
- [[03_Aventuras/Casa da Morte/Encontros/Encontro - Convencer as Crianças]]
- [[03_Aventuras/Casa da Morte/Encontros/Encontro - A Casa Fecha a Saida]]
- [[03_Aventuras/Casa da Morte/Itens_e_Pistas/Pistas - Casa da Morte]]

## Jogadores

- [[Svetlana#^resumo|Svetlana]]
- [[Kael Varzhen#^resumo|Kael Varzhen]]
- [[Lionel Roarshield#^resumo|Lionel Roarshield]]
- [[Dhorak Khal#^resumo|Dhorak Khal]]
- [[Oryn Fizzlestryke#^resumo|Oryn Fizzlestryke]]
- [[Yann Vaelor#^resumo|Yann Vaelor]]

## Ferramentas de mestre

- [[11_Mecanicas/_Mecanicas - Indice]]
- [[Fome Dhampyr do Yann]]
- [[12_Banco_de_Encontros/_Banco de Encontros - Hub]]
- [[13_Missoes_Custom/_Missoes Custom - Hub]]
- [[14_Referencias/_README]]

## Ideias soltas

- [[00_Inbox/Ideia - Barovia reconhece os personagens]]
- [[00_Inbox/Ideia - A Casa testa cada personagem]]

## Consultas Dataview opcionais

```dataview
LIST
FROM "02_Sessoes"
WHERE tipo = "sessao"
SORT file.name ASC
```

```dataview
LIST
FROM "08_Itens_e_Pistas_Global_Global" OR "03_Aventuras/Casa da Morte/Itens_e_Pistas"
WHERE status != "entregue"
SORT prioridade DESC
```

```dataview
LIST
FROM "12_Banco_de_Encontros" OR "13_Missoes_Custom" OR "11_Mecanicas"
WHERE tipo
SORT file.name ASC
```
