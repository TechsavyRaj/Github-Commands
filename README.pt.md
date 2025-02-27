# Folha de Referência de Comandos Git

Uma lista simples de comandos úteis do Git que os desenvolvedores costumam usar:-

## Índice

- [Comandos Básicos](#comandos-básicos)
- [Trabalhando com Commits](#trabalhando-com-commits)
- [Ramificação](#ramificação)
- [Stashing](#stashing)
- [Repositórios Remotos](#repositórios-remotos)
- [Desfazendo Alterações](#desfazendo-alterações)
- [Tags](#tags)
- [Colaboração](#colaboração)
- [Comandos Avançados](#comandos-avançados)
- [Traduções do Cheatsheet](#translations)

---

## Comandos Básicos

| Comando               | Descrição                                 |
|-----------------------|-------------------------------------------|
| `git init`            | Inicializa um novo repositório Git.      |
| `git clone <url>`     | Clona um repositório existente.          |
| `git status`          | Mostra o status do diretório de trabalho.|
| `git log`             | Mostra o histórico de commits.           |
| `git show <commit>`   | Mostra detalhes de um commit específico. |

---

## Trabalhando com Commits

| Comando                       | Descrição                                  |
|-------------------------------|--------------------------------------------|
| `git add <file>`              | Adiciona um arquivo à área de stage.      |
| `git add .`                   | Adiciona todas as mudanças à área de stage.|
| `git commit -m "mensagem"`    | Comita mudanças com uma mensagem.          |
| `git commit --amend`          | Emenda o commit anterior.                  |
| `git reset <file>`            | Desfaz o stage de um arquivo.               |
| `git reset --hard <commit>`   | Reseta para um commit específico, descartando mudanças. |

---

## Ramificação

| Comando                        | Descrição                                  |
|--------------------------------|--------------------------------------------|
| `git branch`                   | Lista todas as branches.                  |
| `git branch <branch-name>`     | Cria uma nova branch.                     |
| `git branch -d <branch-name>`  | Deleta uma branch.                        |
| `git checkout <branch-name>`   | Muda para uma branch.                     |
| `git checkout -b <branch-name>`| Cria e muda para uma nova branch.         |
| `git merge <branch-name>`      | Faz merge de uma branch para a branch atual.|
| `git merge --squash <branch-name>`| Squasha múltiplos commits em um durante o merge de branch.|

---

## Stashing

| Comando                  | Descrição                                   |
|--------------------------|---------------------------------------------|
| `git stash`              | Salva mudanças não comitadas para uso futuro.|
| `git stash push -m <mensagem>`| Salva mudanças não comitadas com uma mensagem.|
| `git stash list`         | Lista todos os stashes.                    |
| `git stash apply`        | Aplica o stash mais recente.               |
| `git stash apply <stash>`| Aplica um stash específico.                |
| `git stash pop` | Aplica o stash mais recente e o remove da lista de stashes. |
| `git stash pop <stash>` | Aplica um stash específico e o remove da lista de stashes. |
| `git stash drop`         | Deleta um stash específico.                |

---

## Repositórios Remotos

| Comando                                   | Descrição                                   |
|-------------------------------------------|---------------------------------------------|
| `git remote -v`                           | Mostra repositórios remotos.               |
| `git remote add <nome> <url>`             | Adiciona um novo repositório remoto.       |
| `git fetch <remoto>`                      | Busca mudanças de um repositório remoto.   |
| `git pull <remoto> <branch>`              | Puxa mudanças de uma branch remota.        |
| `git push <remoto> <branch>`              | Envia mudanças para uma branch remota.     |
| `git push --set-upstream <remoto> <branch>` | Envia uma branch e define rastreamento upstream.|

---

## Desfazendo Alterações

| Comando                        | Descrição                                   |
|--------------------------------|---------------------------------------------|
| `git checkout -- <arquivo>`    | Descarta mudanças em um arquivo.            |
| `git revert <commit>`          | Reverte um commit específico.               |
| `git reset <commit>`           | Desfaz commits, mantendo mudanças no diretório de trabalho.|
| `git reset --hard`             | Desfaz todas as mudanças e commits permanentemente.|

---

## Tags

| Comando                    | Descrição                                   |
|----------------------------|---------------------------------------------|
| `git tag`                  | Lista todas as tags.                       |
| `git tag <nome-tag>`       | Cria uma nova tag.                         |
| `git tag -d <nome-tag>`    | Deleta uma tag.                            |
| `git push <remoto> <tag>`  | Envia uma tag para um repositório remoto.  |
| `git push --tags`          | Envia todas as tags para um repositório remoto.|

---

## Colaboração

| Comando                             | Descrição                                   |
|-------------------------------------|---------------------------------------------|
| `git pull`                          | Busca e faz merge de mudanças de uma branch remota.|
| `git fetch`                         | Busca mudanças de um repositório remoto.   |
| `git cherry-pick <commit>`          | Aplica um commit específico na branch atual.|
| `git blame <arquivo>`               | Mostra quem modificou cada linha de um arquivo.|
| `git rebase <branch>`           | Inicia um rebase no branch especificado.                |
| `git rebase --continue`         | Continua o rebase após resolver os conflitos.           |
| `git rebase --abort`            | Cancela o rebase e restaura o branch.                  |
| `git rebase -i <branch>`        | Inicia um rebase interativo.                           |
| `git push --force`              | Força o envio das alterações do rebase para o branch remoto. |

---

## Comandos Avançados

| Comando                        | Descrição                                   |
|--------------------------------|---------------------------------------------|
| `git diff`                     | Mostra mudanças entre commits, branches ou diretório de trabalho.|
| `git reflog`                   | Mostra o histórico de todas as ações (incluindo resets).|
| `git config --global <chave> <valor>` | Configura as definições do Git globalmente.|
| `git submodule add <url>`      | Adiciona um submódulo ao repositório.       |
| `git bisect`                   | Usa a busca binária para encontrar o commit que introduziu um bug.|

---

## Translations

- [English](README.md)
- [Español](README.es.md)
- [Française](README.fr.md)
- [Português](README.pt.md)
- [Deutsch](README.de.md)
- [Türkçe](README.tr.md)
- [日本語](README.jp.md)
- [हिन्दी](README.hi.md)

Criado por [TechsavyRaj](https://github.com/TechsavyRaj)
