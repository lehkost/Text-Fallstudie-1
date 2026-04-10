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
- Wählen Sie bei jeder Frage die Antwort(en) aus, die Sie für richtig halten.
- Lesen Sie das Feedback zu den einzelnen Antwortoptionen sorgfältig durch.
- Die Erklärungen helfen Ihnen dabei, Ihr Verständnis zu vertiefen – auch bei korrekten Antworten.

Es erfolgt keine Bewertung oder Speicherung Ihrer Ergebnisse. Nutzen Sie dieses Assessment, um Wissenslücken zu identifizieren und gegebenenfalls die entsprechenden Abschnitte des Kapitels noch einmal zu bearbeiten.

**Geschätzte Zeit**: 1h 15min

Viel Erfolg!
````

## Frage 1

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

"""
Lernziel: Sie verfügen über ein Grundverständnis des Konzepts des semantischen Feldes, können den Unterschied zwischen absoluten und relativen Häufigkeiten erklären und die Darstellungsmethoden des Liniendiagramms und der Key Word in Context (KWIC)-Anzeige interpretieren.
Bloom-Stufe: Verstehen, Analysieren
Format: Multiple Choice
"""


import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_1 = [{
    "question": """Was versteht man unter einem semantischen Feld im Kontext der Analyse der Spanischen Grippe?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Eine grafische Darstellung der Verbreitung einer Krankheit auf einer Landkarte",
            "correct": False,
            "feedback": """× Nicht korrekt. Diese Aussage beschreibt nicht ein semantisches Feld, sondern eher eine epidemiologische Karte. Ein semantisches Feld bezieht sich auf eine Gruppe von Wörtern mit verwandten Bedeutungen."""
        },
        {
            "answer": "Eine Sammlung von Wörtern, die mit der Spanischen Grippe im Zusammenhang stehen und diese spezifisch bezeichnen",
            "correct": True,
            "feedback": """✓ Richtig! Laut Text ist ein semantisches Feld eine "Sammlung dieser Wörter", die "mit der Spanischen Grippe im Zusammenhang" stehen. Diese Wörter sollten "sich auf die Spanische Grippe und nur auf diese beziehen"."""
        },
        {
            "answer": "Die Gesamtheit aller Zeitungsartikel zu einem bestimmten Thema",
            "correct": False,
            "feedback": """× Nicht korrekt. Diese Aussage beschreibt ein Korpus zu einem Thema, nicht ein semantisches Feld. Ein semantisches Feld besteht aus Wörtern mit verwandten Bedeutungen, nicht aus vollständigen Texten."""
        },
        {
            "answer": "Eine statistische Methode zur Berechnung der Häufigkeit von Krankheitsfällen",
            "correct": False,
            "feedback": """× Nicht korrekt. Diese Aussage beschreibt eine epidemiologische Analysemethode, nicht ein semantisches Feld. Ein semantisches Feld ist eine linguistische Kategorie, die bedeutungsverwandte Wörter zusammenfasst."""
        }
    ]
}]

display_quiz(multiple_choice_1, colors=colors.jupyterquiz)
```

## Frage 2

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_2 = [{
    "question": """Worin besteht der Unterschied zwischen absoluter und relativer Häufigkeit?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Absolute Häufigkeit bezieht sich auf die Anzahl der Erkrankten, relative Häufigkeit auf die Anzahl der Todesopfer",
            "correct": False,
            "feedback": """× Nicht korrekt. Diese Aussage bezieht sich auf epidemiologische Kennzahlen, nicht auf textanalytische Häufigkeitsmaße. Im Kontext der Textanalyse haben absolute und relative Häufigkeit andere Bedeutungen."""
        },
        {
            "answer": "Absolute Häufigkeit misst das Vorkommen in Qualitätszeitungen, relative Häufigkeit in allen verfügbaren Medien",
            "correct": False,
            "feedback": """× Nicht korrekt. Der Unterschied zwischen absoluter und relativer Häufigkeit bezieht sich nicht auf unterschiedliche Medientypen, sondern auf die Art der Berechnung."""
        },
        {
            "answer": "Absolute Häufigkeit ist die tatsächliche Anzahl des Vorkommens eines Wortes, relative Häufigkeit setzt diese ins Verhältnis zur Textlänge",
            "correct": True,
            "feedback": """✓ Richtig! Im Text wird erklärt: "Dafür wird die absolute Häufigkeit durch die Textlänge dividiert, daraus ergibt sich die relative Frequenz." Die relative Häufigkeit ermöglicht den Vergleich von Texten unterschiedlicher Länge."""
        },
        {
            "answer": "Absolute Häufigkeit bezieht sich auf ein einzelnes Wort, relative Häufigkeit auf ein ganzes semantisches Feld",
            "correct": False,
            "feedback": """× Nicht korrekt. Sowohl absolute als auch relative Häufigkeit können sich auf einzelne Wörter oder auf semantische Felder beziehen. Der Unterschied liegt in der Berechnungsmethode, nicht im betrachteten Objekt."""
        }
    ]
}]

