# 🏆Selbsttest: Wissen und Praxis

````{admonition} Hinweis
:class: hinweis
Diese Übungsaufgaben dienen Ihrer Selbsteinschätzung und helfen Ihnen, das im Kapitel Gelernte zu reflektieren.

Sie können die Fragen in beliebiger Reihenfolge beantworten und auch mehrfach versuchen. 

**So funktioniert es:**
- Wählen Sie bei jeder Frage die Antwort(en), die Sie für richtig halten.
- Lesen Sie das Feedback zu den einzelnen Antwortoptionen sorgfältig durch.
- Die Erklärungen helfen Ihnen, Ihr Verständnis zu vertiefen – auch bei korrekten Antworten.

Es erfolgt keine Bewertung oder Speicherung Ihrer Ergebnisse. Nutzen Sie dieses Assessment, um Wissenslücken zu identifizieren und gegebenenfalls die entsprechenden Abschnitte des Kapitels noch einmal zu bearbeiten.

**Geschätzte Zeit**: 45min

**Viel Erfolg!**
````

## Frage 1
(Wählen Sie alle zutreffenden Antworten aus.)


```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

""" 
Lernziel: 
     Sie können verschiedene Verfahren der OCR-Nachbearbeitung beschreiben und deren Einsatzzwecke unterscheiden
Bloom-Stufe: Verstehen
Format: Multiple Choice
Geschätzte Zeit: 15 Minuten
"""

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_1 = [{
    "question": """Welche der folgenden Fehler fallen in die Kategorie \"Zeichenerkennung\"?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Fehlende Absätze",
            "correct": False,
            "feedback": """× Nicht korrekt. Dieser Fehler gehört zur Kategorie \"Formatierung\", da es sich um ein Layoutproblem handelt und nicht um die falsche Erkennung einzelner Zeichen."""
        },
        {
            "answer": "Der Buchstabe \"l\" (kleines L) wird als Ziffer \"1\" (Eins) erkannt",
            "correct": True,
            "feedback": """✓ Richtig! Dies ist ein klassischer Zeichenerkennungsfehler, der durch visuelle Ähnlichkeit der Zeichen entsteht."""
        },
        {
            "answer": "Verlorene Überschriftenformatierung",
            "correct": False,
            "feedback": """× Nicht korrekt. Dies gehört zur Kategorie \"Formatierung\", da es die Struktur des Dokuments betrifft."""
        },
        {
            "answer": "Die Buchstabenfolge \"rn\" wird als Buchstabe \"m\" interpretiert",
            "correct": True,
            "feedback": """✓ Richtig! Hierbei handelt es sich um einen Zeichenerkennungsfehler, bei dem ähnlich aussehende Zeichenkombinationen falsch interpretiert werden."""
        }
    ]
}]

display_quiz(multiple_choice_1, colors=colors.jupyterquiz)
```

## Frage 2
(Wählen Sie alle zutreffenden Antworten aus.)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_2 = [{
    "question": """Welche Aussagen zu Formatierungsfehlern bei der OCR sind korrekt?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Sie entstehen, weil OCR primär zeichenbasiert arbeitet",
            "correct": True,
            "feedback": """✓ Richtig! OCR-Systeme konzentrieren sich hauptsächlich auf die Erkennung einzelner Zeichen, wodurch Layoutinformationen und Strukturelemente oft verloren gehen."""
        },
        {
            "answer": "Sie haben keinen Einfluss auf die weitere Verarbeitung des Textes",
            "correct": False,
            "feedback": """× Nicht korrekt. Formatierungsfehler können die weitere Verarbeitung erheblich beeinträchtigen, da strukturelle Informationen wichtig für viele Analyseverfahren sind."""
        },
        {
            "answer": "Sie betreffen hauptsächlich einzelne Buchstaben",
            "correct": False,
            "feedback": """× Nicht korrekt. Formatierungsfehler betreffen größere Strukturelemente wie Absätze, Überschriften und das allgemeine Layout, nicht einzelne Zeichen."""
        },
        {
            "answer": "Sie beeinträchtigen die Dokumentstruktur und Lesbarkeit",
            "correct": True,
            "feedback": """✓ Richtig! Formatierungsfehler wirken sich direkt auf die Struktur des Dokuments und damit auf dessen Lesbarkeit und Verständlichkeit aus."""
        }
    ]
}]

display_quiz(multiple_choice_2, colors=colors.jupyterquiz)
```

## Frage 3
(Wählen Sie alle zutreffenden Antworten aus.)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_3 = [{
    "question": """Welche Eigenschaften treffen auf die manuelle OCR-Korrektur zu?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Sie ist gut skalierbar für große Textkorpora",
            "correct": False,
            "feedback": """× Nicht korrekt. Manuelle Korrektur ist zeitintensiv und daher für große Textmengen schwer skalierbar."""
        },
        {
            "answer": "Sie ermöglicht kontextsensitive Entscheidungen",
            "correct": True,
            "feedback": """✓ Richtig! Menschen können den Kontext besser verstehen und entsprechend korrekte Entscheidungen bei der Texterkennung treffen."""
        },
        {
            "answer": "Sie ist zeitaufwändig",
            "correct": True,
            "feedback": """✓ Richtig! Die manuelle Korrektur erfordert viel Zeit, da jeder Text individuell geprüft und korrigiert werden muss."""
        },
        {
            "answer": "Sie eignet sich für die Erstellung von Ground Truth-Daten",
            "correct": True,
            "feedback": """✓ Richtig! Manuell korrigierte Texte dienen oft als Referenz (Ground Truth) für die Bewertung automatischer OCR-Verfahren."""
        }
    ]
}]

