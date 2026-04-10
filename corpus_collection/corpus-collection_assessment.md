---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
---

# 🏆Selbsttest: Wissen und Praxis

````{admonition} Hinweise
:class: hinweis
Diese Übungsaufgaben dienen Ihrer Selbsteinschätzung und helfen Ihnen, das im Kapitel Gelernte zu reflektieren.

Sie können die Fragen in beliebiger Reihenfolge beantworten und auch mehrfach versuchen.

**So funktioniert es:**
- Wählen Sie bei jeder Frage die Antwort(en), die Sie für richtig halten
- Lesen Sie das Feedback zu den einzelnen Antwortoptionen sorgfältig durch
- Die Erklärungen helfen Ihnen, Ihr Verständnis zu vertiefen – auch bei korrekten Antworten
- Wählen Sie bei jeder Frage die Antwort(en), die Sie für richtig halten.
- Lesen Sie das Feedback zu den einzelnen Antwortoptionen sorgfältig durch.
- Die Erklärungen helfen Ihnen, Ihr Verständnis zu vertiefen – auch bei korrekten Antworten.

Es erfolgt keine Bewertung oder Speicherung Ihrer Ergebnisse. Nutzen Sie dieses Assessment, um Wissenslücken zu identifizieren und gegebenenfalls die entsprechenden Abschnitte des Kapitels noch einmal zu bearbeiten.

**Geschätzte Zeit**: 1h

**Viel Erfolg!**
````

## Frage 1
(Wählen Sie alle zutreffenden Antworten aus.)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

"""
Lernziel:
    Sie können Korpora als geisteswissenschaftliche Forschungsobjekte definieren und ihre wesentlichen Merkmale beschreiben.
Bloom-Stufe: Verstehen
Format: Multiple Choice + Zuordnungsaufgabe
Geschätzte Zeit: 5 Minuten
Schwerpunkte:
    - Verständnis der Korpus-Grundprinzipien
    - Unterscheidung von Korpustypen
    - Bewertung von Korpusqualität
"""


