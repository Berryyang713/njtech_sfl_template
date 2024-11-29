Template für die Fakultät der Fremdsprachen und Literatur, Nanjing Tech University <br>
=========
DE: Eine Latex und DOCX Template für die allgemeine Finalarbeit der Nanjing Tech University (Für die Sprachlernenden und die Fakultät der Fremdsprachen und Literatur verarbeitet) <br>
中文：为南京工业大学普通结课作业设计的Latex和DOCX模板（依据语言学习者及外语学院要求设计） <br>
EN: A Latex and DOCX Template for the normal course thesis of Nanjing Tech University (Designated for the students majoring in Languages and School of Foreign Languages and Literature) <br>
# DOCX-Version
## Vorstellung
Diese Template ist ein Beispiel für die Finalarbeit mit ohne zusätzlichen Aufforderungen. Wenn Sie die Template benutzen, bitte beachten Sie:
### 1. Alle Schriftarten (Fonts) heruntergeladen und installiert
Überprüfen Sie, dass Sie die Schriftarten "Times New Roman" und "Helvetica" heruntergeladen und installiert in Ihrem PC haben. Um eine Schriftart zu installieren, muss man die Schriftart herunterladen und dann verschiebt man in die folgende Ordner: `C:\Windows\Fonts`. <br>
Die Schriftarten enthalten: 
* Times New Roman (Embeddet im OS)
* Helvetica (Herunterladen: [Helvetica (Alle)](https://github.com/Berryyang713/njtech_sfl_template/tree/main/schriftarten)
### 2. Die Umgebung konfigurieren
|Umgebung|DOCX|Latex|
|:-----:|:------:|:--------:|
|Software|Microsoft Word (*Achtung:* Software-Mischung führt vielleicht zur Störung der Format.)|TexLive|
|Version|Office 2016 od. neuer|Keine Beschränkung|
|Makro|Keine|normale Makros, *ctex*|
### 3. Die Word-eigenen Tools zum Rendern der PDF-Datei verwenden
Sie müssen die Word-eigenen Tools zum Rendern der PDF-Datei verwenden. Irgendes Werkzeug wie *Adobe Acrobat PDF* konnte Fehler bei der Konvertierung haben. Um eine PDF-Datei zu konvertieren, müssen Sie: Kopie Speichern (od. F12) --> Dateityp als PDF auswählen --> Speichern
## Verbesserung
Diese Template enthält die folgenden Verbesserungen gegenüber dem Original:
### 1. Der Umschlag optimiert
* Die Gestaltung des Umschlags und die deutsch-chinesische Entsprechung einiger Begriffe werden optimiert.
* Das Layout wird optimiert.
* Bearbeitbare Felder über eine Tabelle mit horizontalen Linien werden ausgefüllt.
### 2. Die Fußzeile optimiert
* Die Seitenzahlen in den Fußzeilen wurden je nach Abschnitt optimiert, indem von fortlaufenden Seitenzahlen zu Seitenzahlen mit unterschiedlichen Bezeichnungen für verschiedene Abschnitte übergegangen wurde.

  |Typ|Seitenzahl|
  |:-----:|:------:|
  |Umschlag|Keine|
  |Inhaltsverzeichnis|Keine|
  |Hauptteil|1,2,3,... |
  |Literaturverzeichnis|i,ii,iii,... |

  |Anhang|iv,v,vi,... (mit vorherigen verknüpft)|

* Die einzelnen Abschnitte werden neu nummeriert und das Format der automatisch generierten Seitenzahlen im Inhaltsverzeichnis werden synchorisiert.
### 3. Die Format der Fußnote formuliert
Nach dem Standard wird die Format der Fußnote formuliert.

# LaTeX-Version
Diese Template basiert auf [Thesis Template for TH Deggendorf](https://www.overleaf.com/latex/templates/thesis-template-for-th-deggendorf/nwnndpxfttrb) von Prof. Dr. Andreas Fischer  und wird teilweise verändert. Diese Vorlage folgt der CC-BY-SA 4.0-Vereinbarung. Wenn Sie sie ändern möchten, lesen Sie bitte den Originaltext der Vereinbarung: [CC-BY-SA 4.0](https://creativecommons.org/licenses/by/4.0/deed.en)
## Struktur
|Teil|Ort|Komponenten|
|:-----:|:------:|:--------:|
|Umschlag|`/thesis/thesis.tex`|Variable mit `\newcommand`|
|Erklärung|`/thesis/declaration.tex`|Keine verfügbar in dieser Template. Wenn es nötig ist, bitte von der [Quelle](https://www.overleaf.com/latex/templates/thesis-template-for-th-deggendorf/nwnndpxfttrb) hinzuzufügen|
|Abstrakt|`/thesis/thesis.tex`|Ein Beispieltext der Abstrakt|
|Hauptteil|`/thesis/main.tex`|Ein Beispieltext des Hauptteils|
|Literaturverzeichnis|`/thesis/references.bib`|Man muss die Literatur in `/thesis/references.bib` zuerst hinzufügen und dann in `/thesis/main.tex` zitieren|
|Bilder|`/pictures`|Hier gibt es ein Beispiel: `/pictures/sample_pic.png`. Man kann die Bilder in diesem Ordner hinzufügen und im Artikel zitieren mit `\includegraphics`|
|Logo|`/logo`|Zwei Datei-Formaten des Logos werden geboten: `/logo/nanjing_tech.svg` und `/logo/nanjing_tech.ai`|
|Generierte Dateien|`/Makefile`|Generierte PDF-Datei|

*Achtung: Die Inhaltsverzeichnis wird automatisch generiert!*
## Genutzte LaTeX-Package
```
\usepackage[utf8]{inputenc}
\usepackage{graphicx}
\usepackage{booktabs}
\usepackage{url}
\usepackage{relsize}
\usepackage{hyperref}
\usepackage{libertine}
\usepackage{ifthen}
\usepackage{fancyhdr}
```
## Anhang
Für die `README.md` und das Syntax der Markdown bitte sehen Sie nach: [Markdown Basic Syntax](https://markdown.com.cn/basic-syntax/), [Markdown Extended Syntax](https://markdown.com.cn/extended-syntax/) <br>
Für die Grundwissen der LaTeX bitte sehen Sie nach: [StackExchange](https://tex.stackexchange.com/), [The Overleaf Tutorials](https://www.overleaf.com/learn) <br>
Für das Konvertieren des Schema zwischen GUI (Graphic User Interface) und LaTeX Syntax bitte sehen Sie nach: [Axmath](https://github.com/loongmxbt/AxMath) <br>
Für die Generierung der Tabelle bitte sehen Sie nach: [Tables Generator](https://www.tablesgenerator.com/) <br>
