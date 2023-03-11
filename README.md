# 📑 Author-Year Citation Style for Zotero

This citation style aims to add a missing author-year citation style to the [Zotero Style Repository](https://www.zotero.org/styles). This style is furthermore  based on guideline [<ins>Zitate und Fußnoten</ins>](https://www.gmth.de/formatierung.aspx#zf) by the [ZGMTH](https://www.gmth.de/zeitschrift.aspx).

## ⚡️ Use the style with Zotero

An overview of the different types of sources that can be referenced can be found [here](https://docs.citationstyles.org/en/stable/specification.html#appendix-iii-types).

## 🧑‍💻 Improve the style

The citation style is written in the XML-based [Citation Style Language](https://citationstyles.org/)-spec. The documentation can be found [here](https://docs.citationstyles.org/en/stable/specification.html).

It is most convenient to use the [Visual CSL Editor](https://editor.citationstyles.org/visualEditor/). To see a how a style can look use the provided [American Psychological Association 7th Edition](apa.csl) which already looks very similar to what is needed.

## ❗️ Limits

## 💎 Features

### Fußnoten

- [x] Fußnoten: 
    - Müller 2014, 325.
    - Müller 2014, 325f.
    - Müller 2014, 325–327. ← "En Dash" (`⌥ -`)
- [x] Unmittelbar folgende Verweise auf die gleiche Publikation
    - Ebd., 34.
- [ ] Zitate und Literaturnachweise in Fußnoten: 
    - »Zitat« (Müller 2014, 34).
    - Müller kommentiert: »Zitat« (2014, 34).
    - Müller (2014, 34) weist darauf hin, dass …
    - Müller 2014, 33. Weiterhin vertritt Müller die Position, die »Zitation vollständiger Sätze« sei »zumeist verzichtbar« (ebd., 34).
- [ ] Punctuation: 
    - »Hieraus folgt nun, dass es so viel Formen geben kann als Kunstwerke« (Marx 1838, 5).
    - »Der Inbegriff nun der Grundzüge, in denen eine Masse einzelner Kunstwerke übereinstimmt, heißt Kunstform.« (Marx 1838, 5) ← Zitat endet mit Punkt.

### Literaturverzeichnis

- [ ] Disambiguation mehrerer Publikationen des gleichen Autors im gleichen Jahr
    - Riemann, Hugo (1901a), »Musikalische Logik« [1872], in: ders., Präludien und Studien III, Leipzig: Breitkopf & Härtel, 1–22.
    - Riemann, Hugo (1901b), »Zur Theorie der Konsonanz und Dissonanz«, in: ders., Präludien und Studien III, Leipzig: Breitkopf & Härtel, 31–45.
- [ ] Simplifikation des Erscheinungsortes (nur der erste wird aufgeführt
    - Schmidt, Lothar (1990), *Organische Form in der Musik. Stationen eines Begriffs 1795–1850*, Kassel: Bärenreiter[.]
        > Fehlt hier ein Punkt auf der Website??

#### Selbstständige Publikationen

- [x] Basics
    - Jost, Christa (1988), *Mendelssohns Lieder ohne Worte*, Tutzing: Schneider. → **book**
    - Autor, Anton (Hg.) (2008), […]
- [ ] Mehrere AutorInnen/HerausgeberInnen
    - Müller, Peter / Friedrich Huber / Petra Meier (1999), […]
    - Müller, Peter / Friedrich Huber / Petra Meier (Hg.) (1999), […]

#### Unselbstständige Publikationen

- [ ] Basics
    - Bernstein, David W. (2002), »Nineteenth-Century Harmonic Theory: The Austro-German Legacy«, in: *The Cambridge History of Western Music Theory*, hg. von Thomas Christensen, Cambridge: Cambridge University Press, 788–794.
    - Riemann, Hugo (1901), »Zur Theorie der Konsonanz und Dissonanz«, in: ders., *Präludien und Studien III*, Leipzig: Breitkopf & Härtel, 31–45.
    - Aerts, Hans (2007), »›Modell‹ und ›Topos‹ in der deutschsprachigen Musiktheorie seit Riemann«, *Zeitschrift der Gesellschaft für Musiktheorie* 4/1–2, 143–158.
https://doi.org/10.31751/250 (15.2.2017)
- [ ] Mehrere AutorInnen/HerausgeberInnen
    - […], hg. von Peter Müller, Sabine Meier und Sieglinde Delmenhorst, […]
- [ ] Spezifikation Band/Bände
    - Marx, Adolf Bernhard (1837), *Die Lehre von der musikalischen Komposition*, Bd. 1, Leipzig: Breitkopf & Härtel[.]
    - Schumann, Robert (1854), *Gesammelte Schriften über Musik und Musiker* (4 Bde.), Leipzig: Wiegand[.]
- [ ] Teilbände werden mit Punkt abgetrennt: Bd. 34.2.
- [ ] Betitelte Einzelbände
    - Riemann, Hugo (1903), *Der polyphone Satz* (= *Große Kompositionslehre*, Bd. 2), Berlin: Spemann[.]
- [ ] Reihentitel: Reihentitel wie »Beihefte von…«, »Schriftenreihe der …« werden nicht angegeben.
Gesamtausgaben und Gesammelte Schriften werden aber immer vollständig mit Herausgeber*innen angegeben.
    - Adorno, Theodor W. (1976), *Der getreue Korrepetitor* [1958] in: ders., *Gesammelte Schriften*, hg. von Rolf Tiedemann, Bd. 15, Frankfurt a. M.: Suhrkamp, 157–401.
    - Adorno, Theodor W. (2001a), *Zu einer Theorie der musikalischen Reproduktion. Aufzeichnungen, ein Entwurf und zwei Schemata* (= Nachgelassene Schriften Abt. I/Bd. 2), hg. von Henri Lonitz, Frankfurt a. M.: Suhrkamp.
    - Dahlhaus, Carl (2002), *Die Idee der absoluten Musik* [1978], in: ders., *19. Jahrhundert I* (= *Gesammelte Schriften in zehn Bänden*, Bd. 4), hg. von Hermann Danuser in Verbindung mit Hans-Joachim Hinrichsen und Tobias Plebuch, Laaber: Laaber, 9–126.

#### Neuauflagen, Reprints und Neueditionen

- [ ] Erscheinungsdatum der Erstausgabe in eckigen Klammern
    - Dahlhaus, Carl (2002), *Die Idee der absoluten Musik* [1978], in: ders., *19. Jahrhundert I* (= *Gesammelte Schriften in zehn Bänden*, Bd. 4), hg. von Hermann Danuser in Verbindung mit Hans-Joachim Hinrichsen und Tobias Plebuch, Laaber: Laaber, 9–126.
- [ ] Bei Reprints (Faksimiles) steht ›Reprint‹ vor dem Ort ohne Komma; die Jahreszahl in Klammern gibt das Erscheinungsjahr des Originals wieder
    - Riemann, Hugo (1901), *Präludien und Studien III*, Leipzig: Breitkopf & Härtel, Reprint Hildesheim: Olms 1967.
    - Fenaroli, Fedele (1775), *Regole musicali di cembalo*, Neapel, Reprint Bologna: Forni 1975.
        > Zusätzliches Leerzeichen vor schließendem Punkt auf der Website...
- [ ] Neueditionen:
    - Koch, Heinrich Christoph (2007), *Versuch einer Anleitung zur Composition* [1782; 1787; 1793], Neuedition, hg. von Jo Wilhelm Siebert, Hannover: Siebert.

#### Übersetzungen

- [ ] Hinweise zur Übersetzung (abgekürzt: ›übers. von‹) stehen gegebenfalls vor dem Ort mit Komma getrennt. 
    - Goodman, Nelson (1995), *Sprachen der Kunst. Entwurf einer Symboltheorie*, übers. von Bernd Philippi, Frankfurt a. M.: Suhrkamp.

#### Wissenschaftliche Abschlussarbeiten

- [ ] unveröffentlicht
    - Preuß, Volkhardt (1991), *Die Anwendung der Clausellehre des 17. Jahrhunderts im Theorieunterricht*, Diplomarbeit, Hochschule für Musik und Theater Hamburg.
- [ ] veröffentlicht
    - Müller, Peter (2008), *Der Akkord C‐Dur*, Phil. Diss., Laaber, Laaber.
- [ ] Hinweise zum Dissertationsstatus stehen vor der Institution (unveröffentl.) bzw. dem Ort (veröffentl.), durch Komma getrennt.
    - [...] Phil. Diss., Universität Bonn.
    - [...] Ph.D., University of Oregon.

#### Manuskripte und Typoskripte

Die Angabe Ms. steht nach dem Titel.

- [ ] Nicht editierte Manuskripte
    - Anonym (um 1700), *Regole del contrappunto, del sonare il basso continuo, et accompagnare la parte che canta*, Ms., I-Bc P.120 (5), fol. 32r–46v.
- [ ] Editierte Manuskripte, selbständige Publikation
    - Durante, Francesco (2003), *Bassi e Fughe* [Ms.], hg. von Giuseppe A. Pastore, Padua: Armelin Musica.
    - Muffat, Georg (1961), »Regulae concentuum partiturae« [Ms., 1699], in: *Georg Muffat. An Essay on Thoroughbass*, hg. von Hellmut Federhofer, Dallas (TX): American Institute of Musicology, 39–130.
- [ ] Editierte Manuskripte, Reprint-Ausgaben
    - [...] Reprint Badenweiler 1955 [...]

#### Internetpublikationen

- [ ] Internetlinks werden nachgestellt und enden ohne Punkt. Die Aktualität zum Zeitpunkt der Herausgabe wird von der Redaktion geprüft, das Datum des letzten Zugriffs wird bei nicht-stabilen Links in Klammern nachgestellt.
    - Reich, Kersten (2009), Beobachtung und die Unschärfen der Erkenntnis, 2., völlig überarbeitete Auflage, Köln: Luchterhand. http://www.uni-koeln.de/hf/konstrukt/reich_works/buecher/ordnung/band1.html (3.2.2016)

