# Open Source

Índice público de contribuições em projetos **open source**.

Este repositório é uma **capa de portfólio**: documenta PRs, issues e contexto técnico. O código das contribuições fica nos repositórios **upstream** (e, durante o trabalho, no fork).

## Resumo

| Projeto | Stack | Status | Última alteração | Contribuição |
|---------|-------|--------|------------------|--------------|
| BRMW | React 19, TypeScript, JointJS, Webpack | PR aberto | 22/09/2026 | [#718](https://github.com/brmodeloweb/brmodelo-app/pull/718) |
| BRMW | React 19, TypeScript, JointJS, Webpack | PR fechado | 22/09/2026 | [#716](https://github.com/brmodeloweb/brmodelo-app/pull/716) |

## Cases

### BRMW

![Preview BRMW](docs/previews/brmw.png)

Contribuições ao [brmodelo-app](https://github.com/brmodeloweb/brmodelo-app) (ferramenta livre de modelagem ER usada em cursos de banco de dados).

#### Tipos de dados parametrizados (#712)

Adiciona tamanho/precisão a tipos variáveis (`VARCHAR(255)`, `DECIMAL(10,2)`), amplia o catálogo de tipos e preserva esses metadados na conversão conceitual → lógico / NoSQL e na geração SQL.

- **Stack:** React 19, TypeScript, JointJS (`@joint/core`), Webpack 5, pnpm
- **Entrega:** Campos estruturados `length` / `precision` / `scale` nos editores lógico, conceitual e NoSQL; formatador compartilhado no DDL e no diagrama; catálogo ampliado (`DECIMAL`, `TEXT`, `BIGINT`, `UUID`, …)
- **Destaques técnicos:** `dataTypes.ts` + `TypeParamsFields`; params em `Column` / `erd.Attribute` / rows NoSQL; `formatColumnType` no `sqlGenerator`
- **Upstream:** [`brmodeloweb/brmodelo-app`](https://github.com/brmodeloweb/brmodelo-app)
- **PR:** [#718](https://github.com/brmodeloweb/brmodelo-app/pull/718) *(aberto)*
- **Issues:** [#712](https://github.com/brmodeloweb/brmodelo-app/issues/712)

#### Cardinalidade, sync de FK e export (#706 / #386)

Restauração da edição de cardinalidade nos editores conceitual e lógico, sincronização de FK ao mudar 1:1/1:N, export/import JSON do modelo e geração SQL mais confiável.

- **Stack:** React 19, TypeScript, JointJS (`@joint/core`), Webpack 5, pnpm
- **Entrega:** Seleção de links pelo clique, edição de cardinalidade com sync de FK, import/export `.brmw.json`, SQL com `REFERENCES` pela PK, copiar/baixar e validação; dirty/`cross-env` no Windows
- **Destaques técnicos:** `link:pointerclick` + tools persistentes; `logicalCardinality` + `syncForeignKeyForLink`; `modelFileIO` e validação SQL
- **Upstream:** [`brmodeloweb/brmodelo-app`](https://github.com/brmodeloweb/brmodelo-app)
- **PR:** [#716](https://github.com/brmodeloweb/brmodelo-app/pull/716) *(fechado)*
- **Issues:** [#706](https://github.com/brmodeloweb/brmodelo-app/issues/706), [#714](https://github.com/brmodeloweb/brmodelo-app/issues/714), [#713](https://github.com/brmodeloweb/brmodelo-app/issues/713), [#386](https://github.com/brmodeloweb/brmodelo-app/issues/386), [#693](https://github.com/brmodeloweb/brmodelo-app/issues/693), [#626](https://github.com/brmodeloweb/brmodelo-app/issues/626), [#715](https://github.com/brmodeloweb/brmodelo-app/issues/715)

## Padrões que sigo

- Respeitar Code of Conduct e convenções do projeto upstream
- Preferir issues claras e reproduzíveis antes de abrir PR
- Branches `fix/`, `feature/` ou `enhancement/` a partir de `main`
- Commits com prefixo (`Fix:`, `Feat:`, `Docs:`, …) quando o projeto pedir
- Documentar na capa o link do PR e o status (aberto / mergeado)

## Como adicionar uma nova contribuição

Siga o template em [docs/ADDING_A_PROJECT.md](docs/ADDING_A_PROJECT.md).