question1 = [
    {
        "question": "Welche der folgenden Aussagen beschreiben korrekt die wesentlichen Merkmale eines Korpus in den Digital Humanities? Wählen Sie alle zutreffenden Aussagen.",
        "type": "multiple_choice",
        "answers": [
            {
                "answer": "Eine Sammlung von maschinenlesbaren Textdokumenten",
                "correct": True,
                "feedback": """✓ Korrekt! Die Maschinenlesbarkeit ist ein zentrales Merkmal von DH-Korpora, da sie die computergestützte Analyse ermöglicht. Dies unterscheidet DH-Korpora von traditionellen Textsammlungen und ist Voraussetzung für quantitative Analysen."""
            },
            {
                "answer": "Eine nach bestimmten Kriterien zusammengestellte Textsammlung",
                "correct": True,
                "feedback": """✓ Korrekt! Die kriteriengeleitete Zusammenstellung ist essentiell für wissenschaftliche Korpora. Die Kriterien müssen dabei:
                - transparent dokumentiert sein
                - zur Forschungsfrage passen
                - systematisch angewendet werden"""
            },
            {
                "answer": "Eine Sammlung, die nur digitalisierte Bücher enthält",
                "correct": False,
                "feedback": """× Nicht korrekt. Korpora können verschiedene Arten von Texten enthalten:
                - Zeitungsartikel (wie in unserer Fallstudie)
                - Literarische Texte
                - Dokumente
                - Andere Textformen
                Die Art der Texte wird durch die Forschungsfrage bestimmt, nicht durch das Format."""
            },
            {
                "answer": "Eine Textsammlung, die spezifischen Forschungszwecken dient",
                "correct": True,
                "feedback": """✓ Korrekt! Die Zweckgebundenheit ist ein wichtiges Merkmal:
                - Das Korpus wird für bestimmte Forschungsfragen zusammengestellt
                - Die Forschungszwecke bestimmen die Auswahlkriterien
                - Die Zweckbindung beeinflusst auch die Art der Aufbereitung der Texte"""
            },
            {
                "answer": "Eine beliebige Sammlung von digitalisierten Texten",
                "correct": False,
                "feedback": """× Nicht korrekt. Eine beliebige Sammlung erfüllt nicht die wissenschaftlichen Anforderungen an ein Korpus:
                - Es fehlen systematische Auswahlkriterien
                - Die Zusammenstellung ist nicht durch Forschungsfragen motiviert
                - Eine methodisch fundierte Analyse wäre nicht möglich"""
            },
            {
                "answer": "Eine Sammlung, die immer alle verfügbaren Texte zu einem Thema enthalten muss",
                "correct": False,
                "feedback": """× Nicht korrekt. Vollständigkeit ist nur eine mögliche Strategie des Korpusaufbaus:
                - Wie im Text erläutert, gibt es verschiedene Strategien (z.B. repräsentative Stichproben)
                - Die Vollständigkeit ist nur bei klar begrenzten, kleinen Untersuchungsbereichen sinnvoll
                - Die Strategie der Korpuserstellung richtet sich nach der Forschungsfrage und praktischen Erwägungen"""
            }
        ]
    }
]
display_quiz(question1, colors=colors.jupyterquiz, max_width=1000)
```

## Frage 2

Welche Aussage trifft auf das jeweilige Textformat zu? Wählen Sie für jede Aussage das passende Format.

### Frage 2(a)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

"""
Lernziel:
    Sie können die vier Hauptformate digitaler Texte (Bilddigitalisate, Plain Text, XML/TEI, CSV) anhand ihrer charakteristischen Eigenschaften unterscheiden und deren Vor- und Nachteile für spezifische Anwendungsfälle analysieren.
Bloom-Stufe: Analysieren
Format: Vergleichsmatrix + Multiple Choice
Geschätzte Zeit: 15 Minuten
Schwerpunkte:
    - Eigenschaften digitaler Textformate
    - Vor- und Nachteile verschiedener Formate
    - Formatauswahl für spezifische Zwecke
"""

statements = [
    {
        "question": "Dieses Format eignet sich besonders für linguistische Annotationen wie Wortarten und Lemmata in tabellarischer Form.",
        "type": "multiple_choice",
        "answers": [
            {
                "answer": "CSV",
                "correct": True,
                "feedback": "✓ Korrekt! Weil:\n    - Tabellarische Struktur ermöglicht klare Zuordnung von Token und Annotationen\n    - Einfache Verarbeitung mit Analysewerkzeugen\n    - Gut geeignet für große Datenmengen\n    - Standardformat für viele linguistische Tools"
            },
            {
                "answer": "XML/TEI",
                "correct": False,
                "feedback": """× Nicht optimal. Obwohl XML/TEI auch Annotationen unterstützt:
                    - Komplexerer Aufbau als nötig für einfache tabellarische Daten
                    - Weniger effizient für große Mengen einfach strukturierter Annotatione"""
            },
            {
                "answer": "Plain Text",
                "correct": False,
                "feedback": """× Nicht korrekt, weil:
                    - Keine Strukturierung für Annotationen möglich
                    - Keine Möglichkeit, zusätzliche Informationen systematisch zu speichern"""
            },
            {
                "answer": "Bilddigitalisate",
                "correct": False,
                "feedback": """× Nicht optimal, weil:
                    - Keine maschinenlesbare Textstruktur
                    - Keine Möglichkeit für systematische Annotationen"""
            }
        ]
    }
]
display_quiz(statements, colors=colors.jupyterquiz)
```


### Frage 2(b)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

