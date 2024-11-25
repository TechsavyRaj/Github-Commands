# Git Commands Cheat Sheet

Una lista simple de comandos útiles de Git que los desarrolladores utilizan comúnmente:

## Tabla de Contenidos

- [Comandos Básicos](#comandos-básicos)
- [Trabajar con Commits](#trabajar-con-commits)
- [Branching](#branching)
- [Stashing](#stashing)
- [Repositorios Remotos](#repositorios-remotos)
- [Deshacer Cambios](#deshacer-cambios)
- [Etiquetas](#etiquetas)
- [Colaboración](#colaboración)
- [Comandos Avanzados](#comandos-avanzados)
- [Traducciones de hojas de referencia](#translations)

---

## Comandos Básicos

| Comando                   | Descripción                                   |
|---------------------------|-----------------------------------------------|
| `git init`                | Inicializar un nuevo repositorio Git.         |
| `git clone <url>`         | Clonar un repositorio existente.              |
| `git status`              | Mostrar el estado del directorio de trabajo.  |
| `git log`                 | Mostrar el historial de commits.              |
| `git show <commit>`       | Mostrar detalles de un commit específico.     |

---

## Trabajar con Commits

| Comando                             | Descripción                                   |
|-------------------------------------|-----------------------------------------------|
| `git add <file>`                    | Agregar un archivo al área de preparación.    |
| `git add .`                         | Agregar todos los cambios al área de preparación. |
| `git commit -m "mensaje"`           | Confirmar cambios con un mensaje.             |
| `git commit --amend`                | Modificar el commit anterior.                 |
| `git reset <file>`                  | Quitar un archivo del área de preparación.    |
| `git reset --hard <commit>`         | Restablecer a un commit específico, descartando cambios. |

---

## Branching

| Comando                             | Descripción                                    |
|-------------------------------------|------------------------------------------------|
| `git branch`                        | Listar todas las ramas.                        |
| `git branch <branch-name>`          | Crear una nueva rama.                          |
| `git branch -d <branch-name>`       | Eliminar una rama.                             |
| `git checkout <branch-name>`        | Cambiar a una rama.                            |
| `git checkout -b <branch-name>`     | Crear y cambiar a una nueva rama.              |
| `git merge <branch-name>`           | Fusionar una rama con la rama actual.          |
| `git merge --squash <branch-name>`  | Aplastar múltiples commits en uno durante la fusión de ramas. |

---

## Stashing

| Comando                             | Descripción                                   |
|-------------------------------------|-----------------------------------------------|
| `git stash`                         | Guardar cambios no confirmados para uso posterior. |
| `git stash push -m <mensaje>`       | Guardar cambios no confirmados con un mensaje. |
| `git stash list`                    | Listar todos los stashes.                     |
| `git stash apply`                   | Aplicar el stash más reciente.                |
| `git stash apply <stash>`           | Aplicar un stash específico.                  |
| `git stash pop`          | Aplica el stash más reciente y lo elimina de la lista de stashes. |
| `git stash pop <stash>`  | Aplica un stash específico y lo elimina de la lista de stashes. |
| `git stash drop`                    | Eliminar un stash específico.                 |

---

## Repositorios Remotos

| Comando                             | Descripción                                   |
|-------------------------------------|-----------------------------------------------|
| `git remote -v`                     | Mostrar los repositorios remotos.             |
| `git remote add <name> <url>`       | Agregar un nuevo repositorio remoto.          |
| `git fetch <remote>`                | Obtener cambios de un repositorio remoto.     |
| `git pull <remote> <branch>`        | Obtener y fusionar cambios de una rama remota.|
| `git push <remote> <branch>`        | Enviar cambios a una rama remota.             |
| `git push --set-upstream <remote> <branch>` | Enviar una rama y establecer seguimiento ascendente. |

---

## Deshacer Cambios

| Comando                             | Descripción                                   |
|-------------------------------------|-----------------------------------------------|
| `git checkout -- <file>`            | Descartar cambios en un archivo.              |
| `git revert <commit>`               | Revertir un commit específico.                |
| `git reset <commit>`                | Deshacer commits, manteniendo los cambios en el directorio de trabajo. |
| `git reset --hard`                  | Deshacer todos los cambios y commits permanentemente. |

---

## Etiquetas

| Comando                             | Descripción                                   |
|-------------------------------------|-----------------------------------------------|
| `git tag`                           | Listar todas las etiquetas.                   |
| `git tag <tag-name>`                | Crear una nueva etiqueta.                     |
| `git tag -d <tag-name>`             | Eliminar una etiqueta.                        |
| `git push <remote> <tag>`           | Enviar una etiqueta a un repositorio remoto.  |
| `git push --tags`                   | Enviar todas las etiquetas a un repositorio remoto. |

---

## Colaboración

| Comando                             | Descripción                                   |
|-------------------------------------|-----------------------------------------------|
| `git pull`                          | Obtener y fusionar cambios de una rama remota.|
| `git fetch`                         | Obtener cambios de un repositorio remoto.     |
| `git rebase <branch>`               | Reaplicar commits en otra rama.               |
| `git cherry-pick <commit>`          | Aplicar un commit específico a la rama actual.|
| `git blame <file>`                  | Mostrar quién modificó cada línea de un archivo.|

---

## Comandos Avanzados

| Comando                             | Descripción                                   |
|-------------------------------------|-----------------------------------------------|
| `git diff`                          | Mostrar cambios entre commits, ramas o el directorio de trabajo. |
| `git reflog`                        | Mostrar el historial de todas las acciones (incluyendo resets). |
| `git config --global <key> <value>` | Configurar ajustes de Git globalmente.        |
| `git submodule add <url>`           | Agregar un submódulo al repositorio.          |
| `git bisect`                        | Usar búsqueda binaria para encontrar el commit que introdujo un error. |

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

Created by TechsavyRaj - [[GitHub Profile Link]](https://github.com/TechsavyRaj)
