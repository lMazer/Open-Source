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

No README, crie uma seção `### Nome do Projeto` com:

1. Screenshot em `docs/previews/nome-do-projeto.png` (app, diff relevante ou tela do bug)
2. Uma frase sobre o problema e a contribuição
3. Bullet **Autor** (obrigatório): nome de exibição + `@login` do GitHub humano
4. Bullet **Stack**
5. Bullet **Entrega** (o que mudou / o que o PR faz) — ou **Papel** se for acompanhamento
6. Bullet **Destaques técnicos** (até 3), quando couber
7. Bullet **Upstream** (link do repositório original)
8. Bullet **PR** / **Issue** (links clicáveis)

## 3. Autoria (obrigatório)

- Sempre credite pessoas humanas com o **nome de visualização** e o **`@login`** do GitHub.
- **Não** listar ferramentas de IA (Cursor, Copilot, ChatGPT, Claude, CodeRabbit, etc.) como autor, coautor ou colaborador.
- Se o papel for acompanhamento de PR de terceiros, deixe explícito o autor upstream do PR e o papel *Acompanhamento*.

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
### Nome do Projeto

![Preview Nome](docs/previews/nome.png)

Uma frase sobre o problema e a contribuição.

- **Autor:** [Mazer](https://github.com/lMazer) (`@lMazer`)
- **Stack:** ...
- **Entrega:** ...
- **Destaques técnicos:** ...
- **Upstream:** [`org/repo`](https://github.com/org/repo)
- **PR:** [#123](https://github.com/org/repo/pull/123) *(aberto|mergeado)*
```
