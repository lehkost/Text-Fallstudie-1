(corpus-collection_text_as_digital_objects)=
# Elemente von Korpora: Texte als digitale Objekte

Texte können digital auf sehr unterschiedliche Weisen gespeichert, prozessiert und repräsentiert werden. Die vielfältigen Formen von Text im Digitalen weisen dabei jeweils spezifische Eigenschaften und Einsatzmöglichkeiten auf. In diesem Abschnitt werden vier weit verbreitete Erscheinungsformen digitaler Texte vorgestellt:

- Bilddigitalisate von Text (z.B. PDF, PNG, JPG, TIFF)
- Reiner Text, auch „Plain Text“ (TXT)
- XML/TEI
- CSV

## Bilddigitalisate von Text

**Charakteristika:**

- **Repräsentation:** Bilddigitalisate sind digitale Abbildungen von Originaldokumenten. Sie bewahren deren visuelle Gestalt, einschließlich Layout, Schriftarten und Illustrationen.
- **Formate:** Die gängigsten Formate sind PDF, PNG und JPG.
- **Nutzung:** Diese Form ist besonders nützlich für die Archivierung und den Zugang zu historischen Dokumenten, da sie eine authentische visuelle Wiedergabe des Originals ermöglicht.
- **Einschränkungen:** Der Textinhalt ist in diesen Formaten nicht direkt durchsuchbar oder maschinenlesbar, es sei denn, es wird eine optische Zeichenerkennung (OCR) angewendet.

**Beispiel:**

```{figure} ../assets/images/corpus-collection_text_as_digital_objects_image-example.png
---
height: 200
name: Snippet eines Bilddigitalisats
---
```

*Beispiel für ein Bilddigitalisat von Text, hier ein Ausschnitt eines historischen Zeitungsartikels als PNG-Datei*

## Reiner Text, „Plain Text“

**Charakteristika:**

- **Repräsentation:** Plain Text ist eine einfache, unformatierte Textdatei, die nur den reinen Text ohne jegliche Stilelemente oder Metadaten enthält.
- **Formate:** Das gängigste Format ist TXT.
- **Nutzung:** Plain Text ist ideal für einfache Textanalysen und die Datenverarbeitung, da er leicht zu bearbeiten und in verschiedenen Softwareumgebungen zu importieren ist.
- **Einschränkungen:** Es fehlen strukturelle und semantische Informationen, etwa in Form von Textauszeichnungen, die für komplexere Analysen oder Darstellungen notwendig sind.

**Beispiel:**

`
Die Grippe wütet weiter
Zunahme der schweren Fälle in Berlin.
Die Zahl der Grippefälle ist in den letzten beiden Tagen auch in Groß-Berlin noch deutlich gestiegen. Die Warenhäuser und sonstigen Geschäfte, die Kriegs- und die privaten Betriebe klagen, dass übermäßig viele Angestellte krank melden müssen, und auch bei der Post und bei der Straßenbahn ist die Zahl der Grippekranken bedeutend gestiegen.
`

*Beispiel für reinen Text ohne jede Formatierung, üblicherweise als TXT-Datei gespeichert*


## XML/TEI

**Charakteristika:**

- **Repräsentation:** XML (eXtensible Markup Language) ermöglicht eine strukturierte Darstellung von Texten mit verschachtelten Tags, die die semantische Struktur und Metadaten enthalten. TEI (Text Encoding Initiative) ist ein spezieller XML-Standard für die Kodierung von historischen Texten.
- **Formate:** Dateien im XML-Format, oft mit der Endung .xml.
- **Nutzung:** XML/TEI wird häufig in den Geisteswissenschaften verwendet, um komplexe Textstrukturen und Annotationen zu kodieren, wie z.B. Kapitelüberschriften, Fußnoten, Zitate und sprachliche Besonderheiten.
- 	**Einschränkungen:** Die Erstellung und Verarbeitung von XML/TEI-Dokumenten setzen eine genaue Kenntnis der <a href="https://tei-c.org/guidelines/" class="external-link" target="_blank">TEI Guidelines</a> voraus. Zudem unterscheidet sich die Arbeit in den verwendeten Editoren, etwa <a href="https://www.oxygenxml.com/" class="external-link" target="_blank">Oxygen XML Editor</a>, <a href="https://notepad-plus-plus.org" class="external-link" target="_blank">Notepad++</a> oder <a href="https://code.visualstudio.com/" class="external-link" target="_blank">Visual Studio Code</a>, was den Einstieg erschwert.