display_quiz(multiple_choice_2, colors=colors.jupyterquiz)
```

## Frage 3

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_3 = [{
    "question": """Warum ist die Verwendung relativer Häufigkeiten bei der vergleichenden Analyse von Texten aus verschiedenen Zeitungen sinnvoll?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Weil verschiedene Zeitungen unterschiedliche Schreibstile verwenden",
            "correct": False,
            "feedback": """× Nicht korrekt. Unterschiedliche Schreibstile sind zwar ein wichtiger Aspekt bei der Textanalyse, erklären aber nicht, warum relative statt absolute Häufigkeiten verwendet werden sollten."""
        },
        {
            "answer": "Weil die Texte unterschiedlich lang sein können und die relative Häufigkeit diese Unterschiede ausgleicht",
            "correct": True,
            "feedback": """✓ Richtig! Der Text erklärt: "Wenn Texte verschieden lang sind, sollten die Häufigkeiten normalisiert werden, das heißt sie werden in Bezug zur Textlänge gesetzt." Dies ermöglicht einen faireren Vergleich zwischen Texten unterschiedlicher Länge."""
        },
        {
            "answer": "Weil absolute Häufigkeiten nur in Prozentangaben aussagekräftig sind",
            "correct": False,
            "feedback": """× Nicht korrekt. Absolute Häufigkeiten sind durchaus aussagekräftig, allerdings nicht für den Vergleich von Texten unterschiedlicher Länge. Prozentangaben sind eine Form der relativen Häufigkeit, nicht der absoluten."""
        },
        {
            "answer": "Weil verschiedene Zeitungen unterschiedliche Erscheinungszyklen haben",
            "correct": False,
            "feedback": """× Nicht korrekt. Der Erscheinungszyklus von Zeitungen hat keinen direkten Einfluss auf die Wahl zwischen absoluter und relativer Häufigkeit. Entscheidend ist vielmehr die Vergleichbarkeit der Textlängen."""
        }
    ]
}]

display_quiz(multiple_choice_3, colors=colors.jupyterquiz)
```

## Frage 4

Ein Text hat eine Länge von 500 Wörtern und enthält 15 Wörter aus dem semantischen Feld "Grippe". Ein zweiter Text hat eine Länge von 800 Wörtern und enthält 20 Wörter aus demselben semantischen Feld.

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_4 = [{
    "question": """Welche Aussage ist korrekt?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Der erste Text hat eine höhere absolute Häufigkeit von Grippewörtern",
            "correct": False,
            "feedback": """× Nicht korrekt. Der erste Text enthält 15 Grippewörter, der zweite 20 Grippewörter. Daher hat der zweite Text die höhere absolute Häufigkeit."""
        },
        {
            "answer": "Beide Texte haben dieselbe relative Häufigkeit von Grippewörtern",
            "correct": False,
            "feedback": """× Nicht korrekt. Die relative Häufigkeit des ersten Textes ist 15/500 = 0,03 (3%), die des zweiten Textes ist 20/800 = 0,025 (2,5%). Die relativen Häufigkeiten sind unterschiedlich."""
        },
        {
            "answer": "Der erste Text hat eine höhere relative Häufigkeit von Grippewörtern",
            "correct": True,
            "feedback": """✓ Richtig! Die relative Häufigkeit des ersten Textes beträgt 15/500 = 0,03 (3%), die des zweiten Textes 20/800 = 0,025 (2,5%). Obwohl der zweite Text mehr Grippewörter enthält (höhere absolute Häufigkeit), ist ihr Anteil am Gesamttext (relative Häufigkeit) geringer als im ersten Text."""
        },
        {
            "answer": "Aus den gegebenen Informationen kann keine Aussage über die Häufigkeiten getroffen werden",
            "correct": False,
            "feedback": """× Nicht korrekt. Die gegebenen Informationen (Textlänge und Anzahl der Grippewörter) sind ausreichend, um sowohl absolute als auch relative Häufigkeiten zu berechnen und zu vergleichen."""
        }
    ]
}]

display_quiz(multiple_choice_4, colors=colors.jupyterquiz)
```

## Frage 5
Betrachten Sie folgende drei Texte und ihre Häufigkeitswerte:

- Text A: 30 Grippewörter bei 600 Wörtern Gesamtlänge
- Text B: 25 Grippewörter bei 400 Wörtern Gesamtlänge
- Text C: 20 Grippewörter bei 500 Wörtern Gesamtlänge

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_6 = [{
    "question": """Was ist die korrekte relative Häufigkeit der Grippewörter, wenn alle drei Texte zusammen betrachtet werden?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "0,05083 (5,083%)",
            "correct": False,
            "feedback": """× Nicht korrekt. Dieser Wert entspricht dem Durchschnitt der relativen Häufigkeiten (0,05 + 0,0625 + 0,04)/3 = 0,05083. Der Text erklärt jedoch, warum diese Berechnungsmethode problematisch sein kann."""
        },
        {
            "answer": "0,075 (7,5%)",
            "correct": False,
            "feedback": """× Nicht korrekt. Die korrekte Berechnung ist: Summe aller Grippewörter geteilt durch Summe aller Wörter: (30+25+20)/(600+400+500) = 75/1500 = 0,05 (5%)."""
        },
        {
            "answer": "0,0625 (6,25%)",
            "correct": False,
            "feedback": """× Nicht korrekt. Dieser Wert entspricht der relativen Häufigkeit von Text B (25/400 = 0,0625), nicht der Gesamthäufigkeit aller drei Texte."""
        },
        {
            "answer": "0,05 (5%)",
            "correct": True,
            "feedback": """✓ Richtig! Die korrekte Berechnung der relativen Häufigkeit für mehrere Texte addiert alle absoluten Häufigkeiten und teilt sie durch die Summe aller Textlängen: (30+25+20)/(600+400+500) = 75/1500 = 0,05 (5%). Wie im Text erläutert, ist diese Methode besser als die Berechnung des Durchschnitts der relativen Häufigkeiten."""
        }
    ]
}]