statements = [
    {
        "question": "Dieses Format bewahrt die ursprüngliche visuelle Erscheinung des Dokuments, ist aber nicht direkt maschinenlesbar.",
        "type": "multiple_choice",
        "answers":  [
            {
                "answer": "CSV",
                "correct": False,
                "feedback": """× Nicht korrekt, weil:
                    - CSV nur tabellarische Daten speichert
                    - Keine visuellen Informationen enthält
                    - Primär für strukturierte Daten gedacht ist"""
            },
            {
                "answer": "XML/TEI",
                "correct": False,
                "feedback": """× Nicht ganz korrekt. XML/TEI:
                    - Kann zwar Layoutinformationen beschreiben
                    - Bewahrt aber nicht das visuelle Erscheinungsbild selbst
                    - Ist bereits maschinenlesbar"""
            },
            {
                "answer": "Plain Text",
                "correct": False,
                "feedback": """× Nicht korrekt, weil:
                    - Alle Formatierungen verloren gehen
                    - Nur der reine Text erhalten bleibt
                    - Keine visuellen Informationen gespeichert werden"""
            },
            {
                "answer": "Bilddigitalisate",
                "correct": True,
                "feedback": """✓ Korrekt! Bilddigitalisate (PDF, PNG, JPG) sind ideal dafür, weil sie:
                    - Layout und Typographie originalgetreu bewahren
                    - Illustrationen und grafische Elemente erhalten
                    - Als historische Referenz dienen können
                    Allerdings benötigen sie OCR für Textanalysen."""
            }
        ]
    }
]
display_quiz(statements, colors=colors.jupyterquiz)
```

## Frage 3

**Szenario:** Ein Forschungsprojekt möchte ein historisches Zeitungskorpus erstellen, das:
- für automatische Textanalysen nutzbar ist
- die ursprüngliche Seitengestaltung dokumentiert
- langfristig archiviert werden soll

**Frage:** Welches Format oder Kombination von Formaten würden Sie empfehlen?

```{code-cell} ipython3
:tags: [remove-input]
import sys
sys.path.append("../quadriga")  # Adjust path as needed
from assessment import create_answer_box

create_answer_box('korpus-1')
```

````{admonition}  Lösungen
:class: solution, dropdown
**Musterlösung:** XML oder Kombination aus Bilddigitalisaten (PDF) und Plain Text

**Begründung:**
XML:
- kann sowohl Text als auch Informationen zum originalen Layout in spezialisierten Tags speichern
- kann Text und Bildinformationen verknüpfen
- ermöglicht automatische Textanalysen
- eignet sich zur Langzeitarchivierung
- Nachteil: Die Verarbeitung ist komplexer als die von Plain Text

Bilddigitalisate (PDF):
- Bewahren das originale Layout
- Dienen als Referenz
- Eignen sich für die Langzeitarchivierung
- Nachteil: automatische Prozessierung und Verknüpfung zu Plain Text ist nicht möglich

Plain Text (nach OCR):
- Ermöglicht automatische Textanalysen
- Einfach zu verarbeiten
- Geringer Speicherbedarf

Alternative Ansätze:
- CSV ist nicht geeignet für Volltext
- Nur Bilddigitalisate würden Analysen erschweren
- Nur Plain Text dokumentiert die ursprüngliche Seitengestaltung nicht
````
## Frage 4
(Wählen Sie alle zutreffenden Antworten aus.)

### Frage 4(a)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

format_questions = [
    {
        "question": "Welche der folgenden Formate sind direkt maschinenlesbar? (Mehrere Antworten können korrekt sein)",
        "type": "multiple_choice",
        "answers": [
            {
                "answer": "Bilddigitalisate",
                "correct": False,
                "feedback": "Falsch. Bilddigitalisate benötigen erst OCR (Optical Character Recognition), um für Maschinen lesbar zu werden. Die Inhalte sind für Computer nicht direkt zugänglich."
            },
            {
                "answer": "Plain Text",
                "correct": True,
                "feedback": "Richtig. Text in einfachen Textdateien kann direkt von Algorithmen gelesen und verarbeitet werden."
            },
            {
                "answer": "XML/TEI",
                "correct": True,
                "feedback": "Richtig. XML und TEI sind strukturierte Textformate, die von Computern direkt verarbeitet werden können."
            },
            {
                "answer": "CSV",
                "correct": True,
                "feedback": "Richtig. Comma-Separated Values sind strukturierte Daten, die direkt maschinenlesbar sind."
            }
        ]
    }
]

display_quiz(format_questions, colors=colors.jupyterquiz)
```

### Frage 4(b)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

