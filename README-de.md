**[English translation](./README.md)**

# ifg-letter-appeal

Eine [LaTeX](https://www.latex-project.org/)-Vorlage für Einsprüche gegen ablehnende Bescheide von Behörden auf IFG-Anfragen (siehe [Informationsfreiheitsgesetz](https://de.wikipedia.org/wiki/Informationsfreiheitsgesetz)).
Erstellt für und vorgeschlagen zur Verwendung mit [FragDenStaat](https://fragdenstaat.de/).

Derzeit nur in deutsch verfügbar.

## Beispiel

Der enthaltene Text ist hauptsächlich als Beispiel gedacht. Außerdem enthält er einige allgemeine Argumente/Boilerplate-Text, der wiederverwendet werden kann.

![Vorschaubild der ersten Seite](./screenshots/template-page1.png)
![Vorschaubild der zweiten Seite](./screenshots/template-page2.png)

Die [PDF dieser zusammengestellten Vorlage kann auch heruntergeladen werden](https://github.com/rugk/ifg-letter-appeal/releases/latest).

## Erstellen

Wir empfehlen eine aktuelle Tex-Distribution, z. B. TexLive 2020. Die verwendete [Schriftart hat in älteren Versionen einen Anzeige-Bug](https://tex.stackexchange.com/q/578223/98645).
Außerdem wird LuaLaTeX empfohlen (es sollten aber auch andere LaTeX-Compiler funktionieren)

Die Datei `me-agency.lco.example` im Ordner `sender` muss zu zu `me-agency.lco` umbenannt werden, damit der Buildvorgang funktioniert.

## Struktur

* [`sender/`](sender/) enthält die Daten des Absenders (d. h. deine Daten), die du einbinden möchtest.
* [`receiver/`](receiver/) enthält die Kontaktdaten des Empfängers (d. h. der Behörde).
* [`sender.lco`](sender.lco) enthält allgemeine Einstellungen, die entscheiden wie der Absender dargestellt wird.
* [`ifg-letter-appeal.tex`](ifg-letter-appeal.tex) ist der Haupteinstiegspunkt. Verwende ihn, um den Brief zu erzeugen.

## Credits

Der Briefstil ist größtenteils dank [`scrletter`](https://www.ctan.org/pkg/scrletter)/[`scrlttr2`](https://www.ctan.org/pkg/scrlttr2), d.h. den LaTeX [KOMA-Script](https://komascript.de/)-Klassen möglich.

Danke auch an die großartige [Stackexchange Tex](https://tex.stackexchange.com/)-Gemeinschaft. (Verwendete Fragen/Antworten sind meist als Kommentare verlinkt).

## Weitere hilfreiche Links

* [Wie ist die Frist bei Widersprüchen zu berechnen?](https://forum.okfn.de/t/berechnung-interpretation-der-monatsfrist-fuer-einen-widerspruch/943?u=rugk) Erklärt auch die Formerfordernisse.  
* [CTAN-Seite für `scrletter`] (https://www.ctan.org/pkg/scrletter) mit Links zur Dokumentation von KOMA-Script (`scrguide.pdf`) in Deutsch und Englisch.