display_quiz(multiple_choice_6, colors=colors.jupyterquiz)
```

## Frage 6

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_7 = [{
    "question": """Warum eignet sich ein Liniendiagramm besonders gut zur Darstellung der Häufigkeitsverläufe der Grippewörter über die Zeit?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Es zeigt kontinuierliche Verläufe und macht lokale und globale Extremwerte leicht erkennbar",
            "correct": True,
            "feedback": """✓ Richtig! Im Text wird erklärt: "Liniendiagramme eignen sich gut, um zeitliche Verläufe darzustellen, da lokale und globale Minima und Maxima leicht erkennbar sind und sie die Kontinuität der Daten unterstreichen." """
        },
        {
            "answer": "Es ermöglicht die gleichzeitige Darstellung von absoluten und relativen Häufigkeiten",
            "correct": False,
            "feedback": """× Nicht korrekt. Ein Liniendiagramm kann entweder absolute oder relative Häufigkeiten darstellen, nicht jedoch beide gleichzeitig auf derselben Skala, da sie unterschiedliche Maßeinheiten haben."""
        },
        {
            "answer": "Es ist die einzige Darstellungsform, die für Zeitreihenanalysen geeignet ist",
            "correct": False,
            "feedback": """× Nicht korrekt. Es gibt auch andere Darstellungsformen für Zeitreihenanalysen, wie z.B. Balkendiagramme. Der Text erwähnt: "Die Häufigkeiten über Zeit ließen sich auch in einem Balkendiagramm darstellen." """
        },
        {
            "answer": "Es verbindet automatisch qualitative und quantitative Analyse",
            "correct": False,
            "feedback": """× Nicht korrekt. Ein Liniendiagramm ist ein rein quantitatives Analysewerkzeug. Die Verbindung zur qualitativen Analyse wird eher durch die KWIC-Darstellung hergestellt, nicht durch das Liniendiagramm."""
        }
    ]
}]

display_quiz(multiple_choice_7, colors=colors.jupyterquiz)
```

## Frage 7

Analysieren Sie das folgende Szenario:

Ein Forschungsteam untersucht die mediale Berichterstattung über COVID-19 in verschiedenen deutschen Zeitungen im Jahr 2020. Sie haben ein semantisches Feld mit Begriffen wie "Coronavirus", "COVID-19", "Pandemie", "Lockdown" usw. erstellt.

1. Beschreiben Sie, wie Sie die relative Häufigkeit dieser Begriffe für einen monatlichen Vergleich berechnen würden.
2. Erläutern Sie, warum relative statt absolute Häufigkeiten für den Vergleich verschiedener Zeitungen wichtig sind.
3. Erklären Sie, wie Sie die KWIC-Darstellung nutzen könnten, um das semantische Feld zu verfeinern.
4. Diskutieren Sie, welche Einsichten ein Liniendiagramm der relativen Häufigkeiten über die Zeit liefern könnte.

```{code-cell} ipython3
:tags: [remove-input]
import sys
sys.path.append("../quadriga")  # Adjust path as needed
from assessment import create_answer_box

create_answer_box('semantic-field')
```

````{admonition} Lösung
:class: solution, dropdown
**Beispiellösung zur Selbstbewertung:**

**1. Berechnung der relativen Häufigkeit für monatlichen Vergleich:**
- Für jeden Monat alle Artikel der jeweiligen Zeitung zusammenfassen
- Absolute Häufigkeit: Zählen aller Vorkommen von Wörtern aus dem semantischen Feld "COVID-19" in den Artikeln des Monats
- Gesamtwortzahl: Zählen aller Wörter in den Artikeln des Monats
- Relative Häufigkeit = Absolute Häufigkeit / Gesamtwortzahl
- Alternativ könnte man auch die Summe der absoluten Häufigkeiten durch die Summe der Textlängen teilen

**2. Bedeutung relativer Häufigkeiten für den Zeitungsvergleich:**
- Zeitungen haben unterschiedliche Formate, Umfänge und Erscheinungsweisen
- Absolute Häufigkeiten wären stark von den Gesamttextlängen abhängig
- Relative Häufigkeiten ermöglichen fairen Vergleich unabhängig von Textlänge
- Beispiel: Eine Zeitung mit 50 COVID-Begriffen in 1000 Wörtern (5%) vs. eine Zeitung mit 100 COVID-Begriffen in 4000 Wörtern (2,5%)

**3. Nutzung der KWIC-Darstellung zur Verfeinerung des semantischen Feldes:**
- Analyse des Kontexts einzelner Begriffe, um deren tatsächliche Verwendung zu prüfen
- Identifikation mehrdeutiger Begriffe (z.B. "Corona" könnte sich auch auf das Bier beziehen)
- Entdeckung weiterer relevanter Begriffe im Kontext der vorhandenen Suchbegriffe
- Überprüfung, ob Begriffe tatsächlich im Zusammenhang mit COVID-19 verwendet werden
- Iterative Anpassung des semantischen Feldes: Entfernen irrelevanter und Hinzufügen neuer Begriffe

**4. Einsichten aus einem Liniendiagramm der relativen Häufigkeiten:**
- Visualisierung des zeitlichen Verlaufs der medialen Aufmerksamkeit für COVID-19
- Identifikation von Höhepunkten der Berichterstattung und Korrelation mit wichtigen Ereignissen
- Vergleich zwischen "Wellen" der Pandemie und "Wellen" der Berichterstattung
- Erkennen von Trends wie Ermüdungserscheinungen in der Berichterstattung
- Unterschiede zwischen verschiedenen Zeitungen im zeitlichen Verlauf ihrer Berichterstattung
````


## Frage 8
(Wählen Sie alle zutreffenden Antworten aus)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

"""
Lernziel: Sie können die notwendigen Schritte zur Frequenzanalyse eines semantischen Felds aufzählen, Unterschiede in der Berechnung der Häufigkeiten benennen und die Ergebnisse reflektieren.
Bloom-Stufe: Verstehen, Analysieren
Format: Multiple Choice
"""


