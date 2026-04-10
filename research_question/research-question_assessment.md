---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
---

# 🏆Selbsttest: Wissen und Praxis

````{admonition} Hinweis
:class: hinweis
Diese Übungsaufgaben dienen Ihrer Selbsteinschätzung und helfen Ihnen dabei, das im Kapitel Gelernte zu reflektieren.

Sie können die Fragen in beliebiger Reihenfolge beantworten und jeden Versuch bei Bedarf mehrfach wiederholen.

**So funktioniert es:**
- Wählen Sie bei jeder Frage die Antwort(en) aus, die Sie für richtig halten
- Lesen Sie das Feedback zu den einzelnen Antwortoptionen sorgfältig durch
- Die Erklärungen helfen Ihnen dabei, Ihr Verständnis zu vertiefen – auch bei korrekten Antworten

Es erfolgt keine Bewertung oder Speicherung Ihrer Ergebnisse. Nutzen Sie dieses Assessment, um Wissenslücken zu identifizieren und gegebenenfalls die entsprechenden Abschnitte des Kapitels noch einmal zu bearbeiten.

**Geschätzte Zeit**: 15min

Viel Erfolg!
````

## Frage 1

Eine Forschungsfrage im Bereich der Digital Humanities lautet: "Wie entwickelte sich die öffentliche Aufmerksamkeit für Umweltthemen in deutschen Tageszeitungen zwischen 1960–1980?"

(Wählen Sie alle zutreffenden Antworten aus)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

question2 = [
    {
        "question": "Welche der folgenden Operationalisierungen eignen sich, um die öffentliche Aufmerksamkeit für Umweltthemen in deutschen Tageszeitungen zwischen 1960–1980 messbar zu machen? (Mehrere Antworten sind korrekt)",
        "type": "multiple_choice",
        "answers": [
            {
                "answer": "Zählen der Häufigkeit von umweltbezogenen Begriffen (wie 'Umweltschutz', 'Verschmutzung') in den Zeitungstexten",
                "correct": True,
                "feedback": """✓ Korrekt! Diese Operationalisierung ist geeignet, weil:
                    - Sie ein quantifizierbares Maß für die Intensität der Berichterstattung liefert
                    - Die Häufigkeit von Schlüsselbegriffen messbar ist
                    - Systematische Vergleiche über Zeit möglich sind
                    - Die Analyse auf dem definierten Korpus basiert"""
            },
            {
                "answer": "Messen der Länge von Artikeln, die Umweltthemen behandeln",
                "correct": True,
                "feedback": """✓ Korrekt! Diese Methode ist geeignet, weil:
                    - Sie den Umfang der Berichterstattung quantifiziert
                    - Längere Artikel oft mehr Aufmerksamkeit bedeuten
                    - Die Messung über Zeit vergleichbar ist
                    - Die Analyse innerhalb des Quellenkorpus bleibt"""
            },
            {
                "answer": "Erfassen der tatsächlichen Umweltverschmutzungswerte aus diesem Zeitraum",
                "correct": False,
                "feedback": """× Nicht korrekt, weil:
                    - Dies keine mediale Aufmerksamkeit misst
                    - Es außerhalb des Untersuchungskorpus liegt
                    - Es das tatsächliche Geschehen statt der Berichterstattung erfasst
                    - Es nicht die Forschungsfrage beantwortet"""
            },
            {
                "answer": "Analyse von Regierungsdokumenten zur Umweltpolitik",
                "correct": False,
                "feedback": """× Nicht korrekt, weil:
                    - Dies außerhalb des definierten Quellenkorpus (Tageszeitungen) liegt
                    - Es eine andere Textgattung betrifft
                    - Es nicht die mediale Aufmerksamkeit misst
                    - Es eine andere Forschungsfrage erfordern würde"""
            },
            {
                "answer": "Erfassen des prozentualen Anteils der Zeitungsseiten mit Umweltthemen",
                "correct": True,
                "feedback": """✓ Korrekt! Diese Operationalisierung ist geeignet, weil:
                    - Sie den relativen Stellenwert des Themas misst
                    - Sie verschiedene Zeitpunkte vergleichbar macht
                    - Sie auf dem definierten Korpus basiert
                    - Sie ein quantifizierbares Maß liefert"""
            }
        ]
    }
]
display_quiz(question2, colors=colors.jupyterquiz, max_width=1000)
```

## Frage 2
Entwickeln Sie eine Operationalisierung für folgende Forschungsfrage: "Wie veränderte sich die Berichterstattung über wissenschaftliche Themen in der Wochenzeitung 'Die Zeit' zwischen 1950–1970?"

### Frage 2(a)
Formulieren Sie zunächst selbst eine mögliche Operationalisierung

```{code-cell} ipython3
:tags: [remove-input]
import sys
sys.path.append("../quadriga")  # Adjust path as needed
from assessment import create_answer_box

