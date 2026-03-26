(ocr_tesseract-installation)=
# Installation von Tesseract und weiteren Werkzeugen

Die Jupyter Notebooks in diesem Kapitel verwenden **Tesseract OCR** zur Texterkennung sowie einige weitere Werkzeuge. Bevor Sie die Notebooks ausführen können, müssen diese Werkzeuge auf Ihrem System installiert sein.

```{admonition} Cloud Mode (Colab)
:class: tip
Wenn Sie die Notebooks über **Google Colab** ausführen, müssen Sie nichts manuell installieren — die Notebooks erledigen die Installation automatisch.
```

Die folgenden Installationsanleitungen richten sich an Nutzer\*innen im **Local Mode**, die die Notebooks auf dem eigenen Computer ausführen möchten.

## Tesseract OCR

Tesseract ist die eigentliche OCR-Engine, die im Hintergrund die Texterkennung durchführt. Das Python-Paket `pytesseract` ist lediglich ein Wrapper, der Tesseract aus Python heraus ansteuert. Daher muss Tesseract als eigenständiges Programm auf Ihrem System installiert sein.

Für diese Fallstudie benötigen wir zusätzlich das **Fraktur-Modell** (`frk`), da wir mit historischen deutschsprachigen Zeitungstexten in Frakturschrift arbeiten.

### Windows

1. Laden Sie den Installer von der Seite der UB Mannheim herunter: <a href="https://github.com/UB-Mannheim/tesseract/wiki" class="external-link" target="_blank">github.com/UB-Mannheim/tesseract/wiki</a>
2. Führen Sie den Installer aus. Wählen Sie bei der Komponentenauswahl unter *Additional script data* bzw. *Additional language data* das **German Fraktur** (`frk`) Modell aus.
3. Merken Sie sich den Installationspfad (standardmäßig `C:\Program Files\Tesseract-OCR`).

```{admonition} PATH-Variable unter Windows
:class: warning
Damit `pytesseract` Tesseract finden kann, muss der Installationspfad in der **PATH-Umgebungsvariable** eingetragen sein. Der Installer bietet diese Option an — aktivieren Sie sie.

Falls Tesseract trotzdem nicht gefunden wird, können Sie den Pfad auch direkt in Python angeben:

    import pytesseract
    pytesseract.pytesseract.tesseract_cmd = r'C:\Program Files\Tesseract-OCR\tesseract.exe'
```

### macOS

Installieren Sie Tesseract über <a href="https://brew.sh" class="external-link" target="_blank">Homebrew</a>:

```bash
brew install tesseract
```

Für das Fraktur-Modell gibt es zwei Möglichkeiten:

**Option A** — Alle Sprachmodelle installieren (einfacher, aber größerer Download):
```bash
brew install tesseract-lang
```

**Option B** — Nur das Fraktur-Modell manuell herunterladen:
1. Laden Sie die Datei `frk.traineddata` aus dem offiziellen Repository herunter: <a href="https://github.com/tesseract-ocr/tessdata/blob/main/frk.traineddata" class="external-link" target="_blank">github.com/tesseract-ocr/tessdata</a>
2. Kopieren Sie die Datei in das Tesseract-Datenverzeichnis:
   - Apple Silicon (M1/M2/…): `/opt/homebrew/share/tessdata/`
   - Intel Mac: `/usr/local/share/tessdata/`

### Linux (Debian/Ubuntu)

```bash
sudo apt install tesseract-ocr tesseract-ocr-frk
```

## Poppler (für PDF-Verarbeitung)

Das Python-Paket `pdf2image`, das wir zur Umwandlung von PDF-Seiten in Bilder verwenden, benötigt **Poppler** als Backend.

### Windows

Installieren Sie Poppler über Conda (empfohlen, wenn Sie Anaconda verwenden):
```bash
conda install -c conda-forge poppler
```

Alternativ können Sie vorkompilierte Binärdateien herunterladen: <a href="https://github.com/oschwartz10612/poppler-windows/releases" class="external-link" target="_blank">github.com/oschwartz10612/poppler-windows/releases</a>. Entpacken Sie das Archiv und fügen Sie den `bin`-Ordner zur PATH-Umgebungsvariable hinzu.

### macOS

```bash
brew install poppler
```

### Linux (Debian/Ubuntu)

```bash
sudo apt install poppler-utils
```

## Python-Pakete

Die benötigten Python-Pakete sind betriebssystemunabhängig und können mit `pip` installiert werden:

```bash
pip install pytesseract pillow pdf2image tqdm
```

Für das Notebook zur Messung der OCR-Qualität wird zusätzlich benötigt:

```bash
pip install Levenshtein
```

```{admonition} Überprüfung der Installation
:class: hint
Um zu prüfen, ob Tesseract korrekt installiert ist, können Sie folgenden Befehl im Terminal ausführen:

    tesseract --version

Wenn eine Versionsnummer angezeigt wird, ist die Installation erfolgreich.
```
