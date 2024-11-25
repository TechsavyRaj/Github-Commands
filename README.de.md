# Git-Befehle Spickzettel

Eine einfache Liste nützlicher Git-Befehle, die Entwickler häufig verwenden :-

## Inhaltsverzeichnis

- [Grundlegende Befehle](#grundlegende-befehle)
- [Arbeiten mit Commits](#arbeiten-mit-commits)
- [Branching](#branching)
- [Stashing](#stashing)
- [Remote-Repositories](#remote-repositories)
- [Änderungen rückgängig machen](#änderungen-rückgängig-machen)
- [Tags](#tags)
- [Zusammenarbeit](#zusammenarbeit)
- [Erweiterte Befehle](#erweiterte-befehle)
- [Spickzettel-Übersetzungen](#translations)

---

## Grundlegende Befehle

| Befehl               | Beschreibung                              |
|----------------------|-------------------------------------------|
| `git init`           | Ein neues Git-Repository initialisieren.  |
| `git clone <url>`    | Ein bestehendes Repository klonen.        |
| `git status`         | Den Status des Arbeitsverzeichnisses anzeigen. |
| `git log`            | Den Commit-Verlauf anzeigen.              |
| `git show <commit>`  | Details eines bestimmten Commits anzeigen.|

---

## Arbeiten mit Commits

| Befehl                       | Beschreibung                                   |
|------------------------------|-----------------------------------------------|
| `git add <file>`             | Eine Datei zum Staging-Bereich hinzufügen.    |
| `git add .`                  | Alle Änderungen zum Staging-Bereich hinzufügen.|
| `git commit -m "message"`    | Änderungen mit einer Nachricht committen.     |
| `git commit --amend`         | Den vorherigen Commit ändern.                 |
| `git reset <file>`           | Eine Datei aus dem Staging-Bereich entfernen. |
| `git reset --hard <commit>`  | Auf einen bestimmten Commit zurücksetzen und Änderungen verwerfen. |

---

## Branching

| Befehl                        | Beschreibung                                  |
|-------------------------------|----------------------------------------------|
| `git branch`                  | Alle Branches auflisten.                     |
| `git branch <branch-name>`    | Einen neuen Branch erstellen.                |
| `git branch -d <branch-name>` | Einen Branch löschen.                        |
| `git checkout <branch-name>`  | Zu einem Branch wechseln.                    |
| `git checkout -b <branch-name>`| Einen neuen Branch erstellen und wechseln.  |
| `git merge <branch-name>`     | Einen Branch in den aktuellen Branch mergen. |
| `git merge --squash <branch-name>`| Mehrere Commits während des Branch-Merges zu einem zusammenfassen. |

---

## Stashing

| Befehl                  | Beschreibung                                   |
|-------------------------|-----------------------------------------------|
| `git stash`             | Nicht commitete Änderungen für später speichern. |
| `git stash push -m <message>`| Nicht commitete Änderungen mit Nachricht speichern. |
| `git stash list`        | Alle Stashes auflisten.                       |
| `git stash apply`       | Den neuesten Stash anwenden.                  |
| `git stash apply <stash>`| Einen bestimmten Stash anwenden.             |
| `git stash pop`         | Den neuesten Stash anwenden und aus der Stash-Liste entfernen. |
| `git stash pop <stash>` | Einen bestimmten Stash anwenden und aus der Stash-Liste entfernen. |
| `git stash drop`        | Einen bestimmten Stash löschen.               |

---

## Remote-Repositories

| Befehl                                   | Beschreibung                                   |
|------------------------------------------|-----------------------------------------------|
| `git remote -v`                          | Remote-Repositories anzeigen.                 |
| `git remote add <name> <url>`            | Ein neues Remote-Repository hinzufügen.       |
| `git fetch <remote>`                     | Änderungen von einem Remote-Repository holen. |
| `git pull <remote> <branch>`             | Änderungen von einem Remote-Branch holen.     |
| `git push <remote> <branch>`             | Änderungen zu einem Remote-Branch pushen.     |
| `git push --set-upstream <remote> <branch>` | Einen Branch pushen und Upstream-Tracking setzen. |

---

## Änderungen rückgängig machen

| Befehl                        | Beschreibung                                   |
|-------------------------------|-----------------------------------------------|
| `git checkout -- <file>`      | Änderungen an einer Datei verwerfen.          |
| `git revert <commit>`         | Einen bestimmten Commit rückgängig machen.    |
| `git reset <commit>`          | Commits rückgängig machen und Änderungen im Arbeitsverzeichnis behalten. |
| `git reset --hard`            | Alle Änderungen und Commits dauerhaft rückgängig machen. |

---

## Tags

| Befehl                    | Beschreibung                                   |
|---------------------------|-----------------------------------------------|
| `git tag`                 | Alle Tags auflisten.                          |
| `git tag <tag-name>`      | Einen neuen Tag erstellen.                    |
| `git tag -d <tag-name>`   | Einen Tag löschen.                            |
| `git push <remote> <tag>` | Einen Tag zu einem Remote-Repository pushen.  |
| `git push --tags`         | Alle Tags zu einem Remote-Repository pushen.  |

---

## Zusammenarbeit

| Befehl                             | Beschreibung                                   |
|------------------------------------|-----------------------------------------------|
| `git pull`                         | Änderungen von einem Remote-Branch holen und mergen. |
| `git fetch`                        | Änderungen von einem Remote-Repository holen. |
| `git rebase <branch>`              | Commits auf einen anderen Branch erneut anwenden. |
| `git cherry-pick <commit>`         | Einen bestimmten Commit auf den aktuellen Branch anwenden. |
| `git blame <file>`                 | Anzeigen, wer jede Zeile einer Datei geändert hat. |

---

## Erweiterte Befehle

| Befehl                        | Beschreibung                                   |
|-------------------------------|-----------------------------------------------|
| `git diff`                    | Änderungen zwischen Commits, Branches oder Arbeitsverzeichnis anzeigen. |
| `git reflog`                  | Die Historie aller Aktionen anzeigen (einschließlich Resets). |
| `git config --global <key> <value>` | Git-Einstellungen global konfigurieren.     |
| `git submodule add <url>`     | Ein Submodul zum Repository hinzufügen.       |
| `git bisect`                  | Binäre Suche verwenden, um den Commit zu finden, der einen Fehler eingeführt hat. |

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