import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_1 = [{
    "question": """Welche Schritte sind für die Frequenzanalyse eines semantischen Feldes in historischen Texten notwendig?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Einlesen des Korpus und der Metadaten",
            "correct": True,
            "feedback": """✓ Richtig! Im Notebook werden zunächst die annotierten CSV-Dateien und die zugehörigen Metadaten eingelesen. Dies ist ein essentieller erster Schritt, um auf die Textdaten und deren zeitliche Einordnung zugreifen zu können."""
        },
        {
            "answer": "Einlesen der definierten Wortliste (semantisches Feld)",
            "correct": True,
            "feedback": """✓ Richtig! Im Notebook wird explizit eine Wortliste für das semantische Feld "Grippe" eingelesen, die die Suchbegriffe für die Frequenzanalyse enthält."""
        },
        {
            "answer": "Manuelle Annotation aller Texte nach relevanten Begriffen",
            "correct": False,
            "feedback": """× Nicht korrekt. Die Texte wurden bereits zuvor annotiert (tokenisiert und lemmatisiert) und liegen als CSV-Dateien vor. Eine manuelle Annotation ist nicht Teil des Prozesses, der im Notebook beschrieben wird."""
        },
        {
            "answer": "Berechnung der Häufigkeiten der Begriffe über verschiedene Zeiträume",
            "correct": True,
            "feedback": """✓ Richtig! Im Notebook werden die Häufigkeiten der Begriffe aus dem semantischen Feld berechnet und nach verschiedenen Zeiträumen (Tag, Woche, Monat) gruppiert."""
        },
        {
            "answer": "Visualisierung der Ergebnisse in einem diachronen Diagramm",
            "correct": True,
            "feedback": """✓ Richtig! Die berechneten Häufigkeiten werden in einem interaktiven Liniendiagramm dargestellt, das den zeitlichen Verlauf (diachron) der Wortfrequenzen visualisiert."""
        }
    ]
}]

display_quiz(multiple_choice_1, colors=colors.jupyterquiz)
```

## Frage 9
(Wählen Sie alle zutreffenden Antworten aus)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_2 = [{
    "question": """Welche Arten von Frequenzberechnungen werden im Notebook für die Analyse verwendet?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Absolute Häufigkeiten pro Zeiteinheit",
            "correct": True,
            "feedback": """✓ Richtig! Im Notebook werden absolute Häufigkeiten berechnet, die die tatsächliche Anzahl der Vorkommen der Suchbegriffe pro Zeiteinheit darstellen."""
        },
        {
            "answer": "Relative Häufigkeiten pro Zeiteinheit",
            "correct": True,
            "feedback": """✓ Richtig! Im Notebook werden auch relative Häufigkeiten berechnet, indem die absoluten Häufigkeiten durch die Gesamtzahl der Wörter in den jeweiligen Zeitabschnitten geteilt werden."""
        },
        {
            "answer": "Syntaktische Häufigkeiten",
            "correct": False,
            "feedback": """× Nicht korrekt. Diese Art der Häufigkeitsberechnung wird im Notebook nicht erwähnt oder verwendet. Die Analyse konzentriert sich auf absolute und relative Worthäufigkeiten, nicht auf syntaktische Strukturen."""
        },
        {
            "answer": "Kookkurrenzhäufigkeiten",
            "correct": False,
            "feedback": """× Nicht korrekt. Diese Art der Häufigkeitsberechnung wird im Notebook nicht erwähnt oder verwendet. Es werden keine Kookkurrenzen (gemeinsames Auftreten von Wörtern) analysiert, sondern nur das Vorkommen einzelner Wörter aus dem semantischen Feld."""
        }
    ]
}]

display_quiz(multiple_choice_2, colors=colors.jupyterquiz)
```

## Frage 10

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_3 = [{
    "question": """Warum ist die Unterscheidung zwischen absoluten und relativen Häufigkeiten bei der diachronen Analyse wichtig?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Absolute Häufigkeiten sind präziser und sollten daher immer bevorzugt werden",
            "correct": False,
            "feedback": """× Nicht korrekt. Absolute Häufigkeiten geben zwar die tatsächliche Anzahl der Vorkommen an, können aber bei unterschiedlichen Textlängen pro Zeitabschnitt zu verzerrten Ergebnissen führen."""
        },
        {
            "answer": "Relative Häufigkeiten berücksichtigen unterschiedliche Textlängen in verschiedenen Zeitabschnitten",
            "correct": True,
            "feedback": """✓ Richtig! Relative Häufigkeiten setzen die Anzahl der Vorkommen ins Verhältnis zur Gesamttextlänge und ermöglichen dadurch einen faireren Vergleich zwischen Zeitabschnitten mit unterschiedlich vielen Texten oder unterschiedlichen Textlängen."""
        },
        {
            "answer": "Absolute Häufigkeiten sind nur für die tägliche Analyse relevant, relative Häufigkeiten nur für die monatliche",
            "correct": False,
            "feedback": """× Nicht korrekt. Sowohl absolute als auch relative Häufigkeiten können für alle zeitlichen Granularitäten (Tag, Woche, Monat) relevant sein, abhängig vom Analyseziel und der Beschaffenheit der Daten."""
        },
        {
            "answer": "Die Unterscheidung ist nur wichtig, wenn unterschiedliche Zeitungen verglichen werden",
            "correct": False,
            "feedback": """× Nicht korrekt. Diese Aussage ist zu eingeschränkt. Die Unterscheidung zwischen absoluten und relativen Häufigkeiten ist bei jeder Art von diachroner Analyse wichtig, bei der die Textlängen und die Textanzahl über die Zeit variiert, nicht nur beim Vergleich verschiedener Zeitungen."""
        }
    ]
}]

display_quiz(multiple_choice_3, colors=colors.jupyterquiz)
```