format_questions = [
    {
        "question": "Welche der folgenden Formate können Formatierungen (z.B. Kursivierung / Fettung) darstellen oder speichern? (Mehrere Antworten können korrekt sein)",
        "type": "multiple_choice",
        "answers": [
            {
                "answer": "Bilddigitalisate",
                "correct": True,
                "feedback": "Richtig. Sie bewahren alle visuellen Formatierungen des Originaldokuments."
            },
            {
                "answer": "Plain Text",
                "correct": False,
                "feedback": "Falsch. In reinen Textdateien können keine Formatierungen (wie Fettdruck, Kursiv, etc.) gespeichert werden."
            },
            {
                "answer": "XML/TEI",
                "correct": True,
                "feedback": "Richtig. Diese Formate können Formatierungen strukturiert beschreiben und kodieren."
            },
            {
                "answer": "CSV",
                "correct": False,
                "feedback": "Falsch. CSV-Dateien können nur tabellarische Strukturen speichern, aber keine Textformatierungen."
            }
        ]
    }
]

display_quiz(format_questions, colors=colors.jupyterquiz)
```

### Frage 4(c)
```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

format_questions = [
    {
        "question": "Welche der folgenden Formate eignen sich für linguistische Annotationen? (Mehrere Antworten können korrekt sein)",
        "type": "multiple_choice",
        "answers": [
            {
                "answer": "Bilddigitalisate",
                "correct": False,
                "feedback": "Falsch. Ohne Textextraktion können keine linguistischen Informationen hinzugefügt werden."
            },
            {
                "answer": "Plain Text",
                "correct": True,
                "feedback": "Teilweise richtig. Grundlegende Annotationen können durch zusätzliche Zeichen eingefügt werden, aber die Möglichkeiten sind sehr begrenzt."
            },
            {
                "answer": "XML/TEI",
                "correct": True,
                "feedback": "Richtig. Diese Formate wurden speziell für strukturierte Textannotationen entwickelt und eignen sich hervorragend für linguistische Informationen."
            },
            {
                "answer": "CSV",
                "correct": True,
                "feedback": "Teilweise richtig. Tabellarische Strukturen können linguistische Merkmale in separaten Spalten speichern, sind aber für komplexe hierarchische Annotationen weniger geeignet."
            }
        ]
    }
]

display_quiz(format_questions, colors=colors.jupyterquiz)
```

### Frage 4(d)
```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

format_questions = [
    {
        "question": "Zusatzfrage: Welche der folgenden Formate sind besonders speichereffizient? (Mehrere Antworten können korrekt sein)",
        "type": "multiple_choice",
        "answers": [
            {
                "answer": "Bilddigitalisate",
                "correct": False,
                "feedback": "Falsch. Bilddateien benötigen in der Regel viel Speicherplatz, besonders bei hoher Auflösung."
            },
            {
                "answer": "Plain Text",
                "correct": True,
                "feedback": "Richtig. Reiner Text ohne Metadaten oder Formatierungen braucht sehr wenig Speicherplatz."
            },
            {
                "answer": "XML/TEI",
                "correct": False,
                "feedback": "Falsch. Durch die zusätzlichen Tags und strukturellen Informationen benötigen diese Formate mehr Speicherplatz als Plain Text."
            },
            {
                "answer": "CSV",
                "correct": True,
                "feedback": "Richtig. Tabellarische Daten in CSV-Format sind sehr speichereffizient für strukturierte Informationen."
            }
        ]
    }
]

display_quiz(format_questions, colors=colors.jupyterquiz)
```

### Frage 4(e)
```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

format_questions = [
    {
        "question": "Welche der folgenden Formate bewahren visuelle Informationen? (Mehrere Antworten können korrekt sein)",
        "type": "multiple_choice",
        "answers": [
            {
                "answer": "Bilddigitalisate",
                "correct": True,
                "feedback": "Richtig. Sie enthalten die vollständige visuelle Information des Originaldokuments."
            },
            {
                "answer": "Plain Text",
                "correct": False,
                "feedback": "Falsch. Visuelle Informationen wie Layout, Schriftarten oder Bilder gehen in Plain Text vollständig verloren."
            },
            {
                "answer": "XML/TEI",
                "correct": True,
                "feedback": "Teilweise richtig. Layout und visuelle Strukturen können beschrieben werden, aber die tatsächlichen visuellen Informationen werden nicht direkt gespeichert."
            },
            {
                "answer": "CSV",
                "correct": False,
                "feedback": "Falsch. CSV-Dateien speichern nur tabellarische Daten ohne visuelle Informationen."
            }
        ]
    }
]

