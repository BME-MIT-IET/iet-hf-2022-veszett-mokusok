# Manuális teszt 
### Bevezetés
A manuális teszteket egy excel táblázatban készítettem el. Összesen 20-at.
A táblázat oszlopai: tesztID, teszt neve, funkcionalitása, elvért eredmény, kapott eredmény
és az ezekből adodó teszt sikeressége. Ezek a jellemzők alapján alaposan manuális teszteket készíthetünk.
A tesztekben az oldal navigációrája fektettem a hangsúlyt, ezt céloztam meg.

### Linkek tesztelése, egyszerű navigálás az oldalon
Teszteltem, hogy az oldalon linkek szempontjából megfelelően tudunk navigálni. Hova kattintuk, hova kerülünk
kérdésekre terveztem teszteket, majd értékeltem ki őket. Az összes így elvégzett teszt sikeres lett, eredményképpen 
elmondható, hogy az oldalon jól működik a linkek közti navigáció.

### Linkek tesztelése, linkek mögötti funkcionalitás
Ezeknél a teszteknél a regisztráció és a bejelntkezés mögötti logikát vizsgáltam, 
törekedtem minnél több edge case-t lefedni, tesztelni. Itt némely teszt sikerrel, sikertelen eredménnyel zárult.
Számszerűsítve, a tesztek 70%-a sikerrel zárult, 30% sikertelen volt.

### Összefoglalás
Összesítve pedig a következő eredmény született: sikeres tesztek: 80%, sikertelen: 20%
Ebből és a fentiekből az a következtetés vonható le, hogy az oldalon az egyszerű navigáció megfelelelően működik, 
de a regisztráción és a bejelentkezésen lehet, kell javítani.