## Frage 11

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_4 = [{
    "question": """Welche Beobachtung lässt sich aus dem im Notebook erstellten diachronen Frequenzdiagramm der Grippe-Begriffe ableiten?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Die Häufigkeit der Grippe-Begriffe blieb über das gesamte Jahr 1918 konstant",
            "correct": False,
            "feedback": """× Nicht korrekt. Diese Aussage widerspricht der Diskussion im Notebook, die von "zwei Wellen der Erwähnungen des Wortes 'Grippe'" spricht, was auf eine Veränderung und nicht auf Konstanz hindeutet."""
        },
        {
            "answer": "Es zeigen sich zwei deutliche Wellen in der Häufigkeit der Grippe-Begriffe, die mit historischen Daten korrelieren",
            "correct": True,
            "feedback": """✓ Richtig! In der Diskussion im Notebook wird explizit erwähnt: "Unsere zwei Wellen der Erwähnungen des Wortes 'Grippe' scheinen den Sterblichkeitszahlen zu entsprechen", was auf eine Korrelation mit historischen Daten hindeutet."""
        },
        {
            "answer": "Die dritte Welle der Spanischen Grippe spiegelt sich deutlich in den Wortfrequenzen wider",
            "correct": False,
            "feedback": """× Nicht korrekt. Diese Aussage widerspricht der Diskussion im Notebook, die explizit erwähnt: "Die dritte Welle scheint nicht reproduziert zu werden, was eine weitere Untersuchung erfordert." """
        },
        {
            "answer": "Die Frequenzanalyse ergibt keine erkennbaren Muster im Zusammenhang mit der Spanischen Grippe",
            "correct": False,
            "feedback": """× Nicht korrekt. Diese Aussage widerspricht der Diskussion im Notebook, die deutliche Muster erkennt und diese mit historischen Daten in Verbindung bringt."""
        }
    ]
}]

display_quiz(multiple_choice_4, colors=colors.jupyterquiz)
```

## Frage 12

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_5 = [{
    "question": """Welche Hypothese wird im Notebook für das Fehlen einer dritten Welle in der Frequenzanalyse angeführt?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Die dritte Welle der Spanischen Grippe fand außerhalb des untersuchten Zeitraums statt",
            "correct": False,
            "feedback": """× Nicht korrekt. Diese Hypothese wird im Notebook nicht angeführt. Im Gegenteil, es wird davon ausgegangen, dass die dritte Welle Anfang 1919 stattfand, was im untersuchten Zeitraum liegt."""
        },
        {
            "answer": "Nach dem Verlust des Krieges und der Revolution waren Grippetodesfälle kein relevantes Nachrichtenthema mehr",
            "correct": True,
            "feedback": """✓ Richtig! Im Notebook wird folgende Hypothese angeführt: "Dies könnte besonders für Anfang 1919 zutreffen, als nach dem Verlust des Krieges und der Revolution von 1918 Grippetodesfälle kein Nachrichtenthema mehr waren." """
        },
        {
            "answer": "Die dritte Welle betraf hauptsächlich ländliche Gebiete und nicht Berlin",
            "correct": False,
            "feedback": """× Nicht korrekt. Diese Hypothese wird im Notebook nicht angeführt. Es gibt keinen Hinweis darauf, dass die dritte Welle geografisch anders verteilt war als die ersten beiden."""
        },
        {
            "answer": "Das semantische Feld wurde nicht korrekt definiert, um die dritte Welle zu erfassen",
            "correct": False,
            "feedback": """× Nicht korrekt. Diese Hypothese wird im Notebook nicht direkt angeführt. Es wird nicht in Frage gestellt, ob das semantische Feld für die Erfassung der dritten Welle geeignet war."""
        }
    ]
}]

display_quiz(multiple_choice_5, colors=colors.jupyterquiz)
```

## Frage 13

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_6 = [{
    "question": """Welche Zeiteinheiten werden im Notebook für die Aggregation der Frequenzdaten angeboten?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Tage, Wochen und Monate",
            "correct": True,
            "feedback": """✓ Richtig! Im Notebook werden drei Zeiteinheiten für die Analyse verwendet: "frequency_parameters = ["M", "W-MON", "D"]", was für Monate, Wochen (beginnend am Montag) und Tage steht."""
        },
        {
            "answer": "Stunden, Tage und Wochen",
            "correct": False,
            "feedback": """× Nicht korrekt. Diese Kombination ist nicht korrekt. Das Notebook verwendet Tage, Wochen und Monate, nicht Stunden."""
        },
        {
            "answer": "Wochen, Monate und Quartale",
            "correct": False,
            "feedback": """× Nicht korrekt. Diese Kombination ist nicht korrekt. Das Notebook verwendet Tage, Wochen und Monate, nicht Quartale."""
        },
        {
            "answer": "Nur Monate, da kleinere Zeiteinheiten zu viel Rauschen enthalten",
            "correct": False,
            "feedback": """× Nicht korrekt. Das Notebook bietet drei verschiedene Zeiteinheiten an (Tage, Wochen und Monate), und Benutzer:innen können zwischen ihnen wählen."""
        }
    ]
}]

display_quiz(multiple_choice_6, colors=colors.jupyterquiz)
```