display_quiz(format_questions, colors=colors.jupyterquiz)
```

## Frage 5
(Wählen Sie alle zutreffenden Antworten aus.)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

"""
Lernziel:
    Sie können die grundlegenden Metadatenschemata (Dublin Core, TEI, MODS, METS) und deren charakteristische Elemente für Korpora und Einzeldokumente beschreiben.
Bloom-Stufe: Verstehen
Format: Multiple Choice + Selbsteinschätzung
Zeitaufwand: 25 Minuten
Schwerpunkte:
    - Verständnis verschiedener Metadatenschemata (Dublin Core, TEI, MODS, METS)
    - Kenntnis charakteristischer Elemente
    - Unterscheidung Korpus- und Dokumentebene
"""

question5 = [
    {
        "question": "Welche Aussagen beschreiben die verschiedenen Metadatenschemata korrekt?",
        "type": "multiple_choice",
        "answers": [
            {
                "answer": "Dublin Core umfasst 15 grundlegende Elemente wie Titel, Autor und Datum",
                "correct": True,
                "feedback": """✓ Richtig! Dublin Core:
                - Bietet ein einfaches, universelles Schema
                - Die 15 Kernelemente sind standardisiert
                - Eignet sich für grundlegende Beschreibungen
                - Ist weit verbreitet und leicht anzuwenden"""
            },
            {
                "answer": "TEI wurde speziell für die Auszeichnung von Texten entwickelt und speichert Metadaten im teiHeader",
                "correct": True,
                "feedback": """✓ Richtig! TEI:
                - Ist ein spezialisiertes Schema für Texte
                - Nutzt den teiHeader für Metadaten
                - Ermöglicht detaillierte Textauszeichnung
                - Bietet umfangreiche Beschreibungsmöglichkeiten"""
            },
            {
                "answer": "MODS und METS sind identische Standards für Bibliotheken",
                "correct": False,
                "feedback": """× Nicht korrekt. Die Standards unterscheiden sich:
                - MODS ist für bibliographische Beschreibungen
                - METS dient der Kodierung und Übertragung von Digitalisaten
                - Beide haben unterschiedliche Schwerpunkte und Anwendungsbereiche"""
            }
        ]
    }
]
display_quiz(question5, colors=colors.jupyterquiz)
```

## Frage 6

### Frage 6(a)
```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

metadata_questions = [
    {
        "question": """Zu welchem Metadatenschema gehört das Element "teiHeader"?""",
        "type": "multiple_choice",
        "answers": [
            {
                "answer": "Dublin Core",
                "correct": False,
                "feedback": """× Falsch. Der "teiHeader" ist ein Element aus dem TEI-Schema, nicht aus Dublin Core."""
            },
            {
                "answer": "TEI",
                "correct": True,
                "feedback": """✓ Richtig. Der "teiHeader" ist ein zentrales Element des TEI-Schemas (Text Encoding Initiative) und dient der strukturierten Beschreibung von Metadaten in TEI-Dokumenten."""
            },
            {
                "answer": "MARC",
                "correct": False,
                "feedback": """× Falsch. MARC ist ein bibliothekarisches Metadatenformat und enthält kein "teiHeader"-Element."""
            },
            {
                "answer": "MODS",
                "correct": False,
                "feedback": """× Falsch. MODS (Metadata Object Description Schema) ist ein XML-Schema für bibliografische Metadaten, aber enthält kein "teiHeader"-Element."""
            }
        ]
    }
]

display_quiz(metadata_questions, colors=colors.jupyterquiz)
```

