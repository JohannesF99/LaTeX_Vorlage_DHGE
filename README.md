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

=> alle Formeln sind zentral zum Gleichheitszeichen
