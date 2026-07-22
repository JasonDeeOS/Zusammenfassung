1. Strukturplan
2. Vorgangsliste
3. Gantt-Diagramm bzw. Netzplan

## Netzplan

![[Pasted image 20260207231720.png]]

- FAZ/FEZ: Frühester Anfangs- bzw. Endzeitpunkt eines Vorgangs
- SAZ/SEZ: Spätester Anfangs- bzw. Endzeitpunkt eines Vorgangs
- D: Dauer eines Vorgangs (meist in Tagen)
- GP: Gesamtpuffer; Gibt an, um wie viel Tage ein Vorgang verschoben werden kann, ohne das Projektende zu gefährden
- FP: Freier Puffer; Gibt die Dauer an, die mit dem Beginn des nachfolgenden Vorgangs gewartet werden kann

### 16 Regeln für die Anwendung der Netzplantechnik

1. Abhängigkeiten werden durch Pfeile dargestellt. Pfeilrichtung: von links nach rechts und vorzugsweise von oben nach unten
2. Ein Vorgang kann mehrere Vorgänger und/oder Nachfolger haben
3. Ein Netzplan darf keine Schleifen enthalten (Zeitrechnung wäre dann nicht möglich)
4. Vom Projektanfang (Startknoten) bis zum Projektende (Zielknoten) muss ein ununterbrochener Ablauf gegeben sein
5. Der Startvorgang beginnt mit einem FAZ von 0
6. FEZ = FAZ + Dauer
7. FEZ eines Vorgangs ist FAZ aller unmittelbar nachfolgenden Vorgänge
8. Münden mehrere Vorgänge in einen Knoten, so ist dessen FAZ der größte FEZ aller Vorgänger
9. FEZ des Zielknotens ist SEZ des Projekts
10. SAZ = SEZ - Dauer
11. SAZ eines Vorgangs ist SEZ aller unmittelbar vorausgehenden Vorgänge
12. Haben mehrere Vorgänge einen gemeinsamen Vorgänger, so ist dessen SEZ der früheste (kleinste) SAZ aller Nachfolger. Zur Kontrolle: Der SAZ des Startknotens muss den Wert 0 aufweisen.
13. GP = SAZ - FAZ oder GP = SEZ - FEZ
14. FP des Vorgangs A = FAZ des Nachfolgers B - FEZ des Vorgangs A
15. Vorgänge ohne Zeitreserven sind kritische Vorgänge
16. Der kritische Weg ist die Kette aller kritischen Vorgänge