(ocr_intro)=

# OCR. Von Bild zu Text

````{margin}
```{admonition} Fragen oder Feedback 
:class: frage-feedback

<a href="https://github.com/quadriga-dk/Text-Fallstudie-1/issues/new?assignees=&labels=question&projects=&template=frage.yml" class="external-link" target="_blank">
    Stellen Sie eine Frage.
</a> <br>
<a href="https://github.com/quadriga-dk/Text-Fallstudie-1/issues/new?assignees=&labels=feedback&projects=&template=feedback.yml" class="external-link" target="_blank">
    Geben Sie uns Feedback.
</a>

Mit Ihren Rückmeldungen können wir unser interaktives Lehrbuch gezielt an Ihre Bedürfnisse anpassen.

```
````

`````{margin}
````{admonition} Zitierhinweis
:class: citation-information
```{literalinclude} /CITATION.bib
:language: bibtex
```
Skorinkin, D., Sluyter-Gäthje, H. & Trilcke, P. (2024). _Quantitative Analyse der Medienwellen der Spanischen Grippe (1918/19). Eine Fallstudie._ https://doi.org/10.5281/zenodo.15682652

`````

```{include} ../introduction/learning-outcomes.md
:start-after: "<!-- START: OCR. Von Bild zu Text -->"
:end-before: "<!-- END: OCR. Von Bild zu Text -->"
```

Nach dem vorherigen [Kapitel](../corpus_collection/corpus-collection_summary) haben wir also ein Korpus als Sammlung gescannter Bilder. Ein Korpus in dieser Form ist jedoch noch **nicht maschinenlesbar** und kann nicht direkt verarbeitet werden. In diesem Kapitel lernen wir, wie man mit OCR **Bilder in Text umwandelt**.

```{figure} ../assets/images/flow-chart_ocr.jpeg
---
height:
name: Flussdiagramm der Fallstudie
---
Flussdiagramm der Fallstudie. Wir befinden uns im dritten Arbeitspaket.
```
Zunächst werden wir lernen, [was OCR ist](ocr), warum wir es brauchen und wie es funktioniert. Außerdem werden wir einen Überblick über einige OCR-Tools geben.

Anschließend werden wir [OCR in Python mit PyTesseract](ocr_pytesseract_intro) durchführen, einem kostenlosen und quelloffenen OCR-Tool.

Schließlich werden wir die Metriken kennenlernen, die zur Messung der [OCR-Qualität](ocr-quality) verwendet werden, und [Qualitätsmessungen](ocr_ocr-quality) durchführen.
