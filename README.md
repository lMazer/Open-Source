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

Contribuição ao [brmodelo-app](https://github.com/brmodeloweb/brmodelo-app) (ferramenta livre de modelagem ER usada em cursos de banco de dados): restauração da edição de cardinalidade nos editores conceitual e lógico, sincronização de FK ao mudar 1:1/1:N, export/import JSON do modelo, e geração SQL mais confiável.

- **Stack:** React 19, TypeScript, JointJS (`@joint/core`), Webpack 5, pnpm
- **Entrega:** PR que permite selecionar links pelo clique, editar cardinalidade com sync de FK, importar/exportar `.brmw.json`, endurecer SQL (`REFERENCES` pela PK, copiar/baixar, validação) e manter dirty/`cross-env` no Windows
- **Destaques técnicos:** `link:pointerclick` + tools persistentes; `logicalCardinality` + `syncForeignKeyForLink`; `modelFileIO` e validação SQL
- **Upstream:** [`brmodeloweb/brmodelo-app`](https://github.com/brmodeloweb/brmodelo-app)
- **PR:** [#716](https://github.com/brmodeloweb/brmodelo-app/pull/716) *(aberto)*
- **Issues:** [#706](https://github.com/brmodeloweb/brmodelo-app/issues/706), [#714](https://github.com/brmodeloweb/brmodelo-app/issues/714), [#713](https://github.com/brmodeloweb/brmodelo-app/issues/713), [#386](https://github.com/brmodeloweb/brmodelo-app/issues/386), [#693](https://github.com/brmodeloweb/brmodelo-app/issues/693), [#626](https://github.com/brmodeloweb/brmodelo-app/issues/626), [#715](https://github.com/brmodeloweb/brmodelo-app/issues/715)

## Padrões que sigo

- Respeitar Code of Conduct e convenções do projeto upstream
- Preferir issues claras e reproduzíveis antes de abrir PR
- Branches `fix/`, `feature/` ou `enhancement/` a partir de `main`
- Commits com prefixo (`Fix:`, `Feat:`, `Docs:`, …) quando o projeto pedir
- Documentar na capa o link do PR e o status (aberto / mergeado)

## Como adicionar uma nova contribuição

Siga o template em [docs/ADDING_A_PROJECT.md](docs/ADDING_A_PROJECT.md).
