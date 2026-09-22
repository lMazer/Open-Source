# Open Source

Índice público de contribuições em projetos **open source**.

Este repositório é uma **capa de portfólio**: documenta PRs, issues e contexto técnico. O código das contribuições fica nos repositórios **upstream** (e, durante o trabalho, no fork).

## Resumo

| Projeto | Stack | Status | Última alteração | Contribuição |
|---------|-------|--------|------------------|--------------|
| BRMW | React 19, TypeScript, JointJS, Webpack | PR aberto | 22/09/2026 | [#716](https://github.com/brmodeloweb/brmodelo-app/pull/716) |

## Cases

### BRMW

![Preview BRMW](docs/previews/brmw.png)

Contribuição ao [brmodelo-app](https://github.com/brmodeloweb/brmodelo-app) (ferramenta livre de modelagem ER usada em cursos de banco de dados): correção para a alteração de cardinalidade no modelo lógico ser de fato salva, e scripts npm compatíveis com Windows.

- **Stack:** React 19, TypeScript, JointJS (`@joint/core`), Webpack 5, pnpm
- **Entrega:** PR que marca o modelo como `dirty` ao editar labels de cardinalidade e troca `export NODE_ENV` por `cross-env`
- **Destaques técnicos:** `change:labels` no graph events; `setDirty` em `editCardinalityA/B`; `pnpm run:fe` funcional no Windows
- **Upstream:** [`brmodeloweb/brmodelo-app`](https://github.com/brmodeloweb/brmodelo-app)
- **PR:** [#716](https://github.com/brmodeloweb/brmodelo-app/pull/716) *(aberto)*
- **Issues:** [#714](https://github.com/brmodeloweb/brmodelo-app/issues/714), [#713](https://github.com/brmodeloweb/brmodelo-app/issues/713), [#386](https://github.com/brmodeloweb/brmodelo-app/issues/386)

## Padrões que sigo

- Respeitar Code of Conduct e convenções do projeto upstream
- Preferir issues claras e reproduzíveis antes de abrir PR
- Branches `fix/`, `feature/` ou `enhancement/` a partir de `main`
- Commits com prefixo (`Fix:`, `Feat:`, `Docs:`, …) quando o projeto pedir
- Documentar na capa o link do PR e o status (aberto / mergeado)

## Como adicionar uma nova contribuição

Siga o template em [docs/ADDING_A_PROJECT.md](docs/ADDING_A_PROJECT.md).
