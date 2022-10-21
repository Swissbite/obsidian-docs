---
aliases: front matter, front matter de
---

YAML, auch Front Matter genannt, ist als Metadaten auf Dateiebene konzipiert, die von Menschen *und* Obsidian lesbar sind.

Frontmatter ist ein Abschnitt mit Klartextattributen, der in der ersten Zeile der Datei beginnt. Es ist eine der populärsten Methoden, um Metadaten in eine Markdown-Datei einzufügen, und wurde von statischen Generatoren wie Jekyll, Hugo und Gatsby populär gemacht.

Ein YAML-Block benötigt **dreifache Bindestriche** am Anfang und Ende, um von Obsidian (und anderen Anwendungen) gelesen werden zu können. ==Er muss außerdem zuoberst in der Datei stehen.==

Als Beispiel:

```
---
key: value
key2: value2
key3: [one, two, three]
key4:
- four
- five
- six
---
```

Seit Version 0.12.12 werden folgende vier Schlüsselwörter standardmässig unterstützt:
- `tags` ([[Mit Tags arbeiten|mehr Information]])
- `aliases` ([[Aliasse zu einer Notitz hinzufügen|mehr Information]])
- `cssclass`
- `publish` ([[Notizen veröffentlichen und wieder zurücknehmen#Automatische Auswahl von Notizen zur Veröffentlichung]] and [[Notizen veröffentlichen und wieder zurücknehmen#Notitzen ignorieren]])

Mit der weiteren Entwicklung von Obsidian werden wir es schrittweise für Plugin-Entwickler zugänglicher und benutzerfreundlicher machen.
