# RandomRound
Erstellt eine Liste aller gegebenen Subjekte in zufälliger Reihenfolge oder gibt ein zufälliges Subjekt dieser Liste zurück.

## Installation
RandomRound benötigt die BASH Shell.

Um RandomRound nach /usr/local/bin/randomround zu installieren, gib folgendes ein:

> git clone https://github.com/JEFF-Media-GbR/RandomRound.git && cd RandomRound  
> chmod +x randomround  
> sudo mv randomround /usr/local/bin/  

(Nur root hat Schreibzugriff auf /usr/local/bin/. Für einen anderen Installationspfad einfach die letzte Zeile anpassen.)

## Benutzung und Parameter
Benutzung:
  `randomround [-r] [-a] [-b \"Subjekt1 Subjekt2 ...\"] [-h] [-L] [-v]`  

Parameter:  
  -r: RPS-Modus. Erfordert keine weiteren Parameter  
  -a: Bildet komplette Runde  
  -b: Übergibt direkt die Namen der Subjekte  
  -h: Zeigt diesen Hilfetext  
  -L: Deaktiviere Log-Funktion  
  -v: Verbose (Debug-Modus und Anzeigen der Zufallsberechnungen)

## Beispiele
Wer muss den Bierkasten zahlen? Wähle zufällig jemand aus den Personen Martin, Angela und Horst aus:

> ```randomround -b "Martin Angela Horst"```  
> oder  
> ```randomround``` und anschließend "Martin Angela Horst" eingeben und mit Enter bestätigen

Wie geht die Wahl aus? Generiere eine zufällige Reihenfolge aus den Personen Donald, Bernie und Hillary:

> ```randomround -ab "Donald Bernie Hillary"```  
> oder  
> ```randomround -a``` und anschließend "Donald Bernie Hillary" eingeben und mit Enter bestätigen

Wie spiele ich Schere-Stein-Papier, ohne berechnbar zu sein? Generiere eine zufällige Geste für Schere-Stein-Papier:

> ```randomround -r```  
> oder  
> ```randomround -b "Schere Stein Papier"```

## Sonstiges
RandomRound speichert in der Standardeinstellung jeden Output unter `~/.randomround.log`, um eine nachträgliche Überprüfung des Ergebnisses zu ermöglichen. Dies kann durch die Nutzung des Parameters `-L` verhindert werden.