**Beispiel:**

```
<?xml version="1.0" encoding="UTF-8"?>
<TEI xmlns="http://www.tei-c.org/ns/1.0">
  <teiHeader>
      <fileDesc>
         <titleStmt>
            <title>Die Grippe wütet weiter</title>
         </titleStmt>
         <publicationStmt>
            <publisher>Berliner Morgenpost</publisher>
            <pubPlace>Berlin</pubPlace>
            <date when="1918-10-15"/>
         </publicationStmt>
         <sourceDesc>
            <p>Digitalisat bereitgestellt vom ZEFYS - ZEitungsinFormationssYStem der Staatsbibliothek zu Berlin</p>
         </sourceDesc>
      </fileDesc>
  </teiHeader>
  <text>
      <body>
         <head>
            Die Grippe wütet weiter
         </head>
         <p>Some text here.</p>
      </body>
  </text>
</TEI>
```

*Beispiel für eine XML-Kodierung nach TEI-Standard. Am Anfang der Datei steht der `<teiHeader>` mit Metadaten, es folgt das `<text>`-Element, in dem der Text mit Strukturinformationen (z.B. `<head>` für Überschrift) gespeichert wird*

## CSV für annotierte Texte

**Charakteristika:**

- **Repräsentation:** CSV (Comma-Separated Values) ist ein tabellarisches Datenformat, bei dem jeder Eintrag in einer Zeile einer Tabelle durch ein Trennzeichen (meist ein Komma) getrennt ist. Es eignet sich gut für die Speicherung von Daten, die aus Texten extrahiert und annotiert wurden.
- **Formate:** Dateien im CSV-Format, oft mit der Endung .csv.
- **Nutzung:** CSV-Dateien werden häufig in der Computerlinguistik verwendet, um annotierte Textdaten zu speichern, wie z.B. Wortformen, Lemmas, syntaktische Strukturen oder semantische Annotationen. Sie sind leicht mit Statistik- und Analysewerkzeugen zu verarbeiten.
- **Einschränkungen:** CSV-Dateien sind weniger flexibel für komplexe Textstrukturen und eignen sich besser für flache, tabellarische Daten.

**Beispiel:**

```
ID,TOKEN,LEMMA,POS
1,Die,die,DET
2,Grippe,Grippe,NOUN
3,wütet,wüten,VERB
4,weiter,weiter,ADV
6,Zunahme,Zunahme,NOUN
7,der,der,DET
8,schweren,schwer,ADJ
9,Fälle,Fall,NOUN
10,in,in,ADP
11,Berlin,Berlin,PROPN
12,.,.,PUNCT
```

*CSV-Datei, deren erste Zeile die Spaltenüberschriften enthält und in deren nachfolgenden Zeilen jeweils zunächst eine fortlaufende ID, dann ein Wort sowie weitere linguistische Informationen aufgeführt sind: Grundform („Lemma”) und Wortart („POS”, „Part of Speech”)*


| ID  | TOKEN    | LEMMA   | POS   |
|-----|----------|---------|-------|
| 1   | Die      | die     | DET   |
| 2   | Grippe   | Grippe  | NOUN  |
| 3   | wütet    | wüten   | VERB  |
| 4   | weiter   | weiter  | ADV   |
| 6   | Zunahme  | Zunahme | NOUN  |
| 7   | der      | der     | DET   |
| 8   | schweren | schwer  | ADJ   |
| 9   | Fälle    | Fall    | NOUN  |
| 10  | in       | in      | ADP   |
| 11  | Berlin   | Berlin  | PROPN |
| 12  | .        | .       | PUNCT |

*CSV-Dateien lassen sich, wie hier zu sehen, mit gängigen Programmen wie LibreOffice oder Microsoft Office auch in Tabellenform darstellen*


## Zusammenfassung
Jedes der vorgestellten Formate hat eigene Stärken und Schwächen und ist für unterschiedliche Anwendungszwecke geeignet. Während Bilddigitalisate die visuelle Authentizität bewahren, bieten Plain Text und CSV einfache Möglichkeiten zur maschinellen Verarbeitung. XML/TEI hingegen ermöglicht eine detaillierte und semantisch reiche Darstellung von Texten. Das Verständnis dieser Formate ist essentiell für die effektive Arbeit mit digital vorliegenden Texten in den Digital Humanities.