display_quiz(multiple_choice_3, colors=colors.jupyterquiz)
```

## Frage 4
(Wählen Sie alle zutreffenden Antworten aus.)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_4 = [{
    "question": """Welche Aussagen zur automatischen OCR-Korrektur sind zutreffend?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Sie arbeitet immer fehlerfrei",
            "correct": False,
            "feedback": """× Nicht korrekt. Automatische Korrekturverfahren können nicht alle Fehler erkennen und manchmal sogar neue Fehler einführen."""
        },
        {
            "answer": "Sie ist effizient für große Textmengen",
            "correct": True,
            "feedback": """✓ Richtig! Automatische Korrektur ermöglicht die schnelle Verarbeitung großer Textmengen und ist daher für umfangreiche Korpora geeignet."""
        },
        {
            "answer": "Sie kann neue Fehler einführen",
            "correct": True,
            "feedback": """✓ Richtig! Da das Kontextverständnis automatischer Systeme begrenzt ist, können falsche Korrekturen vorgenommen werden, die neue Fehler erzeugen."""
        },
        {
            "answer": "Sie erfordert keine weitere Qualitätskontrolle",
            "correct": False,
            "feedback": """× Nicht korrekt. Auch nach automatischer Korrektur ist eine Qualitätskontrolle sinnvoll, um die Zuverlässigkeit der Ergebnisse zu gewährleisten."""
        }
    ]
}]

display_quiz(multiple_choice_4, colors=colors.jupyterquiz)
```

## Frage 5

```{code-cell} ipython3
:tags: [remove-input]
import sys
sys.path.append("../quadriga")
from assessment import DragDropQuiz

quiz = DragDropQuiz()

quiz.create_matching_quiz(
    title="Ordnen Sie die folgenden Schritte der OCR-Nachbearbeitung in die richtige Reihenfolge:",
    descriptions=[
        "Formatierungswiederherstellung", 
        "Grundlegende Zeichenkorrektur",
        "Vollständigkeitsprüfung"],
    options=["1", "2", "3"],
    correct_mapping={
        "Grundlegende Zeichenkorrektur" : "1",
        "Formatierungswiederherstellung" : "2",
        "Vollständigkeitsprüfung" : "3"
    }
)
```

## Frage 6
(Wählen Sie alle zutreffenden Antworten aus.)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

