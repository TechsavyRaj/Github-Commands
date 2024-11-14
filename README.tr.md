# Git Komutları Hızlı Başvuru Kılavuzu

Geliştiricilerin sıkça kullandığı yararlı Git komutlarının basit bir listesi:-

## İçindekiler

- [Temel Komutlar](#temel-komutlar)
- [Commit'lerle Çalışma](#commitlerle-çalışma)
- [Dallanma](#dallanma)
- [Stashing](#stashing)
- [Uzak Depolar](#uzak-depolar)
- [Değişiklikleri Geri Alma](#değişiklikleri-geri-alma)
- [Etiketler](#etiketler)
- [Birlikte Çalışma](#birlikte-çalışma)
- [Gelişmiş Komutlar](#gelişmiş-komutlar)
- [Cheatsheet Çevirileri](#translations)

---

## Temel Komutlar

| Komut               | Açıklama                                  |
|---------------------|-------------------------------------------|
| `git init`          | Yeni bir Git deposu başlatır.             |
| `git clone <url>`   | Mevcut bir depoyu klonlar.                |
| `git status`        | Çalışma dizininin durumunu gösterir.      |
| `git log`           | Commit geçmişini gösterir.                |
| `git show <commit>` | Belirli bir commit'in detaylarını gösterir.|

---

## Commit'lerle Çalışma

| Komut                         | Açıklama                                   |
|-------------------------------|--------------------------------------------|
| `git add <file>`              | Bir dosyayı stage alanına ekler.           |
| `git add .`                   | Tüm değişiklikleri stage alanına ekler.    |
| `git commit -m "mesaj"`       | Bir mesaj ile değişiklikleri commit eder.  |
| `git commit --amend`          | Önceki commit'i düzeltir.                  |
| `git reset <file>`            | Bir dosyanın staging'ini geri alır.        |
| `git reset --hard <commit>`   | Değişiklikleri atarak belirli bir commit'e geri döner. |

---

## Dallanma

| Komut                          | Açıklama                                  |
|--------------------------------|-------------------------------------------|
| `git branch`                   | Tüm branch'leri listeler.                 |
| `git branch <branch-ismi>`     | Yeni bir branch oluşturur.                |
| `git branch -d <branch-ismi>`  | Bir branch'i siler.                       |
| `git checkout <branch-ismi>`   | Bir branch'e geçiş yapar.                 |
| `git checkout -b <branch-ismi>`| Yeni bir branch oluşturur ve ona geçiş yapar.|
| `git merge <branch-ismi>`      | Bir branch'i mevcut branch ile birleştirir.|
| `git merge --squash <branch-ismi>`| Birleştirirken birden fazla commit'i tek commit olarak birleştirir.|

---

## Stashing

| Komut                    | Açıklama                                  |
|--------------------------|-------------------------------------------|
| `git stash`              | Commit edilmemiş değişiklikleri daha sonra kullanmak üzere saklar.|
| `git stash push -m <mesaj>`| Commit edilmemiş değişiklikleri bir mesajla saklar.|
| `git stash list`         | Tüm stash'leri listeler.                   |
| `git stash apply`        | En son saklanan stash'i uygular.           |
| `git stash apply <stash>`| Belirli bir stash'i uygular.               |
| `git stash pop`          | En son stashi uygular ve stash listesinden kaldırır. |
| `git stash pop <stash>`  | Belirli bir stashi uygular ve stash listesinden kaldırır. |
| `git stash drop`         | Belirli bir stash'i siler.                 |

---

## Uzak Depolar

| Komut                                 | Açıklama                                  |
|---------------------------------------|-------------------------------------------|
| `git remote -v`                       | Uzak depoları gösterir.                   |
| `git remote add <isim> <url>`         | Yeni bir uzak depo ekler.                 |
| `git fetch <uzak>`                    | Bir uzak depodan değişiklikleri alır.     |
| `git pull <uzak> <branch>`            | Bir uzak branch'ten değişiklikleri çeker. |
| `git push <uzak> <branch>`            | Bir uzak branch'e değişiklikleri gönderir.|
| `git push --set-upstream <uzak> <branch>` | Bir branch'i gönderir ve upstream takibini ayarlar.|

---

## Değişiklikleri Geri Alma

| Komut                          | Açıklama                                  |
|--------------------------------|-------------------------------------------|
| `git checkout -- <dosya>`      | Bir dosyada yapılan değişiklikleri iptal eder.|
| `git revert <commit>`          | Belirli bir commit'i geri alır.            |
| `git reset <commit>`           | Commit'leri geri alır ve değişiklikleri çalışma dizininde tutar.|
| `git reset --hard`             | Tüm değişiklikleri ve commit'leri kalıcı olarak geri alır.|

---

## Etiketler

| Komut                      | Açıklama                                  |
|----------------------------|-------------------------------------------|
| `git tag`                  | Tüm etiketleri listeler.                  |
| `git tag <etiket-ismi>`    | Yeni bir etiket oluşturur.                |
| `git tag -d <etiket-ismi>` | Bir etiketi siler.                        |
| `git push <uzak> <etiket>` | Bir etiketi uzak depoya gönderir.         |
| `git push --tags`          | Tüm etiketleri uzak depoya gönderir.      |

---

## Birlikte Çalışma

| Komut                             | Açıklama                                  |
|-----------------------------------|-------------------------------------------|
| `git pull`                        | Bir uzak branch'ten değişiklikleri alır ve birleştirir.|
| `git fetch`                       | Bir uzak depodan değişiklikleri alır.     |
| `git rebase <branch>`             | Commit'leri başka bir branch'in üzerine yeniden uygular.|
| `git cherry-pick <commit>`        | Belirli bir commit'i mevcut branch'e uygular.|
| `git blame <dosya>`               | Bir dosyanın her bir satırını kimin değiştirdiğini gösterir.|

---

## Gelişmiş Komutlar

| Komut                          | Açıklama                                  |
|--------------------------------|-------------------------------------------|
| `git diff`                     | Commit'ler, branch'ler veya çalışma dizini arasındaki değişiklikleri gösterir.|
| `git reflog`                   | Tüm eylemlerin geçmişini (reset'ler dahil) gösterir.|
| `git config --global <anahtar> <değer>` | Git ayarlarını küresel olarak yapılandırır.|
| `git submodule add <url>`      | Depoya bir alt modül ekler.               |
| `git bisect`                   | Bir hatayı tanıtan commit'i bulmak için ikili arama kullanır.|

---

## Translations

- [English](README.md)
- [Español](README.es.md)
- [Française](README.fr.md)
- [Português](README.pt.md)
- [Türkçe](README.tr.md)
- [日本語](README.jp.md)
- [हिन्दी](README.hi.md)
