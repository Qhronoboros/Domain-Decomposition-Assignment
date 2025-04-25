# Domain-Decomposition-Assignment

<h1>Game: R.E.P.O.</h1>

**<h3>Bo Rispens:
Player Locomotion and Interactions.</h3>**

Ik zat te denken hoe ik zelf zou beginnen met het maken er van. Dit is de eerste keer dat ik een UML maak. Dus wist niet heel goed waar ik moest beginnen.<br>
Heb eerst een gameplay uitleg van repo bekeken en daarna begonnen met de player class neerzetten.
Dan heb ik gekeken naar wat je allemaal in het spel kon / waarmee je kon interacten als speler. En vanuit daar ben ik verder gegaan.<br>


**<h3>Francisco Ngo:
Item and Object (Valuables) Variations and Effects.</h3>**

Ik heb al eerder een beetje met UML gewerkt. Dus had ik al een beetje ervaring.<br>
Eerst dacht ik aan om de Decorator Pattern te gebruiken, alleen toen realiseerde ik dat de Command Pattern handiger was, omdat je in R.E.P.O. meerdere unieke actions/events hebt voor de verschillende valuables/items.
Dus kan je met de Command Pattern elke action/event koppelen aan een specifieke Command, of meerdere Commands.<br>
De verdere gedachtegang was om in de Valuable class lists/arrays te hebben voor elke action class, dus een list voor OnGrab, OnHeld, OnRelease, OnHit, etc.
Als een specifieke action/event gebeurt, zoals OnGrab. Dan worden de correcte Commands uitgevoerd binnen de list/array.
Hierdoor hoef je niet constant de type te checken van de classes die IOnAction implementeren, wat normaal ietjes meer performance kost.
