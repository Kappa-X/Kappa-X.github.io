---
layout: post
title: Random Number Guesser 
---


## Aufgabenstellung
Der Auftrag der BBBaden war einen eigenen funktionierenden Random Number Guesser zu programmieren

Meine Ziel war es von selber einen eigenen If-Loop zu programmieren nur mit Hilfe meines eigenen Wissen aus dem Unterricht und Infos von der Website [**Codecademy**](https://www.codecademy.com/learn/learn-c-sharp). Ebenfalls will ich auch so lernen wie man einen Absturz verhindert. Auch will ich das mein Programm für Falsche, Richtige und Fehlerhafte Eingabe jeweils eine andere Schriftfarbe hat

## Code des If-Loop

```
  while (lucky != GuessConvert)
                    {
                        Console.ForegroundColor = ConsoleColor.DarkRed;
                        Console.Beep();

                        if ((GuessConvert > 100) || (GuessConvert < 1))
                        {
                            Console.WriteLine("your number isn't betwenn 1 and 100. Please try again");
                            userinput = Console.ReadLine();
                            GuessConvert = Convert.ToInt32(userinput);
                        }

                        Console.Beep();

                        if (GuessConvert > lucky)
                        {
                            Console.ForegroundColor = ConsoleColor.DarkRed;
                            Console.WriteLine("Try a smaller number");
                        }

                        if (GuessConvert < lucky)
                        {
                            Console.ForegroundColor = ConsoleColor.DarkRed;
                            Console.WriteLine("Try a bigger number");
                        }
                        userinput = Console.ReadLine();
                        GuessConvert = Convert.ToInt32(userinput);
                        tries = tries + 1;
                    }

                    if (GuessConvert == lucky)
                        Console.ForegroundColor = ConsoleColor.Green;
                    Console.WriteLine("You are great You tried " + tries + " time(s)");
                    Console.WriteLine("Do you want to try again? [yes|no]");
                    start =Console.ReadLine();
                    Console.Clear();
                }
```


## Try and Catch Meldung in der Konsolenanwendung

![Bild](https://snipboard.io/8jaWg9.jpg)

## Video zum If-Loop und dem Try and Catch im Game

[![thumbnail](https://snipboard.io/ekSvXD.jpg)](https://www.youtube.com/watch?v=G-qD7WWYFr0)

## Reflektion und Verifikation

Ich kamm am Anfang sehr schnell voran mit dem Programmieren des If-Loops und dem Try und Catch mit der Hilfe von Codecademy und konnte deshalb schon sehr schnell das Hauptprogramm des Random Number Guesser fertig stellen. Erst als ich anfing mit dem einfügen von Features (verschiedene Farben für Eingaben)  fiel mir dann auf das der Loop noch nicht ganz perfekt war und noch sehr fehleranfällig war.

**VBV:** Das nächstemal probiere ich ein bisschen langsamer und genauer zu arbeiten, um so zu verhindern das ich im Nachhinein viele kleine Fehler fixen muss.
 
 
 
| Ziel| Wie überprüft?|erreicht?| 
| ---| ---|---| 
| Einen funktionierenden Loop programmieren | Ich habe den Loop in meinem Random Number Guesser benutzt und geschaut, ob er seine Funktion erfüllt|  ☑ |
| Absturz des Programms verhindern| Ich habe irgend ein Buchstaben in meine Konsole eingegeben und geschaut ob das Programm abstürzt. | ☑  |
|Verschiedene Farben für die Eingaben| Ich habe die verschiedenen Eingaben getestet und mir die Farbe der Schrift angeschaut| ☑  |
