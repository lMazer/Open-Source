# Como adicionar uma nova contribuição à capa

Use este checklist sempre que um PR (ou contribuição relevante) entrar no índice público.

## 1. Dados mínimos

Preencha e adicione uma linha na tabela **Resumo** do [README.md](../README.md):

| Campo | Exemplo |
|-------|---------|
| Projeto | Nome do projeto upstream |
| Stack | 3–5 tecnologias principais |
| Status | Em andamento / PR aberto / Mergeado / Acompanhamento |
| Última alteração | Data do PR ou merge (`DD/MM/AAAA`) |
| Contribuição | Link do PR ou da issue |
| Autor | Nome de exibição + `@login` humanos do GitHub (ex.: [Mazer](https://github.com/lMazer) (`@lMazer`)) |

## 2. Bloco de case

No README, sob o projeto (ex.: `### BRMW`), use um `####` por contribuição com:

1. Screenshot em `docs/previews/` (quando fizer sentido; pode ser compartilhado no projeto)
2. Uma frase sobre o problema e a contribuição
3. Bullet **Autor** (obrigatório): nome de exibição + `@login` do GitHub humano — no Resumo, a coluna Autor é quem **fez o PR upstream**
4. Bullet **Stack**
5. Bullet **Entrega** (o que mudou / o que o PR faz) — ou **Papel** se for acompanhamento
6. Bullet **Destaques técnicos** (até 3), quando couber
7. Bullet **Upstream** (link do repositório original)
8. Bullet **PR** com status *(aberto · aguardando review | mergeado | fechado)* e, se útil, o título oficial do PR
9. Bullet **Fixes** (issues que o PR declara fechar) e, se houver, **Related** (contexto) — espelhar a fonte oficial (`Fixes` / `Related` no corpo do PR)
10. Se um PR substituiu outro: bullet **Histórico** com o PR antigo e o motivo (ex.: fechado, não mergeado)
11. Se o PR empilha sobre outro ainda aberto: bullet **Dependência** com o PR base

Antes de publicar ou atualizar a capa, conferir estado, título, Fixes/Related e autor na **fonte oficial** (`gh pr view` / página do PR no GitHub). Não inventar status.

## 3. Autoria (obrigatório)

- Sempre credite pessoas humanas com o **nome de visualização** e o **`@login`** do GitHub.
- **Não** listar ferramentas de IA (Cursor, Copilot, ChatGPT, Claude, CodeRabbit, etc.) como autor, coautor ou colaborador.
- Se o papel for acompanhamento de PR de terceiros: na tabela Resumo use o autor **upstream** do PR; no case, bullets **Autor do PR (upstream)** + **Papel na capa: Acompanhamento**.

## 4. Preview

- Preferir captura do app após o fix, ou do diagrama/tela afetada
- Salvar PNG em `docs/previews/`
- Referenciar no README com caminho relativo

## 5. Commit

Sugestão de mensagem:

```text
docs: adiciona [Nome do Projeto] ao índice open source
```

## Modelo rápido (copiar/colar)

```markdown
#### Título curto da contribuição (#issue)

Uma frase sobre o problema e a contribuição.

- **Autor:** [Mazer](https://github.com/lMazer) (`@lMazer`)
- **Stack:** ...
- **Entrega:** ...
- **Destaques técnicos:** ...
- **Upstream:** [`org/repo`](https://github.com/org/repo)
- **PR:** [#123](https://github.com/org/repo/pull/123) *(aberto · aguardando review)* — título upstream: *...*
- **Fixes:** [#45](https://github.com/org/repo/issues/45)
- **Related:** [#46](https://github.com/org/repo/issues/46)   <!-- só se o PR listar Related -->
```