"""
Lernziel: Sie können regelbasierte Ansätze zur OCR-Nachkorrektur beschreiben und deren Auswirkungen auf die OCR-Qualität anhand von Metriken erläutern.
Bloom-Stufe: Verstehen, Analysieren
Format: Multiple Choice
Geschätzte Zeit: 15 Minuten
"""

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_6 = [{
    "question": """Welche Aussagen zur Änderung historischer Schreibweisen (wie 'ſ' zu 's') sind korrekt?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Es handelt sich um eine Fehlerkorrektur im engeren Sinne",
            "correct": False,
            "feedback": """× Nicht korrekt. Bei der Umwandlung historischer Schreibweisen wie 'ſ' zu 's' handelt es sich nicht um eine Fehlerkorrektur, sondern um eine Normalisierung, da die ursprüngliche Form keine fehlerhafte Erkennung darstellt."""
        },
        {
            "answer": "Die Änderung kann durch einfache Zeichenersetzung erfolgen",
            "correct": True,
            "feedback": """✓ Richtig! Diese Art der Normalisierung kann systematisch durch direkte Zeichenersetzung im gesamten Text umgesetzt werden."""
        },
        {
            "answer": "Diese Art der Änderung ist wichtig für moderne NLP-Werkzeuge",
            "correct": True,
            "feedback": """✓ Richtig! Moderne Textanalysewerkzeuge sind oft für gegenwärtige Sprachformen optimiert, weshalb die Normalisierung historischer Schreibweisen die Verarbeitungsqualität verbessert."""
        },
        {
            "answer": "Die Ersetzung muss für jeden Fall individuell entschieden werden",
            "correct": False,
            "feedback": """× Nicht korrekt. Die Ersetzung kann systematisch im gesamten Text angewendet werden, ohne Einzelfallentscheidungen."""
        }
    ]
}]

display_quiz(multiple_choice_6, colors=colors.jupyterquiz)
```

## Frage 7
(Wählen Sie alle zutreffenden Antworten aus.)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_7 = [{
    "question": """Welche Anforderungen stellt die Korrektur des OCR-Fehlers "'<' statt 'ch'"?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Die Ersetzung muss den umgebenden Kontext berücksichtigen",
            "correct": True,
            "feedback": """✓ Richtig! Der Kontext ist entscheidend, um zu bestimmen, ob '<' tatsächlich ein falsch erkanntes 'ch' ist oder ein korrektes Zeichen."""
        },
        {
            "answer": "Reguläre Ausdrücke sind für diese Korrektur nicht geeignet",
            "correct": False,
            "feedback": """× Nicht korrekt. Reguläre Ausdrücke sind besonders gut geeignet, um Muster mit Kontext zu erkennen und komplexe Ersetzungen durchzuführen."""
        },
        {
            "answer": "Die Korrektur sollte nur zwischen Buchstaben erfolgen",
            "correct": True,
            "feedback": """✓ Richtig! Um falsche Ersetzungen zu vermeiden, ist es wichtig zu prüfen, ob das '<' tatsächlich zwischen Buchstaben steht, was auf ein falsch erkanntes 'ch' hindeutet."""
        },
        {
            "answer": "Die Ersetzung kann ohne Prüfung der umgebenden Zeichen durchgeführt werden",
            "correct": False,
            "feedback": """× Nicht korrekt. Die umgebenden Zeichen müssen geprüft werden, um falsche Ersetzungen zu vermeiden."""
        }
    ]
}]

display_quiz(multiple_choice_7, colors=colors.jupyterquiz)
```

## Frage 8

Analysieren Sie die folgenden Qualitätsmetriken vor und nach der regelbasierten Korrektur:

Vor Korrektur:
- Precision: 0.778
- Recall: 0.7932
- F1-score: 0.7855

Nach Korrektur:
- Precision: 0.8091
- Recall: 0.8248
- F1-score: 0.8169

(Wählen Sie alle zutreffenden Antworten aus.)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_8 = [{
    "question": """Welche Aussagen sind korrekt?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Die Precision hat sich stärker verbessert als der Recall",
            "correct": False,
            "feedback": """× Nicht korrekt. Die Precision stieg von 0.778 auf 0.8091 (Verbesserung um 0.0311), während der Recall von 0.7932 auf 0.8248 stieg (Verbesserung um 0.0316), was eine leicht stärkere Verbesserung des Recalls bedeutet."""
        },
        {
            "answer": "Der Recall hat die stärkste prozentuale Verbesserung erfahren",
            "correct": True,
            "feedback": """✓ Richtig! Die Verbesserung des Recalls ist prozentual am stärksten, was auf eine bessere Erkennung vorhandener Zeichen und eine effektivere Normalisierung hindeutet."""
        },
        {
            "answer": "Der F1-Score ist um etwa 3 Prozentpunkte gestiegen",
            "correct": True,
            "feedback": """✓ Richtig! Der F1-Score stieg von 0.7855 auf 0.8169, was einer Verbesserung um 0.0314 bzw. etwa 3 Prozentpunkte entspricht."""
        },
        {
            "answer": "Die Korrektur hat die Gesamtqualität des OCR-Ergebnisses verschlechtert",
            "correct": False,
            "feedback": """× Nicht korrekt. Alle Metriken zeigen eine Verbesserung, was auf eine erfolgreiche regelbasierte Korrektur hinweist."""
        }
    ]
}]

display_quiz(multiple_choice_8, colors=colors.jupyterquiz)
```

