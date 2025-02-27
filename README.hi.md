# गिट कमांड्स चीट शीट

डेवलपर्स द्वारा अक्सर उपयोग किए जाने वाले उपयोगी गिट कमांड्स की एक सरल सूची:-

## सामग्री सूची

- [मूलभूत कमांड्स](#मूलभूत-कमांड्स)
- [कमिट्स के साथ काम करना](#कमिट्स-के-साथ-काम-करना)
- [ब्रांचिंग](#ब्रांचिंग)
- [स्टैशिंग](#स्टैशिंग)
- [रिमोट रिपॉजिटरीज़](#रिमोट-रिपॉजिटरीज़)
- [परिवर्तनों को वापस लेना](#परिवर्तनों-को-वापस-लेना)
- [टैग्स](#टैग्स)
- [सहयोग करना](#सहयोग-करना)
- [उन्नत कमांड्स](#उन्नत-कमांड्स)
- [चीटशीट अनुवाद](#translations)

---

## मूलभूत कमांड्स

| कमांड               | विवरण                                   |
|---------------------|-----------------------------------------|
| `git init`          | एक नया गिट रिपॉजिटरी प्रारंभ करें।      |
| `git clone <url>`   | एक मौजूदा रिपॉजिटरी को क्लोन करें।     |
| `git status`        | कार्यशील निर्देशिका की स्थिति दिखाएं।  |
| `git log`           | कमिट इतिहास दिखाएं।                    |
| `git show <commit>` | किसी विशेष कमिट का विवरण दिखाएं।       |

---

## कमिट्स के साथ काम करना

| कमांड                        | विवरण                                   |
|------------------------------|-----------------------------------------|
| `git add <file>`             | एक फाइल को स्टेजिंग एरिया में जोड़ें।  |
| `git add .`                  | सभी परिवर्तनों को स्टेजिंग एरिया में जोड़ें।|
| `git commit -m "message"`    | एक संदेश के साथ परिवर्तनों को कमिट करें।|
| `git commit --amend`         | पिछले कमिट को संशोधित करें।            |
| `git reset <file>`           | एक फाइल को अनस्टेज करें।               |
| `git reset --hard <commit>`  | परिवर्तनों को त्याग कर एक विशिष्ट कमिट पर रीसेट करें।|

---

## ब्रांचिंग

| कमांड                         | विवरण                                 |
|-------------------------------|---------------------------------------|
| `git branch`                  | सभी ब्रांचेस की सूची दिखाएं।           |
| `git branch <branch-name>`    | एक नई ब्रांच बनाएं।                   |
| `git branch -d <branch-name>` | एक ब्रांच को हटाएं।                   |
| `git checkout <branch-name>`  | एक ब्रांच पर स्विच करें।              |
| `git checkout -b <branch-name>`| एक नई ब्रांच बनाएं और उस पर स्विच करें।|
| `git merge <branch-name>`     | एक ब्रांच को मौजूदा ब्रांच के साथ मर्ज करें।|
| `git merge --squash <branch-name>`| ब्रांच मर्ज के दौरान कई कमिट्स को एक में स्क्वैश करें।|

---

## स्टैशिंग

| कमांड                     | विवरण                                    |
|---------------------------|------------------------------------------|
| `git stash`               | असंशोधित परिवर्तनों को बाद में उपयोग के लिए सहेजें।|
| `git stash push -m <message>`| एक संदेश के साथ असंशोधित परिवर्तनों को सहेजें।|
| `git stash list`          | सभी स्टैशेस की सूची दिखाएं।              |
| `git stash apply`         | सबसे हाल का स्टैश लागू करें।            |
| `git stash apply <stash>` | किसी विशेष स्टैश को लागू करें।          |
| `git stash pop`          | सबसे हाल का स्टैश लागू करें और इसे स्टैश सूची से हटा दें। |
| `git stash pop <stash>`  | एक विशिष्ट स्टैश लागू करें और इसे स्टैश सूची से हटा दें। |
| `git stash drop`          | एक विशेष स्टैश को हटाएं।                |

---

## रिमोट रिपॉजिटरीज़

| कमांड                                    | विवरण                                    |
|------------------------------------------|------------------------------------------|
| `git remote -v`                          | रिमोट रिपॉजिटरीज़ दिखाएं।               |
| `git remote add <name> <url>`            | एक नया रिमोट रिपॉजिटरी जोड़ें।         |
| `git fetch <remote>`                     | एक रिमोट रिपॉजिटरी से परिवर्तनों को प्राप्त करें।|
| `git pull <remote> <branch>`             | एक रिमोट ब्रांच से परिवर्तनों को प्राप्त करें।|
| `git push <remote> <branch>`             | एक रिमोट ब्रांच पर परिवर्तनों को पुश करें।|
| `git push --set-upstream <remote> <branch>`| एक ब्रांच को पुश करें और अपस्ट्रीम ट्रैकिंग सेट करें।|

---

## परिवर्तनों को वापस लेना

| कमांड                        | विवरण                                    |
|------------------------------|------------------------------------------|
| `git checkout -- <file>`     | एक फाइल में परिवर्तनों को त्यागें।       |
| `git revert <commit>`        | एक विशेष कमिट को पलटें।                  |
| `git reset <commit>`         | कमिट्स को पूर्ववत करें, परिवर्तनों को कार्यशील निर्देशिका में रखते हुए।|
| `git reset --hard`           | सभी परिवर्तनों और कमिट्स को स्थायी रूप से पूर्ववत करें।|

---

## टैग्स

| कमांड                      | विवरण                                   |
|----------------------------|-----------------------------------------|
| `git tag`                  | सभी टैग्स की सूची दिखाएं।               |
| `git tag <tag-name>`       | एक नया टैग बनाएं।                      |
| `git tag -d <tag-name>`    | एक टैग को हटाएं।                       |
| `git push <remote> <tag>`  | एक टैग को रिमोट रिपॉजिटरी पर पुश करें। |
| `git push --tags`          | सभी टैग्स को रिमोट रिपॉजिटरी पर पुश करें।|

---

## सहयोग करना

| कमांड                              | विवरण                                    |
|------------------------------------|------------------------------------------|
| `git pull`                         | एक रिमोट ब्रांच से परिवर्तनों को प्राप्त करें और मर्ज करें।|
| `git fetch`                        | एक रिमोट रिपॉजिटरी से परिवर्तनों को प्राप्त करें।|
| `git cherry-pick <commit>`         | एक विशेष कमिट को मौजूदा ब्रांच पर लागू करें।|
| `git blame <file>`                 | एक फाइल की प्रत्येक लाइन को किसने संशोधित किया, यह दिखाएं।|
| `git rebase <branch>`               | निर्दिष्ट शाखा पर रिबेस शुरू करें।                   |
| `git rebase --continue`             | संघर्ष सुलझाने के बाद रिबेस जारी रखें।               |
| `git rebase --abort`                | रिबेस को रद्द करें और शाखा को पुनर्स्थापित करें।       |
| `git rebase -i <branch>`            | एक इंटरएक्टिव रिबेस शुरू करें।                    |
| `git push --force`                  | रिबेस की गई परिवर्तनों को रिमोट शाखा पर धकेलें।      |

---

## उन्नत कमांड्स

| कमांड                        | विवरण                                    |
|------------------------------|------------------------------------------|
| `git diff`                   | कमिट्स, ब्रांचेस या कार्यशील निर्देशिका के बीच परिवर्तन दिखाएं।|
| `git reflog`                 | सभी क्रियाओं का इतिहास दिखाएं (रीसेट्स सहित)।|
| `git config --global <key> <value>`| गिट सेटिंग्स को वैश्विक रूप से कॉन्फ़िगर करें।|
| `git submodule add <url>`    | एक सबमॉड्यूल को रिपॉजिटरी में जोड़ें।   |
| `git bisect`                 | बग को पेश करने वाले कमिट को खोजने के लिए बाइनरी सर्च का उपयोग करें।|

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

द्वारा निर्मित [TechsavyRaj](https://github.com/TechsavyRaj)
