# if.03.11 CABS Assignment: No-Beard Calculations
Erstellen Sie zwei Varianten eines NoBeard Assembler Programms, dass folgende Berechnung ausführt:   
```13 - 17 * 2 (= -21)```

## Variante 1 (calc_direct.na):
Legen Sie alle Operanden, Zwischenergebnisse und das Ergebnis der Rechnung direkt am Stack ab

## Variante 2 (calc_indirect.na):
Legen Sie alle Operanden sowie das Endergebnis im 'Heap' (bereits allokierter Speicher) so ab, dass die Operanden 13, 17, 2 an den Adresse 0, 4, 8, das Zwischenergebnis an Adresse 12 und das Endergebnis an Adresse 16 gespeichert wird. Zur Durchführung der Berechnung sind die jeweiligen Operanden aus dem Heap auf den Stack zu laden.

## Benötigte Befehle
(es dürfen auch andere / zusätzliche verwendet werden): 
- ```lit X```: Legt den Wert X auf den Stack
- ```add```: addiert die letzten beiden Werte am Stack und legt das Ergebnis am Stack ab
- ```sub```: subtrahiert die letzten beiden Werte am Stack (s2 - s1) und legt das Ergebnis am Stack ab
- ```mul```: multipliziert die letzten beiden Werte am Stack und legt das Ergebnis am Stack ab
- ```a 0 Y```: legt die Adresse (nicht den Wert!) Y auf den Stack ('pointer')
- ```lv 0 Y```: legt den Wert der Adresse Y auf den Stack (Pointer-Dereferenzierung)
- ```sto```: speichert den letzten Wert am Stack and die Adresse, die an der vorletzten Stackposition liegt
- ```halt```: beendet das Programm

Die genaue Beschreibung der Befehle finden Sie im Dokument 'NoBeardReport.pdf', Kapitel 'Instructions'.

_**Wichtig:** eine *.na* Datei ist eine Textdatei mit Unix Zeilenumbrüchen (LF)!_

**Kompilieren:** asm calc_direct.na

Ein Beispiel für eine Berechnung mit Werten, die aus dem Heap geladen werden, finden im Teams-Verzeichnis 'NoBeard' -> 'Assembler_AdditionSample.pdf'. Verwenden Sie beim Ausprobieren dieses Beispiels Adressen aus dem Bereich 8 bis 28 statt der im Beispiel verwendeten 32 - 40.

## Abgabe:
In diesem Repository

Viel Spaß beim Programmieren!