## Frage 14

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_7 = [{
    "question": """Welche Schritte werden im Notebook durchgeführt, um die Daten für die Frequenzanalyse vorzubereiten?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Hinzufügen von Datumsinformationen zu den Annotationen",
            "correct": True,
            "feedback": """✓ Richtig! Im Notebook wird die Funktion add_date_to_corpus_annotations verwendet, um Datumsinformationen aus den Metadaten zu den annotierten Texten hinzuzufügen."""
        },
        {
            "answer": "Zusammenführen aller annotierten Texte in eine gemeinsame Datenstruktur",
            "correct": True,
            "feedback": """✓ Richtig! Im Notebook werden alle annotierten Texte mit pd.concat(corpus_annotations.values()) in einen gemeinsamen DataFrame zusammengeführt."""
        },
        {
            "answer": "Lemmatisierung der Texte während der Analyse",
            "correct": False,
            "feedback": """× Nicht korrekt. Diese Aussage ist nicht korrekt. Die Lemmatisierung wurde bereits in einem früheren Schritt durchgeführt, und die Texte liegen bereits als lemmatisierte CSV-Dateien vor."""
        },
        {
            "answer": "Manuelle Klassifikation der Texte nach Relevanz",
            "correct": False,
            "feedback": """× Nicht korrekt. Diese Aussage ist nicht korrekt. Es findet keine manuelle Klassifikation der Texte während der Analyse statt."""
        }
    ]
}]

display_quiz(multiple_choice_7, colors=colors.jupyterquiz)
```

## Frage 15

Analysieren Sie folgendes Szenario:

Sie planen eine diachrone Frequenzanalyse zu Berichten über eine historische Naturkatastrophe in deutschen Zeitungen. Sie haben bereits ein Korpus mit annotierten Texten und Metadaten sowie ein semantisches Feld mit relevanten Begriffen erstellt.

1. Beschreiben Sie die notwendigen Schritte zur Durchführung der Frequenzanalyse.
2. Erläutern Sie, wann und warum Sie absolute bzw. relative Häufigkeiten verwenden würden.
3. Welche Zeiteinheiten würden Sie für die Aggregation wählen und warum?
4. Wie würden Sie die Ergebnisse visualisieren und interpretieren?

```{code-cell} ipython3
:tags: [remove-input]
import sys
sys.path.append("../quadriga")  # Adjust path as needed
from assessment import create_answer_box

create_answer_box('frequency-analysis')
```

````{admonition} Lösung
:class: solution, dropdown
**Beispiellösung zur Selbstbewertung:**

**1. Notwendige Schritte zur Frequenzanalyse:**
- Einlesen des annotierten Korpus (CSV-Dateien mit Token und Lemmata)
- Einlesen der Metadaten mit Datumsinformationen
- Einlesen des semantischen Feldes zur Naturkatastrophe
- Zusammenführen der Datumsinformationen mit den Annotationen
- Zusammenführen aller Texte in eine gemeinsame Datenstruktur
- Filterung der Lemmata nach dem semantischen Feld
- Gruppierung der Vorkommen nach Zeiteinheiten
- Berechnung der absoluten und relativen Häufigkeiten
- Visualisierung der Ergebnisse in einem Liniendiagramm

**2. Verwendung von absoluten vs. relativen Häufigkeiten:**
- Absolute Häufigkeiten können verwendet werden, wenn die tatsächlichen Anzahl der Erwähnungen von Interesse ist, z.B. um die reine Medienpräsenz zu quantifizieren
- Relative Häufigkeiten können für den Vergleich zwischen Zeitabschnitten mit unterschiedlicher Textmenge verwendet werden
- Bei der Analyse über einen längeren Zeitraum mit schwankender Verfügbarkeit von Zeitungsausgaben sind relative Häufigkeiten unverzichtbar
- Idealerweise werden beide Werte berechnet, da dies die Möglichkeit bietet, zwischen beiden Darstellungen zu wechseln

**3. Wahl der Zeiteinheiten:**
- Tägliche Aggregation: für detaillierte Analysen, besonders bei plötzlichen Ereignissen wie Naturkatastrophen
- Wöchentliche Aggregation: für mittelfristige Trends, reduziert tägliche Schwankungen
- Monatliche Aggregation: für langfristige Trends über mehrere Jahre
- Bei einer Naturkatastrophe könnten alle drei Ebenen angeboten werden, aber der Fokus sollte auf der täglichen und wöchentlichen Aggregation legen, da die mediale Aufmerksamkeit für solche Ereignisse typischerweise schnell ansteigt und dann allmählich abnimmt

**4. Visualisierung und Interpretation:**
- Interaktives Liniendiagramm mit der Möglichkeit, zwischen Zeiteinheiten und absoluten/relativen Häufigkeiten zu wechseln
- Markierung wichtiger Ereignisse im Zusammenhang mit der Katastrophe im Diagramm
- Vergleich der medialen Aufmerksamkeitskurve mit Daten zur tatsächlichen Intensität der Katastrophe
- Interpretation potenzieller Diskrepanzen zwischen medialer Aufmerksamkeit und tatsächlichem Geschehen
- Analyse von Faktoren, die die mediale Aufmerksamkeit beeinflussen könnten (andere wichtige Ereignisse, politische Situation, etc.)
- Bei Naturkatastrophen wird ein schneller Anstieg der Berichterstattung unmittelbar nach dem Ereignis erwartet und dann ein allmählicher Rückgang, möglicherweise mit kleineren Spitzen bei Folgeberichten oder Jahrestagen
````


## Frage 16

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

"""
Lernziel: Sie können die Darstellungsmethode Keywords in Context beschreiben, Wörter zur Anzeige auswählen und diese anzeigen lassen.
Format: Multiple Choice
"""


import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_1 = [{
    "question": """Was ist der Hauptzweck der KWIC-Darstellung (Keyword in Context) in der Textanalyse?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Die automatische Lemmatisierung von Texten",
            "correct": False,
            "feedback": """× Nicht korrekt. Die KWIC-Darstellung dient nicht der Lemmatisierung von Texten. Die Lemmatisierung ist ein separater Vorverarbeitungsschritt, der bereits vor der KWIC-Analyse durchgeführt wird."""
        },
        {
            "answer": "Die Anzeige von Suchbegriffen mit ihrem unmittelbaren textuellen Kontext",
            "correct": True,
            "feedback": """✓ Richtig! Die KWIC-Darstellung zeigt Suchbegriffe zusammen mit ihrem unmittelbaren Kontext an, typischerweise in einer dreispaltigen Tabelle mit dem Kontext vor dem Suchbegriff, dem Suchbegriff selbst und dem Kontext nach dem Suchbegriff."""
        },
        {
            "answer": "Die statistische Berechnung von Wortfrequenzen",
            "correct": False,
            "feedback": """× Nicht korrekt. Die KWIC-Darstellung berechnet keine statistischen Werte wie Wortfrequenzen. Sie dient vielmehr der kontextuellen Einbettung von bereits identifizierten Suchbegriffen."""
        },
        {
            "answer": "Die grafische Visualisierung von Wortfrequenzen über Zeit",
            "correct": False,
            "feedback": """× Nicht korrekt. Die KWIC-Darstellung ist keine grafische Visualisierung von Frequenzen über Zeit. Für diesen Zweck werden typischerweise Linien- oder Balkendiagramme verwendet, wie im vorherigen Abschnitt zur diachronen Analyse gezeigt."""
        }
    ]
}]

