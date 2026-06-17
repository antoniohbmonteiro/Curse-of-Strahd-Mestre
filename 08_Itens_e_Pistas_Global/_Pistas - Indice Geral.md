---
tipo: indice
tags:
  - pistas
---

# Índice Geral de Pistas

## Ativas

```dataview
TABLE prioridade, status
FROM "08_Itens_e_Pistas_Global_Global" OR "03_Aventuras"
WHERE tipo = "pista" AND status != "entregue"
SORT prioridade DESC
```

## Regras

- Toda cena importante precisa de pelo menos 3 pistas.
- Pista boa aponta para decisão, não só para lore.
- Se os jogadores travarem, entregue pista sensorial.
- Se os jogadores arriscarem, entregue pista clara.
