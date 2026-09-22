# Como adicionar uma nova contribuição à capa

Use este checklist sempre que um PR (ou contribuição relevante) entrar no índice público.

## 1. Dados mínimos

Preencha e adicione uma linha na tabela **Resumo** do [README.md](../README.md):

| Campo | Exemplo |
|-------|---------|
| Projeto | Nome do projeto upstream |
| Stack | 3–5 tecnologias principais |
| Status | Em andamento / PR aberto / Mergeado |
| Última alteração | Data do PR ou merge (`DD/MM/AAAA`) |
| Contribuição | Link do PR ou da issue |

## 2. Bloco de case

No README, crie uma seção `### Nome do Projeto` com:

1. Screenshot em `docs/previews/nome-do-projeto.png` (app, diff relevante ou tela do bug)
2. Uma frase sobre o problema e a contribuição
3. Bullet **Stack**
4. Bullet **Entrega** (o que mudou / o que o PR faz)
5. Bullet **Destaques técnicos** (até 3)
6. Bullet **Upstream** (link do repositório original)
7. Bullet **PR** / **Issue** (links clicáveis)

## 3. Preview

- Preferir captura do app após o fix, ou do diagrama/tela afetada
- Salvar PNG em `docs/previews/`
- Referenciar no README com caminho relativo

## 4. Commit

Sugestão de mensagem:

```text
docs: adiciona [Nome do Projeto] ao índice open source
```

## Modelo rápido (copiar/colar)

```markdown
### Nome do Projeto

![Preview Nome](docs/previews/nome.png)

Uma frase sobre o problema e a contribuição.

- **Stack:** ...
- **Entrega:** ...
- **Destaques técnicos:** ...
- **Upstream:** [`org/repo`](https://github.com/org/repo)
- **PR:** [#123](https://github.com/org/repo/pull/123) *(aberto|mergeado)*
```
