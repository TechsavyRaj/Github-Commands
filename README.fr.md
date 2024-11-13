# Git Commands Cheat Sheet

Une liste simple des commandes Git utiles que les développeurs utilisent couramment :

## Table des matières
- [Commandes de base](#commandes-de-base)
- [Travailler avec des commits](#travailler-avec-des-commits)
- [Brancher](#brancher)
- [Mise en réserve](#mise-en-réserve)
- [Dépôts distants](#dépôts-distants)
- [Annuler des changements](#annuler-des-changements)
- [Tags](#tags)
- [Collaborer](#collaborer)
- [Commandes avancées](#commandes-avancées)
- [Cheatsheet Translations](#translations)

---

## Commandes de base
| Commande                 | Description                                      |
|--------------------------|--------------------------------------------------|
| `git init`               | Initialiser un nouveau dépôt Git.                |
| `git clone <url>`        | Cloner un dépôt existant.                        |
| `git status`             | Afficher l'état du répertoire de travail.        |
| `git log`                | Afficher l'historique des commits.               |
| `git show <commit>`      | Afficher les détails d'un commit spécifique.     |

---

## Travailler avec des commits
| Commande                            | Description                                    |
|-------------------------------------|------------------------------------------------|
| `git add <file>`                    | Ajouter un fichier à la zone de staging.       |
| `git add .`                         | Ajouter toutes les modifications à la zone de staging. |
| `git commit -m "message"`           | Committer les changements avec un message.     |
| `git commit --amend`                | Modifier le commit précédent.                  |
| `git reset <file>`                  | Désindexer un fichier.                         |
| `git reset --hard <commit>`         | Réinitialiser à un commit spécifique, en annulant les modifications. |

---

## Brancher
| Commande                             | Description                                     |
|--------------------------------------|-------------------------------------------------|
| `git branch`                         | Lister toutes les branches.                     |
| `git branch <branch-name>`           | Créer une nouvelle branche.                     |
| `git branch -d <branch-name>`        | Supprimer une branche.                          |
| `git checkout <branch-name>`         | Changer de branche.                             |
| `git checkout -b <branch-name>`      | Créer et changer de branche.                    |
| `git merge <branch-name>`            | Fusionner une branche dans la branche actuelle. |
| `git merge --squash <branch-name>`   | Compacter plusieurs commits en un seul pendant la fusion de branche. |

---

## Mise en réserve
| Commande                   | Description                                    |
|----------------------------|------------------------------------------------|
| `git stash`                | Sauvegarder les modifications non committées pour une utilisation ultérieure. |
| `git stash push -m <message>` | Sauvegarder les modifications non committées avec un message. |
| `git stash list`           | Lister toutes les réserves.                    |
| `git stash apply`          | Appliquer la réserve la plus récente.          |
| `git stash apply <stash>`  | Appliquer une réserve spécifique.              |
| `git stash drop`           | Supprimer une réserve spécifique.              |

---

## Dépôts distants
| Commande                                   | Description                                    |
|--------------------------------------------|------------------------------------------------|
| `git remote -v`                            | Afficher les dépôts distants.                  |
| `git remote add <name> <url>`              | Ajouter un nouveau dépôt distant.              |
| `git fetch <remote>`                       | Récupérer les modifications d'un dépôt distant. |
| `git pull <remote> <branch>`               | Tirer les modifications d'une branche distante. |
| `git push <remote> <branch>`               | Pousser les modifications vers une branche distante. |
| `git push --set-upstream <remote> <branch>` | Pousser une branche et définir le suivi en amont. |

---

## Annuler des changements
| Commande                             | Description                                   |
|--------------------------------------|-----------------------------------------------|
| `git checkout -- <file>`             | Annuler les modifications d'un fichier.       |
| `git revert <commit>`                | Revenir à un commit spécifique.               |
| `git reset <commit>`                 | Annuler les commits, en gardant les modifications dans le répertoire de travail. |
| `git reset --hard`                   | Annuler toutes les modifications et les commits de manière permanente. |

---

## Tags
| Commande                             | Description                                   |
|--------------------------------------|-----------------------------------------------|
| `git tag`                            | Lister tous les tags.                         |
| `git tag <tag-name>`                 | Créer un nouveau tag.                         |
| `git tag -d <tag-name>`              | Supprimer un tag.                             |
| `git push <remote> <tag>`            | Pousser un tag vers un dépôt distant.         |
| `git push --tags`                    | Pousser tous les tags vers un dépôt distant.  |

---

## Collaborer
| Commande                            | Description                                   |
|-------------------------------------|-----------------------------------------------|
| `git pull`                          | Récupérer et fusionner les modifications d'une branche distante. |
| `git fetch`                         | Récupérer les modifications d'un dépôt distant. |
| `git rebase <branch>`               | Réappliquer les commits sur une autre branche. |
| `git cherry-pick <commit>`          | Appliquer un commit spécifique à la branche actuelle. |
| `git blame <file>`                  | Afficher qui a modifié chaque ligne d'un fichier. |

---

## Commandes avancées
| Commande                            | Description                                   |
|-------------------------------------|-----------------------------------------------|
| `git diff`                          | Afficher les différences entre les commits, les branches ou le répertoire de travail. |
| `git reflog`                        | Afficher l'historique de toutes les actions (y compris les réinitialisations). |
| `git config --global <key> <value>` | Configurer les paramètres Git globalement.    |
| `git submodule add <url>`           | Ajouter un sous-module au dépôt.              |
| `git bisect`                        | Utiliser la recherche binaire pour trouver le commit qui a introduit un bug. |

---

## Translations
- [English](README.md)
- [Español](README.es.md)
- [Française](README.fr.md)
- [Português](README.pt.md)
- [Türkçe](README.tr.md)
- [日本語](README.jp.md)
- [العربية](READMEar.md)
- [हिन्दी](README.hi.md)