## Frage 9

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_9 = [{
    "question": """Was bedeutet die Verbesserung des F1-Scores nach der regelbasierten Korrektur?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Ausschließlich eine Verbesserung der Erkennungsgenauigkeit",
            "correct": False,
            "feedback": """× Nicht korrekt. Der F1-Score berücksichtigt sowohl Precision (Genauigkeit) als auch Recall (Vollständigkeit)."""
        },
        {
            "answer": "Nur eine Verbesserung der Vollständigkeit des erkannten Textes",
            "correct": False,
            "feedback": """× Nicht korrekt. Der gestiegene F1-Score zeigt nicht nur eine Verbesserung des Recalls (Vollständigkeit), sondern auch der Precision."""
        },
        {
            "answer": "Eine ausgewogene Verbesserung von Precision und Recall",
            "correct": True,
            "feedback": """✓ Richtig! Der F1-Score ist das harmonische Mittel aus Precision und Recall. Seine Verbesserung zeigt, dass sowohl die Genauigkeit als auch die Vollständigkeit der Texterkennung optimiert wurden, was auf eine erfolgreiche regelbasierte Korrektur hindeutet."""
        },
        {
            "answer": "Eine Verschlechterung des Gleichgewichts zwischen Precision und Recall",
            "correct": False,
            "feedback": """× Nicht korrekt. Die Daten zeigen eine Verbesserung beider Metriken und somit auch eine Verbesserung des Gleichgewichts."""
        }
    ]
}]

display_quiz(multiple_choice_9, colors=colors.jupyterquiz)
```

## Frage 10

```{code-cell} ipython3
:tags: [remove-input]
import sys
sys.path.append("../quadriga")
from assessment import DragDropQuiz

quiz = DragDropQuiz()

quiz.create_matching_quiz(
    title="Ordnen Sie die folgenden Schritte der regelbasierten OCR-Nachkorrektur in die richtige Reihenfolge:",
    descriptions=["Identifikation typischer Fehler",
        "Anwendung und Qualitätsmessung",
        "Entwicklung von Korrekturregeln" ],
    options=["1", "2", "3"],
    correct_mapping={
        "Identifikation typischer Fehler" : "1",
        "Entwicklung von Korrekturregeln" : "2",
        "Anwendung und Qualitätsmessung" : "3"
    }
)
```

## Frage 11
(Wählen Sie alle zutreffenden Antworten aus.)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_11 = [{
    "question": """Welche Aussagen zur regelbasierten OCR-Korrektur sind korrekt?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Reguläre Ausdrücke sind für kontextabhängige Korrekturen ungeeignet",
            "correct": False,
            "feedback": """× Nicht korrekt. Reguläre Ausdrücke sind besonders gut für kontextabhängige Korrekturen geeignet, da sie Mustererkennung mit Kontext ermöglichen und flexible Regelformulierungen erlauben."""
        },
        {
            "answer": "Alle OCR-Fehler können durch regelbasierte Korrektur behoben werden",
            "correct": False,
            "feedback": """× Nicht korrekt. Nicht alle OCR-Fehler können durch regelbasierte Ansätze korrigiert werden, besonders wenn sie stark kontextabhängig sind oder keine erkennbaren Muster aufweisen."""
        },
        {
            "answer": "Reguläre Ausdrücke ermöglichen flexible und komplexe Ersetzungen",
            "correct": True,
            "feedback": """✓ Richtig! Reguläre Ausdrücke bieten die Möglichkeit, komplexe Muster zu erkennen und flexible Ersetzungen durchzuführen, was sie zu einem wichtigen Werkzeug bei der regelbasierten Korrektur macht."""
        },
        {
            "answer": "Manche Fehler erfordern eine Kombination verschiedener Korrekturmethoden",
            "correct": True,
            "feedback": """✓ Richtig! Komplexe Fehler können nicht immer durch einen einzelnen Ansatz behoben werden und erfordern oft eine Kombination von regelbasierten, statistischen oder maschinellen Lernmethoden."""
        }
    ]
}]