### Frage 6(b)
```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

metadata_questions = [
    {
        "question": """Zu welchem Metadatenschema gehört das Element "DC.coverage"?""",
        "type": "multiple_choice",
        "answers": [
            {
                "answer": "Dublin Core",
                "correct": True,
                "feedback": """✓ Richtig. \"DC.coverage\" ist ein Element aus dem Dublin Core Metadatenstandard, das räumliche und zeitliche Angaben zum beschriebenen Objekt enthält."""
            },
            {
                "answer": "TEI",
                "correct": False,
                "feedback": """× Falsch. Obwohl TEI Dublin Core Elemente integrieren kann, ist \"DC.coverage\" kein genuines TEI-Element."""
            },
            {
                "answer": "MARC",
                "correct": False,
                "feedback": """× Falsch. MARC verwendet andere Bezeichnungen für räumliche und zeitliche Abdeckungen."""
            },
            {
                "answer": "MODS",
                "correct": False,
                "feedback": """× Falsch. MODS hat eigene Elemente für geografische und chronologische Informationen."""
            }
        ]
    }
]

display_quiz(metadata_questions, colors=colors.jupyterquiz)
```
### Frage 6(c)
```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

metadata_questions = [
    {
        "question": """Auf welcher Beschreibungsebene wird das "DC.coverage"-Element typischerweise verwendet?""",
        "type": "multiple_choice",
        "answers": [
            {
                "answer": "Nur auf Korpus-Level",
                "correct": True,
                "feedback": """✓ Richtig. "DC.coverage" beschreibt typischerweise die zeitliche und räumliche Abdeckung einer gesamten Sammlung und wird daher vorwiegend auf Korpus-Level eingesetzt. Es definiert den Rahmen der Sammlung und ist wichtig für die Gesamteinordnung des Korpus."""
            },
            {
                "answer": "Nur auf Dokument-Level",
                "correct": False,
                "feedback": """× Falsch. Obwohl "DC.coverage" auch auf Dokumentebene verwendet werden kann, ist es in der Praxis besonders relevant für die Korpus-Beschreibung."""
            },
            {
                "answer": "Sowohl auf Korpus- als auch auf Dokument-Level",
                "correct": False,
                "feedback": """× Falsch. Im Kontext dieser Fallstudie wird "DC.coverage" vorrangig auf Korpus-Level verwendet."""
            },
            {
                "answer": "Auf keiner der genannten Ebenen",
                "correct": False,
                "feedback": """× Falsch. "DC.coverage" ist ein wichtiges Element für die Metadatenbeschreibung, insbesondere auf Korpus-Level."""
            }
        ]
    }
]

display_quiz(metadata_questions, colors=colors.jupyterquiz)
```


## Frage 7

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