display_quiz(multiple_choice_1, colors=colors.jupyterquiz)
```

## Frage 17

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_2 = [{
    "question": """Welche Informationen werden typischerweise in einer KWIC-Darstellung angezeigt?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Nur das Suchwort und seine Häufigkeit",
            "correct": False,
            "feedback": """× Nicht korrekt. Die KWIC-Darstellung zeigt mehr als nur das Suchwort und seine Häufigkeit. Sie stellt den Suchbegriff in seinem textuellen Kontext dar."""
        },
        {
            "answer": "Das Suchwort, seine Lemmatisierung und seine Wortart",
            "correct": False,
            "feedback": """× Nicht korrekt. Obwohl das Suchwort angezeigt wird, fokussiert sich die KWIC-Darstellung nicht primär auf linguistische Eigenschaften wie Lemmatisierung oder Wortart, sondern auf den textuellen Kontext."""
        },
        {
            "answer": "Der linke Kontext, das Suchwort und der rechte Kontext sowie zusätzliche Metadaten",
            "correct": True,
            "feedback": """✓ Richtig! Die KWIC-Darstellung besteht typischerweise aus drei Hauptspalten: dem Kontext vor dem Suchwort (linker Kontext), dem Suchwort selbst und dem Kontext nach dem Suchwort (rechter Kontext). Zusätzlich können Metadaten wie Datum oder Quelle angezeigt werden."""
        },
        {
            "answer": "Eine statistische Zusammenfassung aller Vorkommen des Suchwortes",
            "correct": False,
            "feedback": """× Nicht korrekt. Die KWIC-Darstellung bietet keine statistische Zusammenfassung, sondern zeigt jedes einzelne Vorkommen des Suchwortes in seinem Kontext."""
        }
    ]
}]

display_quiz(multiple_choice_2, colors=colors.jupyterquiz)
```

## Frage 18

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_3 = [{
    "question": """Welcher Schritt muss vor der Erstellung einer KWIC-Darstellung durchgeführt werden?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Einlesen und Vorbereiten des Korpus und der Metadaten",
            "correct": True,
            "feedback": """✓ Richtig! Wie im Notebook gezeigt, müssen zunächst das Korpus und die Metadaten eingelesen und vorbereitet werden, bevor eine KWIC-Suche durchgeführt werden kann."""
        },
        {
            "answer": "Manuelle Annotation aller Texte",
            "correct": False,
            "feedback": """× Nicht korrekt. Eine manuelle Annotation ist nicht zwingend erforderlich. Im Notebook wurden bereits annotierte Texte verwendet, die aus früheren Verarbeitungsschritten stammen."""
        },
        {
            "answer": "Grafische Darstellung der Wortfrequenzen",
            "correct": False,
            "feedback": """× Nicht korrekt. Die grafische Darstellung von Wortfrequenzen ist kein notwendiger Vorbereitungsschritt für eine KWIC-Darstellung. Diese beiden Analysemethoden können unabhängig voneinander durchgeführt werden."""
        },
        {
            "answer": "Statistische Berechnung der Signifikanz aller Wörter",
            "correct": False,
            "feedback": """× Nicht korrekt. Eine statistische Signifikanzberechnung ist kein notwendiger Schritt vor der KWIC-Darstellung. Die KWIC-Methode zeigt alle Vorkommen eines Suchbegriffs an, unabhängig von ihrer statistischen Signifikanz."""
        }
    ]
}]

display_quiz(multiple_choice_3, colors=colors.jupyterquiz)
```

## Frage 19

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_4 = [{
    "question": """Welche Funktion erfüllt der Parameter n_words in der KWIC-Darstellung im Notebook?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Er gibt die maximale Anzahl der anzuzeigenden Suchwörter an",
            "correct": False,
            "feedback": """× Nicht korrekt. Der Parameter n_words bezieht sich nicht auf die Anzahl der Suchwörter, sondern auf den Umfang des Kontexts."""
        },
        {
            "answer": "Er definiert die minimale Frequenz, die ein Wort haben muss, um angezeigt zu werden",
            "correct": False,
            "feedback": """× Nicht korrekt. Der Parameter n_words bezieht sich nicht auf Frequenzen, sondern auf den Umfang des Kontexts."""
        },
        {
            "answer": "Er bestimmt die Anzahl der Wörter, die links und rechts vom Suchwort angezeigt werden",
            "correct": True,
            "feedback": """✓ Richtig! Im Notebook wird der Parameter n_words=5 verwendet, um festzulegen, dass jeweils 5 Wörter vor und nach dem Suchwort als Kontext angezeigt werden sollen."""
        },
        {
            "answer": "Er gibt die Gesamtzahl der anzuzeigenden KWIC-Ergebnisse an",
            "correct": False,
            "feedback": """× Nicht korrekt. Der Parameter n_words bezieht sich nicht auf die Anzahl der Ergebnisse, sondern auf den Umfang des Kontexts pro Ergebnis."""
        }
    ]
}]

display_quiz(multiple_choice_4, colors=colors.jupyterquiz)
```

## Frage 20

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_5 = [{
    "question": """Warum ist die KWIC-Darstellung eine sinnvolle Ergänzung zur quantitativen Frequenzanalyse?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Sie ist schneller durchzuführen als die Frequenzanalyse",
            "correct": False,
            "feedback": """× Nicht korrekt. Die Geschwindigkeit ist kein Vorteil der KWIC-Darstellung gegenüber der Frequenzanalyse. Beide Methoden ergänzen sich in ihren analytischen Möglichkeiten."""
        },
        {
            "answer": "Sie erlaubt einen Einblick in den tatsächlichen Gebrauch der Suchwörter im Kontext",
            "correct": True,
            "feedback": """✓ Richtig! Während die Frequenzanalyse quantitative Daten liefert, ermöglicht die KWIC-Darstellung einen qualitativen Einblick in den tatsächlichen Gebrauch der Suchwörter in ihrem Kontext, was für die Interpretation der Daten sehr wertvoll ist."""
        },
        {
            "answer": "Sie ist genauer als die Frequenzanalyse",
            "correct": False,
            "feedback": """× Nicht korrekt. Es geht nicht um Genauigkeit, sondern um unterschiedliche Perspektiven. Die KWIC-Darstellung und die Frequenzanalyse bieten unterschiedliche, sich ergänzende Ansätze."""
        },
        {
            "answer": "Sie kann ohne vorherige Annotation der Texte durchgeführt werden",
            "correct": False,
            "feedback": """× Nicht korrekt. Auch die KWIC-Darstellung profitiert von annotierten Texten, wie im Notebook gezeigt wurde, wo auf tokenisierte und lemmatisierte Texte zugegriffen wird."""
        }
    ]
}]

display_quiz(multiple_choice_5, colors=colors.jupyterquiz)
```

