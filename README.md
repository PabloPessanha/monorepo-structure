# Estrutura base para projetos Monorepo

Fiz este repositório com o intuito de reaproveitar uma estrutura para projetos fullstack, fazendo somente as configurações que acredito que são essenciais para todos os projetos em Typescript.

Pretendo adicionar futuramente:

- [ ] Scripts para atualização de dependencias, inicialização do projeto..;
- Automações de:
  - [ ] Estilização com husky e lint-staged;
  - [ ] Testes unitários e de integração ao pre-push com husky;
  - [ ] Automação de build com Docker e docker-compose;
- [ ] Hooks para CI/CD;
- [ ] Integração de estrutura Mobile;

## Modo de usar

A estrutura de compartilhamento de pacotes é capaz graças ao `workspaces` dentro de `package.json`, entretanto, é preciso recofigurar o nome do projeto baseado em como vai se chamar, para fazer isso é muito simples.

### Vscode

Dentro do VSCode temos a ferramenta de procura `CTRL` + `SHIFT` `F`, mas podemos acessar ela simplesmente selecionando do lado também.

Selecionado, vamos querer alterar todos os arquivos que possuem `monorepo-structure`, para isso é só digitar no primeiro input, o nome que você quer no segundo, e apertar `CTRL` + `ALT` + `ENTER`.

### Manualmente

Se quiser, também existe a possibilidade de alterar ele manualmente, sua localização está em todos os `package.json` na opção `name`.
Os arquivos que devem ser reconfigurados são:

|Diretorio                         |
|----------------------------------|
| ./package.json                   |
| ./packages/backend/package.json  |
| ./packages/frontend/package.json |
