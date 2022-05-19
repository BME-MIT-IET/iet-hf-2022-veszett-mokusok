# A feladat célja

A kiválasztott alkalmazás különböző módú tesztelésével más-más célunk van.

### Unit tesztek

A unit tesztekkel a program működését teszteljük. Ennek a célja elsősorban nem az, hogy
most működik e a program, hiszen ez valamilyen szinten elvárt. Azonban az kérdéses, hogy
esetleg egy módosítás esetén, hogy reagál a program a változásokra. Így ellenőrizni tudjuk, hogy
egy új funkció hozzáadásakor okozunk e valami hibát.

### CI beüzemelése

A CI ezeket a teszteket futtatja le egy pull request esetén, ami az automatizált mivolta
miatt kifejezetten hasznos. Továbbá, ha valaki egy módosítás után elfelejti tesztelni a programot
az sem tudja azt hibásan pusholni, hiszen a redszer ilyenkor jelez, hogy hiba van.

### Manuális tesztek

A manuális tesztek a felhasználó szempontjából hasznos információkat gyűjt számunkra. Itt a 
unit tesztekhez képest tényleg arra vagyunk kíváncsiak, hogy a program jól működik e, és 
hogy adott esetben a felhasználóhoz hogyan jut el a hiba, és jó e így a program működése.

### Performancia tesztek

Végül a performancia tesztek azt a környezetet szimulálják, ami a deploy után vár a szoftverre.
Itt ki kell deríteni, hogy az alkalmazás képes e ellátni a feladatát akkor is, ha egyszerre sokan 
szeretnék használni azt. Ebből is nagyon hasznos tapasztalotat lehet gyűjteni.