question7 = [
    {
        "question": "Welche Metadatenelemente sind charakteristisch für die Beschreibung einzelner Korpus-Dokumente?",
        "type": "multiple_choice",
        "answers": [
            {
                "answer": "Eindeutiger Identifikator (z.B. DOI oder spezifische Kennung)",
                "correct": True,
                "feedback": """✓ Richtig! Ein eindeutiger Identifikator:
                - Ist essentiell für die Dokumentidentifikation
                - Ermöglicht präzise Referenzierung
                - Unterstützt die Langzeitarchivierung
                - Erleichtert die Verknüpfung von Dokumenten"""
            },
            {
                "answer": "Gesamtumfang des Korpus",
                "correct": False,
                "feedback": """× Nicht korrekt! Der Gesamtumfang:
                - Ist ein Korpus-Level Metadatum
                - Beschreibt die gesamte Sammlung
                - Gehört nicht zur Dokumentbeschreibung"""
            }
        ]
    }
]
display_quiz(question7, colors=colors.jupyterquiz)
```
````{admonition} Lösungen
:class: solution, dropdown
Für Einzeldokumente sind stattdessen relevant:
- Individuelle Eigenschaften
- Spezifische Publikationsdaten
- Dokumentspezifische Merkmale
````

## Frage 8

### Frage 8(a)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

metadata_schema_questions = [
    {
        "question": "Welches Metadatenschema wird als \"einfach und universell verwendbar, mit grundlegenden Elementen\" beschrieben?",
        "type": "multiple_choice",
        "answers": [
            {
                "answer": "Dublin Core",
                "correct": True,
                "feedback": """✓ Richtig. Dublin Core ist bewusst einfach gehalten, universal einsetzbar und besteht aus 15 Kernelementen, die grundlegend für die Beschreibung digitaler Ressourcen sind. Es ist weit verbreitet und international standardisiert."""
            },
            {
                "answer": "TEI",
                "correct": False,
                "feedback": """× Falsch. TEI ist ein komplexeres Schema, das speziell für die Auszeichnung und Beschreibung von Texten entwickelt wurde, nicht primär für universelle Einfachheit."""
            },
            {
                "answer": "MARC",
                "correct": False,
                "feedback": """× Falsch. MARC ist ein umfassendes Format für bibliographische Informationen, aber nicht als besonders einfach oder universell bekannt."""
            },
            {
                "answer": "METS",
                "correct": False,
                "feedback": """× Falsch. METS ist ein XML-Schema für Metadaten zu digitalen Objekten in Repositorien, aber nicht primär für Einfachheit konzipiert."""
            }
        ]
    }
]

display_quiz(metadata_schema_questions, colors=colors.jupyterquiz)
```
### Frage 8(b)
```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

metadata_schema_questions = [
    {
        "question": "Welches Metadatenschema wird als \"spezialisiert auf Textauszeichnung und -beschreibung\" charakterisiert?",
        "type": "multiple_choice",
        "answers": [
            {
                "answer": "Dublin Core",
                "correct": False,
                "feedback": """× Falsch. Dublin Core bietet allgemeine Metadatenelemente, ist aber nicht speziell für detaillierte Textauszeichnung konzipiert."""
            },
            {
                "answer": "TEI",
                "correct": True,
                "feedback": """✓ Richtig. Die Text Encoding Initiative (TEI) wurde speziell für Texte entwickelt und ermöglicht detaillierte Textauszeichnung mit umfangreichen Beschreibungsmöglichkeiten. Der spezialisierte teiHeader erlaubt eine präzise Beschreibung von Textdokumenten."""
            },
            {
                "answer": "MARC",
                "correct": False,
                "feedback": """× Falsch. MARC dient in erster Linie der bibliographischen Beschreibung, nicht der Auszeichnung von Textinhalten."""
            },
            {
                "answer": "METS",
                "correct": False,
                "feedback": """× Falsch. METS beschreibt die Struktur digitaler Objekte, ist aber nicht speziell für Textauszeichnung konzipiert."""
            }
        ]
    }
]

display_quiz(metadata_schema_questions, colors=colors.jupyterquiz)
```

### Frage 8(c)
```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

metadata_schema_questions = [
    {
        "question": "Welches Metadatenschema wird als \"umfassend für bibliographische Informationen\" beschrieben?",
        "type": "multiple_choice",
        "answers": [
            {
                "answer": "Dublin Core",
                "correct": False,
                "feedback": """× Falsch. Dublin Core bietet zwar bibliographische Grundelemente, ist aber nicht so umfassend wie spezialisierte bibliographische Formate."""
            },
            {
                "answer": "TEI",
                "correct": False,
                "feedback": """× Falsch. TEI kann bibliographische Informationen enthalten, ist aber primär ein Textauszeichnungsformat."""
            },
            {
                "answer": "MARC",
                "correct": True,
                "feedback": """✓ Richtig. MARC (Machine-Readable Cataloging) wurde speziell für umfassende bibliographische Informationen entwickelt und ist ein Standard in Bibliotheken weltweit. Es enthält detaillierte Felder für alle Aspekte bibliographischer Beschreibung."""
            },
            {
                "answer": "EAD",
                "correct": False,
                "feedback": """× Falsch. Encoded Archival Description ist für archivische Findmittel konzipiert, nicht primär für bibliographische Daten."""
            }
        ]
    }
]

display_quiz(metadata_schema_questions, colors=colors.jupyterquiz)
```

