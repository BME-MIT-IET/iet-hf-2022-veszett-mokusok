# Performancia teszt 
### Bevezetés
A teljesítmény teszteknél az artillery modult használtam, mivel egyszerű
lehetőséget biztosít arra, hogy az oldalakat HTTP kérések segíttségével bejárjuk,
és módot ad arra, hogy viruálisan szimuláljuk, hogy milyen lenne, ha az
oldalt egyszerre sok felhasználó szeretné igénybe venni, és például kattintgatni szeretne rajta.


### Oldal bejárás teszt
Az eredményeket tekintve 50 kérés/másodperc esetén, ha a virtuális felhasználó az 
egész oldalon ide-oda navigál, az sem jelentett bármilyen jellegű 
problémát az oldalnak a kiszolgálás. Ami a szoftver célját bőven kielégíti.

### Fuzz teszt vagy monkey teszt 
Ebben a teszt részben azt szimuláltam, hogy milyen lenne, ha egyszerre sokan
regisztrálnának az oldalon. Ehhez a fuzzer plugint hívtam segítségül, ami 
egy olyan lehetőséget ad a kezünkbe, hogy véletlenszerű stringek segítségével
imitálni lehet a felhasználók regisztrációját. Ebben az esetben sem lépett fel probléma
az alkalmazást simán vette az akadályokat. 

### Összefoglalás
A tesztek elvégézse után kijelentketjük, hogy különösebb performancia gondokkal nem 
küzd a szoftver, ez várható is volt a Node.js és express alap miatt, de így igazolást is nyert.
