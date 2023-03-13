# 📑 ZGMTH.csl

Dieser Zitierstil implementiert einen Autor-Jahr-Stil nach den [Formatierungsregeln der ZGMTH](https://www.gmth.de/formatierung.aspx#zf).

{{TOC:2}}

## Beispiele

Fließtextzitate haben immer die Form `Autor Jahr`: Adorno 2001, Choron/La Fage 1838.

### Bibliographie

Adorno, Theodor W. (2001), *Zu einer Theorie der musikalischen Reproduktion. Aufzeichnungen, ein Entwurf und zwei Schemata* (= *Nachgelassene Schriften* I/2), hg. von Henri Lonitz, Frankfurt a. M.: Suhrkamp.

Aerts, Hans (2007), „›Modell‹ und ›Topos‹ in der deutschsprachigen Musiktheorie seit Riemann“, in: *Zeitschrift der Gesellschaft für Musiktheorie* 4/1–2, 143–158. https://doi.org/10.31751/250 (15.02.2017)

Choron, Alexandre / Adrien de La Fage (1838), *Manuel complet de musique vocale et instrumentale, ou Encyclopédie musicale*, Bd. 2, Paris: Roret.

Preuß, Volkhardt (1991), *Die Anwendung der Clausellehre des 17. Jahrhunderts im Theorieunterricht*, Diplomarbeit, Hochschule für Musik und Theater Hamburg.

Riemann, Hugo (1901a), „Musikalische Logik“ [1872], in: ders. *Präludien und Studien III*, Leipzig: Breitkopf & Härtel, 1–22.

Riemann, Hugo (1901b), „Zur Theorie der Konsonanz und Dissonanz“, in: ders. *Präludien und Studien III*, Leipzig: Breitkopf & Härtel, 31–45.

Schäfke, Rudolf (1964), *Geschichte der Musikästhetik in Umrissen* [1934], 2. Auflage, Tutzing: Schneider.

## 📝 Benutzung

Der Zitierstil benutzt die Typen **Buch**, **Buchteil**, **Dissertation**, **Manuskript**, **Webseite** und **Zeitschriftenartikel**. Wird eine andere Eintragsart verwendet wird **Buch** als Standard verwendet.

> Damit sind sicher noch nicht alle Fälle abgedeckt, siehe auch [Verbesserungen](#🧑‍💻verbesserungen).

### Buch

Ein Buch hat in seiner einfachsten Form die Syntax:

```md
Autor(en) (Datum), *Titel* [type, original-date,] [Edition,] [Reihe,] [hg. von Editor(en),] Ort: Verlag. [DOI/URL (Heruntergeladen am)]
```

Ist das Buch Teil einer Reihe, ändert sich die Syntax zu:

```md
Autor(en) (Datum), *Title* (= *Reihe* Nummer der Reihe/Band [type, original-date]), [Edition,] [hg. von Editor(en),] Ort: Verlag. [DOI/URL (Heruntergeladen am)]
                                    , Abt. Nummer der Reihe
                                    , Bd.  Band
```

Ein Reprint wird markiert, indem **orginal-date**, **original-publisher** und **original-publisher-place** angegeben werden. 

```md
Autor(en) (original-date), *Titel*, original-publisher-place: original-publisher, Reprint Ort: Verlag Datum.
```

### Buchteil

Ein Buchteil unterscheidet sich von der Klasse Zeitschriftenartikel durch das Weglassen von `in:`. Dieses Verhalten kann jedoch die Angabe von **container-author** oder **original-author** überschrieben werden. Dadurch ergeben zwei Schema:

```md
Autor(en) (Datum), "Titel" [type, original-date], *Buchtitel* Band/Issue, Ort: Verlag, Seiten.
                                                            , Bd. Band
                                                            , H. Issue

Autor(en) (Datum), "Titel" [type, original-date], in: collection-author, *Buchtitel* Band/Issue, Ort: Verlag, Seiten.
                                                      original-author              , Bd. Band
                                                                                   , H. Issue
```

Ist der Autor der Reihe derselbe wie der des Auszugs daraus, kann durch die Angabe `collection-author: ders.` die gekürzte Variante erzeugt werden.

### Dissertation

Eine Dissertation hat das folgende Schema:

```md
Autor(en) (Datum), *Titel*, Art, Universität.
                                 Verlag
```

### Manuskript

Für ein Manuskript kann statt Seitenzahlen auch eine explizite Angabe wie `fol. 32r-46v` verwendet werden. Gleiches gilt für die Felder Signatur und Datum.

```md
Autor(en) (Datum), *Titel*, Art, Signatur, pages.
```

### Webseite

Eine Webseite wird wie ein Buch dargestellt.

### Zeitschriftenartikel

Ein Zeitschriftenartikel hat die Form:

```md
Autor(en) (Datum), *Titel* [type, original-date], in: *Publikation* Band/Ausgabe, [hg. von Editor(en),] Ort: Verlag. DOI (Heruntergeladen am)
                                                                  , Bd. Band                                         URL
                                                                  , H. Ausgabe
```

### Extra

Je nach Eintragsart sind die zu Verfügung stehenden Felder zum Teil sehr limitiert. Ein `Zeitschriftenartikel` hat z.B. keine Felder für Ort oder Verlag. Der Workaround ist das Feld **Extra**. Dort lassen sich als Key-Value-Pairs weitere Attribute eintragen. Im Beispiel des Zeitschriftenartikels wäre das:

```plaintext
place: Kassel
publisher: Bärenreiter
```

Es müssen die englischen Bezeichnungen der Attribute verwendet werden. Im Moment sind die folgenden für den Zitierstil relevant:

- container-author
- issue → Band
- original-author
- original-date
- original-publisher
- original-publisher-place
- pages
- place
- publisher
- type → Art

### ⚠️  Limitationen

- Es werden keine Zeilenumbrüche vor URLs oder DOIs eingefügt.
- Das Datenmodell in Zotero erlaubt keine Liste an Erscheinungsorten. Der Eintrag wird verbatim in den Quellennachweis übernommen. Eine automatische Auswahl des ersten Ortes, oder eine Auflistung mehrerer Publikationsorte ist nicht möglich.

## Installation

Der Zitierstil ist (noch) nicht im Zotero-Style-Repository vorhanden. Er kann von Hand zu Zotero hinzugefügt werden:

1. Lade `zgmth.csl` von diesem Repository herunter.
2. Unter `Zitieren` in Zoteros Einstellungen, füge den eben heruntergeladenen Stil mit einem Klick auf das `+` hinzu.

## 🧑‍💻 Verbesserungen 

Bei Wünschen oder Verbesserungsvorschlägen gerne ein Issue oder eine Pull Request öffnen.

Es ist am Einfachsten, den Stil mit dem [Visual CSL Editor](https://editor.citationstyles.org/visualEditor/) zu bearbeiten. Als Beispiel dienen die Zitate in `examples.json` (kommend von `examples.rdf`).