display_quiz(multiple_choice_11, colors=colors.jupyterquiz)
```

## Frage 12

(Wählen Sie alle zutreffenden Antworten aus.)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

"""
Lernziel: Sie können die grundlegenden Herausforderungen beim Einsatz von Large Language Models für die OCR-Nachbearbeitung beschreiben
Bloom-Stufe: Verstehen
Format: Multiple Choice
Geschätzte Zeit: 15 Minuten
"""

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_12 = [{
    "question": """Welche Aussagen beschreiben die Herausforderungen beim Einsatz von Large Language Models für die OCR-Nachbearbeitung korrekt?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "LLMs benötigen erhebliche Rechenressourcen und können typischerweise nicht auf einem herkömmlichen PC ausgeführt werden",
            "correct": True,
            "feedback": """✓ Richtig! LLMs haben einen hohen Bedarf an Rechenleistung, verbrauchen viel Energie, benötigen großen Speicher und erfordern spezielle Infrastruktur."""
        },
        {
            "answer": "LLMs liefern bei gleichem Input immer identische Ergebnisse",
            "correct": False,
            "feedback": """× Nicht korrekt. LLMs sind nicht-deterministisch, d.h. ihre Ergebnisse können variieren, selbst bei identischen Eingaben. Kleine Prompt-Änderungen können zu unterschiedlichen Resultaten führen."""
        },
        {
            "answer": "Ungenaue Prompts können dazu führen, dass LLMs den Originaltext unbeabsichtigt verändern",
            "correct": True,
            "feedback": """✓ Richtig! Dies ist eine zentrale Herausforderung, da ungenaue Anweisungen zu unerwünschter Textgenerierung führen können, die vom Original abweicht und den Text verfälschen kann."""
        },
        {
            "answer": "Die Verarbeitung großer Textkorpora mit LLMs ist problemlos möglich",
            "correct": False,
            "feedback": """× Nicht korrekt. Die Verarbeitung großer Textkorpora ist durch begrenzte Eingabe- und Ausgabegrößen, ressourcenintensive Verarbeitung und eingeschränkten Zugriff auf LLM-Dienste stark limitiert."""
        }
    ]
}]

display_quiz(multiple_choice_12, colors=colors.jupyterquiz)
```

## Frage 13
(Wählen Sie alle zutreffenden Antworten aus.)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_13 = [{
    "question": """Welche der folgenden Aspekte gehören zu den ressourcenbezogenen Herausforderungen beim Einsatz von LLMs für die OCR-Nachbearbeitung?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Hoher Bedarf an Rechenleistung",
            "correct": True,
            "feedback": """✓ Richtig! LLMs erfordern signifikante Rechenkapazitäten, was ihre Anwendung in ressourcenbeschränkten Umgebungen einschränkt."""
        },
        {
            "answer": "Geringe Speicheranforderungen",
            "correct": False,
            "feedback": """× Nicht korrekt. LLMs haben gerade keine geringen, sondern sehr hohe Speicheranforderungen, da ihre Modellarchitekturen und Parameter umfangreich sind."""
        },
        {
            "answer": "Hoher Energieverbrauch",
            "correct": True,
            "feedback": """✓ Richtig! Das Training und die Anwendung von LLMs sind energieintensiv, was sowohl ökologische als auch wirtschaftliche Auswirkungen hat."""
        },
        {
            "answer": "Flexibler Einsatz auf Standard-Hardware",
            "correct": False,
            "feedback": """× Nicht korrekt. Aufgrund ihres hohen Ressourcenbedarfs können LLMs typischerweise nicht flexibel auf gewöhnlicher Hardware eingesetzt werden, sondern benötigen spezielle Infrastruktur wie leistungsstarke GPUs oder TPUs."""
        }
    ]
}]

display_quiz(multiple_choice_13, colors=colors.jupyterquiz)
```

## Frage 14
(Wählen Sie alle zutreffenden Antworten aus.)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_14 = [{
    "question": """Welche orthographischen und inhaltlichen Probleme können bei der LLM-basierten OCR-Nachbearbeitung entstehen?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Zu starke Normalisierung historischer Schreibweisen",
            "correct": True,
            "feedback": """✓ Richtig! Ohne präzise Anweisungen im Prompt könnten LLMs historische Schreibweisen zu stark modernisieren und damit wichtige historische Sprachmerkmale verlieren."""
        },
        {
            "answer": "Unbeabsichtigte Veränderung des Originaltextes",
            "correct": True,
            "feedback": """✓ Richtig! LLMs könnten den ursprünglichen Text inhaltlich verändern, was besonders bei historischen oder wissenschaftlichen Texten problematisch ist."""
        },
        {
            "answer": "Einführung anachronistischer Begriffe",
            "correct": True,
            "feedback": """✓ Richtig! Ohne klare Einschränkungen im Prompt könnten LLMs moderne Begriffe in historische Texte einfügen, die zur Entstehungszeit nicht existierten."""
        },
        {
            "answer": "Bessere Erkennung von Fachtermini",
            "correct": False,
            "feedback": """× Nicht korrekt. Die Anwendung von LLMs bei der Nachbereitung führt nicht zu einer besseren Erkennung, sondern erhöht das Risiko, dass Fachbegriffe falsch interpretiert oder ersetzt werden."""
        }
    ]
}]

