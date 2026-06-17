---
tipo: setup
tags:
  - digital-garden
  - portal-jogadores
  - mestre
---

# Setup — Digital Garden e Portal dos Jogadores

## Decisão do vault

O conteúdo público dos jogadores fica em:

```text
15_Portal_dos_Jogadores/
```

Regra principal:

> Nada de nota mista. Nota de mestre fica privada. Nota pública fica no portal.

## Frontmatter usado

Toda nota pública recebe:

```yaml
---
dg-publish: true
---
```

A home recebe também:

```yaml
dg-home: true
```

## Fluxo seguro

1. Preparar a sessão normalmente nas notas privadas.
2. Depois que os jogadores descobrirem algo, criar ou atualizar uma nota pública em `15_Portal_dos_Jogadores`.
3. Conferir se não tem spoiler.
4. Publicar pelo comando do Digital Garden.
5. Mandar o link do site para os jogadores.

## Checklist antes de publicar

- [ ] A nota está dentro de `15_Portal_dos_Jogadores`?
- [ ] A nota tem `dg-publish: true`?
- [ ] A nota não menciona estatísticas, segredos ou cenas futuras?
- [ ] Os links apontam para notas públicas do portal?
- [ ] A home `00_Inicio.md` continua com `dg-home: true`?

## Links importantes

- [[00_Inicio|Home do Portal]]
- [[Diario das Sessoes|Diário das Sessões]]
- [[Personagens do Grupo|Personagens do Grupo]]
