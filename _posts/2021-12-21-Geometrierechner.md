# Gruppenarbeit LA 1400

## Aufgabenstellung
Bei diesem Auftrag konnte sich unsere Gruppe zwischen mehreren Aufträgen entscheiden, welchen wir erledigen wollten. Unsere Gruppe entschied sich schlussendlich für den Auftrag mit dem Geometrierechner.

##### Mein Ziel:
- Bei Auswahl von Formeln erscheinen nur die nötigen Eingabe Felder

## Code welcher Eingabe Felder verschwinden und erscheinen lässt

```
  private void button2_Click(object sender, EventArgs e)
        {
            WantedCalculation = "Scope";
            label1.Text = "You have chosen scope";
            length2 = 0;
            length3 = 0;
            label7.Visible = false; //height
            textBox4.Visible = false; //height input
            label4.Visible = true; // Length 1
            textBox3.Visible = true; // Length 1 input
            label5.Visible = true; // Length 2
            textBox1.Visible = true; // Lenght 2 input
            label6.Visible = true; // Lenght 3
            textBox2.Visible = true; // Length 3 input
        }

        private void button1_Click(object sender, EventArgs e)
        {
            WantedCalculation = "Surface";
            label1.Text = "You have chosen surface";
            label7.Visible = true; //height
            textBox4.Visible = true; //height input
            label4.Visible = true; // Lenght 1
            textBox3.Visible = true; // Length 1 input
            label5.Visible = false; // Length 2
            textBox1.Visible = false; // Length 2 input
            label6.Visible = false; // Length 3
            textBox2.Visible = false; // Length 3 input
        }
```


## Eingabe Felder Anzeiger bei Oberflächen Berechnung

![Bild](https://snipboard.io/TQmfKM.jpg)

## Auswahl zwischen Scope und Surface

[![thumbnail](https://snipboard.io/j9B7TW.jpg)](https://youtu.be/ibnotyAWhQk)

## Reflektion und Verifikation

Wieder anfängliche Probleme mit Vorstellung des Programms, einige hatten andere Vorstellung des Programms als andere. Wir konnten uns schlussendlich auf eine Vorstellung einigen, welche aber schlussendlich während des Programmierens wieder über den Haufen geworfen werden musste, da sie zum Programmieren für uns noch zu schwierig und kompliziert war.

**VBV:** Am Anfang besseres einschätzen unserer Fähigkeiten und ebenfalls besseres einschätzen was in unserer zur Verfügung stehender Zeit möglich ist. Auch am Anfang lieber nur ein kleines Programm planen, welches man bei früherer Beendigung als gedacht, ausbauen kann.
 
 
 
| Ziel| Wie überprüft?|erreicht?| 
| ---| ---|---| 
|Bei Auswahl von Formeln erscheinen nur die nötigen Eingabe Felder| Programm gestartet und von dort die Dreieck Berechnung ausgewählt und dann die Eingabe Felder bei Scope und Surface überprüft (müssten unterschiedlich sein) | ☑  |