### Frage 8(d)
```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

metadata_schema_questions = [
    {
        "question": "Welches Metadatenschema wird als \"Standard für Digitalisate und deren Übertragung\" bezeichnet?",
        "type": "multiple_choice",
        "answers": [
            {
                "answer": "Dublin Core",
                "correct": False,
                "feedback": """× Falsch. Dublin Core bietet zwar einen einfachen Standard für digitale Ressourcen, ist aber nicht speziell auf Digitalisate und deren Übertragung ausgerichtet."""
            },
            {
                "answer": "TEI",
                "correct": False,
                "feedback": """× Falsch. TEI konzentriert sich auf die Auszeichnung und Beschreibung von Texten, nicht auf die Übertragung von Digitalisaten."""
            },
            {
                "answer": "MARC",
                "correct": False,
                "feedback": """× Falsch. MARC dient hauptsächlich der bibliographischen Beschreibung, nicht dem Management von Digitalisaten."""
            },
            {
                "answer": "METS",
                "correct": True,
                "feedback": """✓ Richtig. Das Metadata Encoding and Transmission Standard (METS) wurde speziell für die Beschreibung und Übertragung digitaler Objekte in Repositorien entwickelt. Es dient als Container für verschiedene Metadatentypen und unterstützt die strukturierte Beschreibung von Digitalisaten."""
            }
        ]
    }
]

display_quiz(metadata_schema_questions, colors=colors.jupyterquiz)
```

## Frage 9

```{code-cell} ipython3
:tags: [remove-input]
import sys
sys.path.append("../quadriga")
from assessment import DragDropQuiz

quiz = DragDropQuiz()

quiz.create_matching_quiz(
    title="Ordnen Sie die folgenden Schritte beim Korpusaufbau in die richtige Reihenfolge:",
    descriptions=["Entwicklung des Korpuskonzepts",
        "Test der Sammlungsmethodik",
        "Festlegung des Metadatenstruktur",
        "Dokumentation der Auswahlkriterien",
        "Durchführung der Datensammlung"],
    options=["1", "2", "3", "4", "5"],
    correct_mapping={
        "Entwicklung des Korpuskonzepts" : "1",
        "Dokumentation der Auswahlkriterien" : "2",
        "Festlegung des Metadatenstruktur" : "3",
        "Test der Sammlungsmethodik" : "4",
        "Durchführung der Datensammlung" : "5"
    }
)
```

## Frage 10

Analysieren Sie den folgenden Ausschnitt aus einem Korpusaufbau-Konzept:

"Für das Zeitungskorpus zur Spanischen Grippe werden Ausgaben der Berliner Morgenpost und der Vossischen Zeitung aus den Jahren 1918-1919 gesammelt. Die Zeitungen sind über ZEFYS als PDF verfügbar. Aufgrund der Datenmenge (ca. 2 TB) wird ein balanciertes Korpus mit repräsentativen Stichproben erstellt."

Bewerten Sie die folgenden Aspekte:

1.	Quellenauswahl
2.	Technische Umsetzbarkeit
3.	Praktische Einschränkungen
4.	Lösungsansatz

```{code-cell} ipython3
:tags: [remove-input]
import sys
sys.path.append("../quadriga")  # Adjust path as needed
from assessment import create_answer_box

create_answer_box('korpus-2')
```


````{admonition} Lösungen
:class: solution, dropdown

**Musterlösung**:

1. Quellenauswahl:
    - Zwei relevante Berliner Zeitungen
    - Zeitraum entspricht Pandemieverlauf
    - Digitale Verfügbarkeit gegeben

2. Technische Umsetzbarkeit:
    - Zugang über ZEFYS-Portal möglich
    - PDF-Format erfordert OCR
    - Systematischer Download möglich

3. Praktische Einschränkungen:
    - Sehr große Datenmenge (2 TB)
    - Hoher Speicherbedarf
    - Aufwendige Verarbeitung

4. Lösungsansatz:
    - Balanciertes Korpus als Alternative
    - Repräsentative Stichproben
    - Praktikable Größe bei wissenschaftlicher Qualität
````