create_answer_box('1')
```

### Frage 2(b)
Vergleichen Sie Ihre Antwort mit den folgenden Kriterien für eine geeignete Operationalisierung. Bewerten Sie Ihre eigene Antwort anhand dieser Kriterien


```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

questions = [
    {
        "question": "Verwendet Ihre Operationalisierung quantifizierbare Indikatoren?",
        "type": "multiple_choice",
        "answers": [
            {
                "answer": "Ja",
                "correct": True,
                "feedback": "✓ Korrekt!"
            },
            {
                "answer": "Nein",
                "correct": False,
                    "feedback": """× Nicht korrekt! Die Indikatoren müssen in Zahlen ausdrückbar sein
                    - Beispiele für quantifizierbare Indikatoren:
                    - Worthäufigkeiten (z.B. Anzahl wissenschaftsbezogener Begriffe), Textlängen (z.B. Wörter pro Artikel), Prozentuale Anteile (z.B. Anteil am Gesamtumfang)
                    - Gegenbeispiele (nicht quantifizierbar):
                    "Wichtigkeit" ohne weitere Spezifikation, "Qualität der Berichterstattung" ohne Messkriterien, Vage Beschreibungen wie "häufig" oder "selten"."""
            }
        ]
    },
    {
        "question": "Basieren die Messungen auf dem definierten Quellenkorpus (Die Zeit)?",
        "type": "multiple_choice",
        "answers": [
            {
                "answer": "Ja",
                "correct": True,
                "feedback": "✓ Korrekt!"
            },
            {
                "answer": "Nein",
                "correct": False,
                "feedback": """× Nicht korrekt! Alle Messungen müssen im Korpus der "Zeit" durchführbar sein.
                - Zu beachten:
                Verfügbarkeit aller Ausgaben im Untersuchungszeitraum,
                Konsistenz des Zeitungsformats,
                Zugänglichkeit der relevanten Artikel.
                - Nicht geeignet sind Messungen, die:
                Andere Zeitungen einbeziehen,
                Externe Datenquellen erfordern,
                Nicht im Zeitungskorpus enthaltene Informationen benötigen"""
            }
        ]
    },
    {
        "question": "Lassen sich die Messungen über den gesamten Zeitraum durchführen?",
        "type": "multiple_choice",
        "answers": [
            {
                "answer": "Ja",
                "correct": True,
                "feedback": "✓ Korrekt!"
            },
            {
                "answer": "Nein",
                "correct": False,
                "feedback": """× Nicht korrekt! Die Messungen müssen von 1950–1970 konsistent möglich sein
                - Wichtige Aspekte:
                Gleichbleibende Verfügbarkeit der Daten,
                Vergleichbarkeit der Messungen über Zeit,
                Berücksichtigung möglicher Formatänderungen.
                - Problematisch wären:
                Indikatoren, die nur für Teilzeiträume verfügbar sind,
                Messungen, die durch Änderungen der Zeitung beeinflusst werden,
                Nicht durchgängig dokumentierte Aspekte"""
            }
        ]
    },
    {
        "question": "Sind die vorgeschlagenen Messverfahren praktisch umsetzbar?",
        "type": "multiple_choice",
        "answers": [
            {
                "answer": "Ja",
                "correct": True,
                "feedback": "✓ Korrekt!"
            },
            {
                "answer": "Nein",
                "correct": False,
                "feedback": """× Nicht korrekt! - Die Methoden müssen mit verfügbaren Ressourcen durchführbar sein
                - Praktische Aspekte:
                Verfügbare Zeit und Personal,
                Technische Möglichkeiten (z.B. OCR, Textanalysetools),
                Aufwand-Nutzen-Verhältnis.
                - Problematisch wären:
                Zu zeitaufwendige manuelle Analysen,
                Technisch nicht realisierbare Messungen,
                Unverhältnismäßig komplexe Verfahren"""
            }
        ]
    }
]
display_quiz(questions, colors=colors.jupyterquiz)
```

#### Anwendung der Kriterien

Bei der Bewertung Ihrer Operationalisierung:

1. Prüfen Sie jeden Indikator einzeln gegen alle Kriterien
2. Identifizieren Sie mögliche Schwachstellen
3. Erwägen Sie Alternativen für problematische Aspekte
4. Dokumentieren Sie Ihre Überlegungen zu jedem Kriterium


````{admonition} Lösungen
:class: solution, dropdown
**Beispielhafte Anwendung**
Ein Indikator wie "Anzahl wissenschaftlicher Artikel pro Ausgabe":
- ✓ Quantifizierbar (zählbare Einheit)
- ✓ Basiert auf Quellenkorpus (nur Zeit-Artikel)
- ✓ Durchgängig messbar (über gesamten Zeitraum)
- ✓ Praktisch umsetzbar (mit klarer Definition und OCR)

**Hinweis**
Es gibt nicht die eine "richtige" Operationalisierung. Verschiedene Ansätze können geeignet sein, solange sie den grundlegenden Kriterien entsprechen und praktisch umsetzbar sind.
````
