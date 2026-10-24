- bedeutet Vielgestaltigkeit
- Objekte mit gemeinsamer Schnittstelle aber unterschiedlichen Verhalten
## Beispiel

```c#
class Tier
{
    public virtual void Geraeusch()
    {
        Console.WriteLine("Ein Tier macht ein Geräusch.");
    }
}

class Hund : Tier
{
    public override void Geraeusch()
    {
        Console.WriteLine("Wuff!");
    }
}

class Katze : Tier
{
    public override void Geraeusch()
    {
        Console.WriteLine("Miau!");
    }
}
```

Jetzt nutzen wir Polymorphie:

```c#
Tier tier1 = new Hund();
Tier tier2 = new Katze();

tier1.Geraeusch(); // Wuff!
tier2.Geraeusch(); // Miau!
```

Was passiert hier?
- `Tier` ist die Basisklasse.
- `Hund` und `Katze` sind abgeleitete Klassen.
- `virtual` erlaubt das Überschreiben einer Methode.
- `override` überschreibt die Methode in der abgeleiteten Klasse.
- Obwohl beide Variablen vom Typ `Tier` sind, wird die Methode des tatsächlichen Objekts ausgeführt.
## Unterschied Vererbung - Polymorphie

| Vererbung                                                | Polymorphie                                                 |
| -------------------------------------------------------- | ----------------------------------------------------------- |
| Unterklasse übernimmt Attribute/Methoden der Basisklasse | Ausführen derselben Methoden je nach Klasse unterschiedlich |
| Ist-ein-Beziehung                                        | unterschiedlicher Verhalten über einen gemeinsamen Typ      |
| Hund : Tier                                              | Tier tier = new Hund();                                     |
