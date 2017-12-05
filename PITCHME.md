# Syntax regulärer Ausdrücke
* Ein Regulärer Ausdruck spezifiziert eine Menge von Zeichenketten, die mit dem Ausruck übereinstimmen.
* Über die Funktionen im Modul re kann geprüft werden, ob eine bestimmte Zeichenkette dem spezifizierten Muster entsprechen.
* Muster können miteinander verkettet werden.
* Ein Muster kann 'normale' Zeichen und 'spezielle' Zeichen (Metazeichen) enthalten.
  * Bsp. normale Zeichen: `a, b, 1, 2`
  * Metazeichen: `. ^ $ * + ? { } [ ] \ | ( )`
* Die besonderen Eigenschaften von Metazeichen (s.u.) können durch einen vorangestellte Rückschrägstrich (`\`) aufgehoben werden.

---

# Online-Auswertung regulärer Ausdrücke
* Im Internet gibt es zahlreiche Möglichkeiten zur Online-Auswertung von regulären Ausdrücken. Bsp.:
  * https://regex101.com/
  * https://regexr.com/
  * https://www.regextester.com/
* Die Nutzung dieser Werkzeuge erleichtert das generelle Verständnis von regulären Ausrücken und ist hilfreich bei der Erstellung konkreter regulärer Ausdrücke.

---

# Einfaches Muster
* Ein einfaches Muster könnte z.B. ausschließlich aus normalen Zeichen (Zeichenliteral) bestehen.
* Beispiel:
   * Text: "Klaus geht ohne Maus mit Laus nicht aus dem Haus."
   * Muster: `Klaus`
       * Ergebnis: 'Klaus'
       * **Klaus** geht ohne Maus mit Laus nicht aus dem Haus.
   * Muster: 'aus'
       * Ergebnis: 'aus', 'aus', 'aus', 'aus'
       * Kl**aus** geht ohne M**aus** mit L**aus** nicht **aus** dem H**aus**.