display_quiz(multiple_choice_14, colors=colors.jupyterquiz)
```

## Frage 15
(Wählen Sie alle zutreffenden Antworten aus.)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_15 = [{
    "question": """Eine Forschungsgruppe plant, ein historisches Zeitungskorpus von 10.000 Seiten mit LLMs nachzukorrigieren. Welche Herausforderungen sind dabei zu erwarten?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Begrenzte Kontextfenster der LLMs",
            "correct": True,
            "feedback": """✓ Richtig! LLMs haben typischerweise begrenzte Eingabe- und Ausgabegrößen (Kontextfenster), was die Verarbeitung längerer Texte erschwert und eine Aufteilung in kleinere Abschnitte erfordert."""
        },
        {
            "answer": "Hohe Kosten für API-Zugriffe",
            "correct": True,
            "feedback": """✓ Richtig! Die Verarbeitung von 10.000 Seiten über kommerzielle LLM-APIs kann erhebliche Kosten verursachen, besonders wenn mehrere Durchläufe oder Korrekturen nötig sind."""
        },
        {
            "answer": "Schwierige Nachvollziehbarkeit der Korrekturen",
            "correct": True,
            "feedback": """✓ Richtig! Aufgrund der \"Black-Box\"-Natur von LLMs kann es schwierig sein nachzuvollziehen, welche Änderungen vorgenommen wurden und warum, was die Qualitätskontrolle erschwert."""
        },
        {
            "answer": "Gleichbleibend hohe Qualität bei allen Korrekturen",
            "correct": False,
            "feedback": """× Nicht korrekt. Wegen der nicht-deterministischen Natur von LLMs und variierenden Texteigenschaften ist eine gleichbleibende Korrekturqualität über den gesamten Korpus hinweg nicht garantiert."""
        }
    ]
}]

display_quiz(multiple_choice_15, colors=colors.jupyterquiz)
```

## Frage 16
(Wählen Sie alle zutreffenden Antworten aus.)

```{code-cell} ipython3
:tags: [remove-input]
from jupyterquiz import display_quiz

import sys
sys.path.append("..")
from quadriga import colors

multiple_choice_16 = [{
    "question": """Welche Maßnahmen sind wichtig für die Qualitätskontrolle bei der LLM-basierten OCR-Nachbearbeitung?""",
    "type": "multiple_choice",
    "answers": [
        {
            "answer": "Stichprobenartige manuelle Überprüfung",
            "correct": True,
            "feedback": """✓ Richtig! Da LLMs unerwartete Änderungen vornehmen können, ist eine manuelle Kontrolle von Stichproben essentiell, um die Qualität der Korrekturen zu bewerten."""
        },
        {
            "answer": "Verzicht auf Zwischenevaluationen",
            "correct": False,
            "feedback": """× Nicht korrekt. Regelmäßige Zwischenevaluationen sind wichtig, um Probleme frühzeitig zu erkennen und die Korrekturparameter anzupassen."""
        },
        {
            "answer": "Dokumentation aller vorgenommenen Änderungen",
            "correct": True,
            "feedback": """✓ Richtig! Die Dokumentation der Änderungen ermöglicht Transparenz, Nachvollziehbarkeit und wissenschaftliche Integrität bei der Textkorrektur."""
        },
        {
            "answer": "Festlegung klarer Regeln für akzeptable Änderungen",
            "correct": True,
            "feedback": """✓ Richtig! Vorab definierte Regeln helfen, den Rahmen für erlaubte Änderungen festzulegen und das Risiko unerwünschter Modifikationen zu minimieren."""
        }
    ]
}]

display_quiz(multiple_choice_16, colors=colors.jupyterquiz)
```
