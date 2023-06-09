# TURTLE RUN
### Projektseite 

von Cosima und Friederike, 12bc

## Inhaltsverzeichnis
[Projektvorstellung](https://github.com/cosima-friederike/Projektseite-TURTLE-RUN/blob/main/README.md#projektvorstellung)

[Programm](https://github.com/cosima-friederike/Projektseite-TURTLE-RUN/blob/main/README.md#programm)

[Aufbau und Code](https://github.com/cosima-friederike/Projektseite-TURTLE-RUN/blob/main/README.md#aufbau-und-code)

[Arbeitstagebuch](https://github.com/cosima-friederike/Arbeitsprotokoll-2#arbeitsprotokoll-2-von-cosima-und-friederike)

## Projektvorstellung
TURTLE RUN ist ein 2D-Spiel, das sich in einer Unterwasserwelt abspielt. Das Konzept des Spiels liegt darin, dass der Hauptsprite, die Schildkröte, helle Muscheln einsammeln und dunklen Muscheln ausweichen muss. Der Spieler übernimmt dabei mithilfe der vier Pfeiltasten die Steuerung der Schildkröte. Um einen Punkt zu erzielen, muss der Spieler jedoch nicht nur eine helle Muschel berühren, sondern zusätzlich eine Wasserblase zum Platzen bringen. Diese entsteht nach dem Berühren der richtigen Muschel. Dabei startet das Spiel recht einfach, weil es zu Beginn nur helle Muscheln gibt und erst mit jeder gesammelten Muschel beziehungsweise Wasserblase eine dunkle Muschel erscheint. Mit jeder berührten Blase steigt der score um 1, wird jedoch eine falsche Muschel berührt, sinkt der Punktestand um 1. Wenn ein Punkt erspielt wurde, wird die jeweilige Wasserblase entfernt und eine neue helle Muschel wird erstellt. Außerdem kommt auch immer eine neue dunkle Muschel dazu. So wird das Spiel im Verlauf einer Runde immer schwieriger.
Sobald der Spieler 10 Punkte erreicht hat, erscheint in der Mitte des Spielfelds ein Pokal, den er berühren muss, damit die Runde als gewonnen endet. Um die Mindestanzahl an Punkten zu sammeln, hat der Spieler eine Minute Zeit, sonst endet das Spiel und der Bildschrirm zeigt "GAME OVER" an. 
## Programm
Dieses Spiel wurde mit dem Programmm SpriteLab entwickelt. Ähnlich wie bei Snap! erstellt man bei SpriteLab keine eigenen Codes, sondern arbeitet mit dem vorgegebenen Quellcode und kann die verfügbaren Blöcke nach eigenen Ideen und Vorstellungen zusammenbauen. Durch die Blockstruktur ist das Programm recht übersichtlich. Zusätzlich können neue Blöcke erstellt werden, wobei aber nur die bereits angegebenen Funktionen zur Verfügung stehen. Auch können die Blöcke nicht beliebig zusammengefügt werden, da jeweils nur bestimmte Arten von Blöcken zusammenpassen. 
## Aufbau und Code 
Bei TURTLE RUN gibt es insgesamt acht verschiedene Sprites, beziehungsweise Kostüme: Die Schildkröte, die helle und dunkle Muschel, die Wasserblase, den Pokal, den Startbutton und die "TURTLE RUN"- und "GAME OVER"-Schriftzüge. 
![image](https://user-images.githubusercontent.com/111414772/230602302-bd49642b-c4ff-4e0b-8ae4-bc7dbfbc65e0.jpeg)
Bild 1

Auf dem Bild ist das Spiel kurz vor dem Sieg zu erkennen. Der Spieler hat mit der Schildkröte den Score von 10 erreicht und der Pokal ist somit erschienen.
#### TURTLE RUN
Wird auf "Ausführen" geklickt, so wird der Hintergrund gestellt und ein Schriftzug, sowie ein Startbutton werden erstellt. Der Schriftzug TURTLE RUN ist ein selbstkreierter Sprite, der auf dem Startbildschirm den Namen des Spieles darstellen soll. Der Sprite selbst hat ansonsten keine weiter Funktion.
![image](https://user-images.githubusercontent.com/111414772/230605161-99ed1b0b-36ba-47cc-b09a-53916c311bf7.jpeg)
Bild 2
#### Startbutton
Der Startbutton ist ein Sprite, den es schon als Vorlage gab. Er liegt, ebenso wie der Schriftzug TURTLE RUN, auf dem Startbildschirm (siehe Bild 2). 
Wird auf den Button geklickt, so öffnet sich der Spielbildschirm. Es erscheinen die Schildkröte, der score und die Muscheln. Der Button und der Name des Spiels verschwinden währenddessen.
![image](https://user-images.githubusercontent.com/111414772/230606395-2098c979-6cf6-48a6-98e3-c07042abdfb8.jpeg)
Bild 3
#### Schildkröte
Die Schildkröte stellt den Hauptsprite dar, der von dem Spieler mit den vier Pfeiltasten gesteuert wird. Sie wird erstellt, wenn der Startbutton geklickt wurde. Zusätzlich sagt sie bei Beginn einer Spielrunde die Worte "I´m ready" (siehe Bild 3).
#### Helle Muschel
Helle Muscheln entstehen ebenfalls nach dem Klicken des Startbuttons. Es erscheinen zu Beginn 3 Muscheln an zufälligen Positionen (siehe Bild 3). Anschließend wird immer dann, wenn der score um einen Punkt steigt, eine neue Muschel hinzugefügt. Es befinden sich also immer höchstens drei helle Muscheln auf dem Spielfeld. Die Muscheln wandern zufällig auf dem Bildschirm herum.
#### Wasserblase
Wird eine helle Muschel von der Schildkröte berührt, so verschwindet diese und an einer anderen Position entsteht eine Wasserblase. Die Wasserblase muss berührt werden, damit der Spieler einen Punkt erhält. Zusätzlich werden bei Berühren der Blase wieder eine neue helle Muschel sowie eine dunkle Muschel erstellt.
![image](https://user-images.githubusercontent.com/111414772/230610704-0b8fc797-4e6d-4d5a-8880-e9e734d2b791.jpeg)
Bild 4
#### Dunkle Muschel
Die dunklen Muscheln dürfen nicht von der Schildkröte berührt werden. Andernfalls sinkt der score um einen Punkt und die Schildkröte sagt einen kurzen Moment "aua". Die dunklen Muscheln entstehen immer dann, wenn eine Wasserblase berührt wurde und bewegen sich ebenfalls zufällig auf dem Bildschrim. Sie sind allerdings viel kleiner und langsamer als die hellen Muscheln (siehe Bild 4).
![image](https://user-images.githubusercontent.com/111414772/230613059-52f778f9-ad96-4bb4-9d03-6c31d59a5b01.jpeg)
Bild 5
#### Pokal
Wird ein score von 10 erreicht, taucht ein Pokal auf. Er bewegt sich auf einer Horizontalen und muss für den Sieg eingesammelt werden. Außerdem fängt der Pokal an, zu schrumpfen. Der Spieler muss also möglichst schnell zu dem Pokal gelangen. Sobald der Pokal berührt wurde, erscheint ein neuer Hintergrund mit den Worten "congrats!" und "you won :)".
![image](https://user-images.githubusercontent.com/111414772/230616252-fcbcd365-f90a-4099-be33-f05af7093c4a.jpeg)
Bild 6
#### GAME OVER
Falls der Spieler es nicht schafft, die benötigten Punkte und den Pokal innerhalb der 120 Sekunden zu sammeln, erscheint ein dunkler Hintergund mit dem Schriftzug GAME OVER. Der Schriftzug ist, ebenso wie die Worte TURTLE RUN zu Beginn des Spiels, ein Sprite, der ansonsten keine weitere Funktion besitzt. Allerdings stammt dieser Sprite aus den Vorlagen und wurde nicht von uns selbst kreiert.
![image](https://user-images.githubusercontent.com/111414772/230617819-559de529-af47-42a7-bed4-7ab2a919d0c8.jpeg)
Bild 7
