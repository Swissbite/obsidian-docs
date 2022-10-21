---
aliases: alias, aliases
---

Manchmal kann es vorkommen, dass Sie in verschiedenen Zusammenhängen auf dieselbe Datei mit mehreren Namen verweisen möchten. Diese alternativen Namen bezeichnen wir als "Aliasnamen".

Zum Beispiel können Sie Ihren Partner mit seinem vollen Namen, seinem Vornamen oder einem Spitznamen ansprechen. Oder Sie möchten "künstliche Intelligenz" mit der Abkürzung "AI" bezeichnen. Wenn Sie mehrere Sprachen beherrschen, können Sie sich auf denselben Begriff mit dem Namen in derselben Sprache beziehen, in der der Rest der Notiz verfasst ist.

### Aliase setzen

Ab 0.9.16 können Sie die Eigenschaft "aliases" im [[YAML Front Matter]] Block einer Notiz wie folgt angeben:

``` 
--- 
aliases: [AI, Künstliche Intelligenz] 
--- 
```

Bitte beachten Sie, dass dieser Abschnitt ganz oben in einer Notiz platziert werden muss, um wirksam zu werden.

In Zukunft werden wir über benutzerfreundlichere Möglichkeiten nachdenken, um Aliase zu verwalten, als sie manuell in den Vorspann zu schreiben.

### Verlinken mit Aliasen

Sobald Sie Aliase für eine Datei gesetzt haben, können Sie `[[alias]]` schreiben, um auf die Originalseite zu verlinken. In der Autovervollständigungsliste wird dann ein Umleitungssymbol angezeigt, etwa so: 

![[Alias hinzufügen.png]]

Ein interner Link mit Anzeigetext wird wie folgt eingefügt: `[[Alias zur Notiz hinzufügen|alias]]`.

Hinweis: Der Link zum Alias wird **NICHT** als `[[alias]]` eingefügt, damit andere Software ihn auch erkennen kann.

### Unverknüpfte Erwähnungen finden

Nachdem Sie Aliasnamen für eine Notiz festgelegt haben, können Sie nicht verlinkte Erwähnungen sowohl anhand des Namens als auch der Aliasnamen finden.

Wenn Sie z. B. "AI" als Alias für "Künstliche Intelligenz" festgelegt haben, finden Sie Erwähnungen von "AI" in anderen Dateien im Abschnitt [[Rückverweise]].

Wenn Sie sich entscheiden, diese Erwähnung zu verlinken, wird ein Link mit dem Anzeigentext, der auf den Alias eingestellt ist, für Sie erstellt. Dem obigen Beispiel folgend, wird `AI` zu `[[Künstliche Intelligenz|AI]]`, sobald Sie auf die Schaltfläche "Link" klicken.