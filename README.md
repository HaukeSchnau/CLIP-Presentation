# Hamburg Neue
Eine einfache Beamer Vorlage, entstanden aus dem desinteresse der Nutzung einer Vorlage der Uni Hamburg.

## Anwendungsanleitung
Der [Beameruserguide](http://tug.ctan.org/macros/latex/contrib/beamer/doc/beameruserguide.pdf) erklärt ganz gut, wie man Beamer benutzen kann. Wenn das nicht reich, kann man einfach im Internet nach Hilfe suchen.

Zum Repository selbst: einfach **template** Ordner Kopieren und in die `main.tex` die Präsentation schreiben. Es empfehlt sich den neuen Ordner mit `git` zu tracken.

### Kompilierung
Das Dokument sollte viermal kompiliert werden.

1. `pdflatex main.tex`
2. `bibtex main`
3. `pdflatex main.tex`
4. `pdflatex main.tex`

Danach sollte ein nutzbares PDF entstanden sein.

### Hinweis zum Literaturverzeichnis
Es ist mit LaTeX möglich eine `.bib`-Datei für mehrere Projekte zu nutzen.
Hierfür ist die `.bib`-Datei an einen Ort der eigenen Wahl abzulegen und der Dateipfad in der `main.tex` Datei anzugeben.

## Design

### Designelemente
- innertheme **circles**
- outhertheme **miniframes**
- Farben selbst entwickelt.

### Customizing
In der `main.tex` Datei kann man zu Beginn den optionalen Parameter `color` benutzen um eine von acht Farben als Akzentfarbe, des **Crayfish** colorthemes zu wählen (die Standardfarbe ist `red`, sonst gibt es noch `orange`, `yellow`, `green`, `cyan`, `blue`, `violet` und `magenta`).

Im gleichen Bereich lässt sich mit der optionalen Parameter `high-contrast` ein höhere Kontrast zwischen schrift und hintergrund aktivieren, für den Fall das es zu hell im Vortragsraum ist.

Ein weiterer optionalen Parameter ist `dark-mode`, damit werden die Folien mit heller Schrift auf dunklen Hintergrund dargestellt. **Wichtig: Diese Funktion ist noch ganz ausgereift es kann also teilweise nicht ganz klappen**

btw. das Colortheme lässt sich auch separat, ohne die **HamburgNeue** Vorlage verwenden.

### Fonts

Die Standardschrift der Folien ist **FiraSans** es lässt sich aber mit dem optionalen Parameter `font` im head package die Font anpassen.

Getestete Fonts:

- `FiraSans` - Siehe Fotos
- `inter` - Schrift, die für Monitore Optimiert ist
- `tgheros` - Schrift, die wie Helvetica aussieht

*Die angegebenen Namen sind so zu übernehmen wenn man die Font verwenden will.*

Weitere Fonts können vermutlich auch verwendet werden wenn man sie direkt per `\\usepackage{font}` laden kann, bei den drei genannten funktioniert es zumindest auf meiner Maschine.
### Demobilder

#### Normal

![pallete](img/palette.png)
![preview](img/preview.png)

#### High-Contrast

![palletehighcontrast](img/palettehighcontrast.png)
![previewhighcontrast](img/previewhighcontrast.png)