## Frage 21

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_6 = [{
    "question": """Welche Aussage zur Auswahl von Suchwörtern für die KWIC-Darstellung ist korrekt?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Es sollten immer nur einzelne Wörter und keine Wortgruppen gesucht werden",
            "correct": False,
            "feedback": """× Nicht korrekt. Je nach Forschungsfrage können sowohl einzelne Wörter als auch Wortgruppen oder Phrasen für die KWIC-Suche relevant sein."""
        },
        {
            "answer": "Die Suchwörter müssen immer aus dem vordefinierten semantischen Feld stammen",
            "correct": False,
            "feedback": """× Nicht korrekt. Obwohl im Beispiel ein semantisches Feld verwendet wird, ist dies keine zwingende Voraussetzung. Die Suchwörter können frei nach Forschungsinteresse gewählt werden."""
        },
        {
            "answer": "Die Suchwörter können einzeln oder als Liste übergeben werden, wie am Beispiel von word_list gezeigt",
            "correct": True,
            "feedback": """✓ Richtig! Im Notebook wird gezeigt, wie die gesamte Wortliste des semantischen Feldes "Grippe" als Parameter für die KWIC-Suche übergeben wird, aber es könnten auch einzelne Wörter oder andere Wortlisten verwendet werden."""
        },
        {
            "answer": "Die Suchwörter müssen vorher auf ihre statistische Signifikanz geprüft werden",
            "correct": False,
            "feedback": """× Nicht korrekt. Eine statistische Signifikanzprüfung ist keine Voraussetzung für die Auswahl von Suchwörtern für die KWIC-Darstellung. Die Auswahl richtet sich nach dem Forschungsinteresse."""
        }
    ]
}]

display_quiz(multiple_choice_6, colors=colors.jupyterquiz)
```

## Frage 22

Stellen Sie sich vor, Sie möchten eine KWIC-Analyse zum Thema "Schutzmaßnahmen gegen die Spanische Grippe" durchführen.

1. Welche spezifischen Wörter würden Sie für Ihre KWIC-Suche auswählen und warum?
2. Welchen Kontextumfang (Anzahl der Wörter links und rechts vom Suchwort) würden Sie wählen und warum?
3. Beschreiben Sie, wie Sie die KWIC-Ergebnisse nutzen würden, um Ihr Verständnis des Themas zu vertiefen.
4. Wie würden Sie die KWIC-Analyse mit der quantitativen Frequenzanalyse kombinieren?

```{code-cell} ipython3
:tags: [remove-input]
import sys
sys.path.append("../quadriga")  # Adjust path as needed
from assessment import create_answer_box

create_answer_box('kwic-analysis')
```

````{admonition} Lösung
:class: solution, dropdown
**Beispiellösung zur Selbstbewertung:**

**1. Auswahl der Suchwörter:**
- Ich würde folgende Wörter wählen: "Schutzmaske", "Desinfektion", "Quarantäne", "Isolierung", "Schutzmaßnahme", "Seuchenschutz"
- Diese Wörter beziehen sich direkt auf Schutzmaßnahmen gegen die Spanische Grippe
- Ich würde auch verwandte Begriffe wie "Schließung" (von Schulen, öffentlichen Einrichtungen) und "Verbot" (von Versammlungen) hinzufügen
- Die Auswahl basiert auf dem im Notebook gezeigten semantischen Feld und wurde um weitere schutzmaßnahmenbezogene Begriffe ergänzt

**2. Wahl des Kontextumfangs:**
- Ich würde einen Kontextumfang von 7-10 Wörtern wählen
- Dies bietet mehr Kontext als die 5 Wörter im Beispiel, was bei komplexeren Themen wie Schutzmaßnahmen hilfreich sein kann
- Ein größerer Kontext ermöglicht es, nicht nur die unmittelbare Umgebung des Suchbegriffs zu sehen, sondern auch breitere syntaktische und semantische Zusammenhänge zu erfassen
- Bei zu großem Kontext könnte die Übersichtlichkeit leiden, daher ist eine Begrenzung auf 7-10 Wörter sinnvoll

**3. Nutzung der KWIC-Ergebnisse:**
- Identifikation der konkreten Schutzmaßnahmen, die während der Pandemie ergriffen wurden
- Analyse der Bewertung dieser Maßnahmen (positiv, negativ, neutral) im Kontext
- Untersuchung, ob bestimmte Maßnahmen mit bestimmten Akteuren (Behörden, Ärzte, Bürger) assoziiert werden
- Erkennung von zeitlichen Mustern: Wann wurden welche Maßnahmen thematisiert?
- Vergleich der Darstellung verschiedener Maßnahmen in unterschiedlichen Zeitungen

**4. Kombination mit quantitativer Frequenzanalyse:**
- Zunächst Identifikation von zeitlichen Mustern durch Frequenzanalyse (wann wurden Schutzmaßnahmen besonders häufig thematisiert?)
- Gezielte KWIC-Analyse für diese Zeiträume, um qualitative Einblicke zu gewinnen
- Überprüfung, ob Häufigkeitsspitzen mit bestimmten Ereignissen oder Maßnahmen korrelieren
- Nutzung der KWIC-Ergebnisse zur Verfeinerung des semantischen Feldes für weitere Frequenzanalysen
- Kombinierte Darstellung von quantitativen Trends und exemplarischen KWIC-Auszügen in einer Forschungspräsentation
````
