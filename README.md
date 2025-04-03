# Template für HSZG Arbeiten

Ein inoffizielles Template für Arbeiten an der HSZG, die man mit Latex schreiben möchte. 
Enthält einige Presets für Programmiersprachen, die in den Informatik-Kursen vorkommen sollten. 
Wird semi-aktiv weiterentwickelt, wenn sich neue Features ergeben, mir Sachen auffallen oder ich in der Mensa bequatscht werde.

## Dateien zum Konfigurieren

### Content
```/content/abstract.tex```<br>
Datei für den Abstract der Arbeit

```/content/content.tex```<br>
Datei für den Inhalt der Arbeit

### Images
```/images/```<br>
Ordner für die Bilder, die in der Arbeit vorhanden sein sollen

### Template

```/template/styles/lst_styles.tex```<br>
Enthält den lst style für alle listings

```/template/styles/programming_languages.tex```<br>
Enthält alle Definitionen für Programmiersprachen, die in Listings genutzt werden können

```/template/glossary.tex```<br>
Enthält definitionen für Glossar Eintrage. Dazu gehören auch Akronyme

Erstellung von neuen Glossareinträgen:
```latex
\newglossaryentry{<id>}{
    name=<Name des Eintrags>,
    description={<Beschreibung des Eintrags>}
}
```

Erstellung von neuen Akronymen:
```latex
\newacronym{<id>}{<Kurzform>}{<Langform>}
```

```/template/lastPages.tex```<br>
Enthält alle Elemente, die auf den abschließenden Seiten der Arbeit eingefügt werden sollen. Per default sind das:

- Glossar der Akronyme
- Glossar
- Liste aller Bilder
- Quellen der Arbeit

```/template/macros.tex```<br>
Enthält definitionen für Makros.

```/template/packages.tex```<br>
Enthält alle Packages, die für das Dokument importiert werden sollen. Dazu zählt auch die Quellendatei.

```/template/settings.tex```<br>
Enthält Einstellungen für das Dokument. Dazu gehört die Geometrie des Papiers mit den Seitenabständen und der Seitenzähler.

```/template/titlepage.tex```<br>
Enthält die Titelseite.

```/main.tex```<br>
Anfang des Dokuments. Alle Variablen, die im Template genutzt werden, werden hier festgelegt.
