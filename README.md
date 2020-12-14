# Anleitung

- Um die Vorlage zu benutzen, wird ein TeX-Interpreter benötigt, zum Beispiel:
  - für Windows:  http://mirror.ctan.org/systems/texlive/tlnet/install-tl-windows.exe
  - für Mac:      http://mirror.ctan.org/systems/mac/mactex/MacTeX.pkg
  - für Linux:    http://mirror.ctan.org/systems/texlive/tlnet/install-tl-unx.tar.gz
- Optional gibt es zusätzlich noch spezielle Texteditoren, zum Beispiel:
  - TeXmaker:     https://www.xm1math.net/texmaker/
  - Kile:         https://kile.sourceforge.io/
- Anschließend kann die ".tex"-Datei geöffnet werden - Sie enthält den Code, wodurch LaTeX die pdf-Datei erstellt
- Nach jeder Änderung muss LaTeX die pdf neu generieren, im Fall von TeXmaker funktionert das mithilfe von "F1"
- Quellen werden in der Datei "quellen.bib" gespeichert und mithilfe von "F11" (in TeXmaker) bereitgestellt.
- Beschriftung des Headers in Zeile 78-79
- Die römische Nummerierung ab dem Literaturverzeichnis funktioniert nicht automatisch
- => muss manuell eingetragen werden, siehe "\setcounter{Page}{NUMMER}"

# Funktionen

## Tabelle:

- Schriftausrichtung entweder durch Links(l), Center(c) oder Rechts(r)

- Feste Spaltengröße durch z.B.: L{3cm}

- "caption": Name des Bildes (wird später im Abbildungsverzeichnis angezeigt).

- senkrechter Stricht durch "\hline"

- Abgrenzung der Spalten durch "&"

## Aufzählung:

- Zeichen in Klammern gibt Aufzählung an, z.B.: "\item[a)]"

## Formeln:

- Formel positioniert sich immer zentral zum "&", z.B.: F &= m * g
- => alle Formeln sind zentral zum Gleichheitszeichen

## Bilder

- Pfad zum Bild mithilfe von "\includegraphics{PFAD_ZUM_BILD}"
- Breite/Höhe kann eingestellt werden
- => siehe z.B.: eine Breite von 13cm: "\includegraphics[width=13cm]{PFAD}"
  
## Code

- Programmiersprache (language), Name (caption) und Start der Nummerierung (firstnumber) kann eingestellt werden
- => siehe z.B.: "\begin{lstlisting}[language=Java, caption=Codeblock 1, style=mystyle, firstnumber=1]"

## Abkürzungen

- wird im Abkürzungsverzeichnis (in Vorlage ab Zeile 111) hinzugefügt 
- Muster: "\acro{ABKÜRZUNG}{AUSGESCHRIEBEN}"
- im Dokument durch "\ac{ABKÜRZUNG}" aufgerufen

## Literatur und Zitate

- verschiedene Arten von Quellen benötigen verschieden Informationen
- für Websites: misc
- Quellen benötigen Zugriffsnamen für LaTeX, so z.B.: @misc{ZUGRIFFSNAME, ...}
- nachdem Quelle hinzugefügt wurde: BibTeX mehrfach aktualisieren ("F11" in TeXmaker)
- Verweis auf Quelle in ".tex"-Datei mithilfe von "\cite{ZUGRIFFSNAME}"

## Fußnoten

- mithilfe von "\footnote{TEXT}"
