
# CI beüzemelése 
### Bevezetés
A CI beüzemeléséhez a github actions fülén található Node.js-es workflowt vettem alapul, az ez által generált yaml fájlt szerkesztettem.


### YAML fájl
Az eredeti yaml fájl majdnem tökéletes is volt, csak egy dolgot kellett módosítani rajta, ami az volt, hogy alapból több Node verzión is elvégzi az ellenőrzést, de ezt én nem tartottam fontosnak úgyhogy csak a 16-os verziót hagytam benne, viszont ezt a későbbiekben könnyen ki lehet bővíteni más verziókkal.

### Package.json
A yaml fájlban a tesztek futtatásához az npm test skriptet használta úgyhogy ezt írtam felül a `mocha test --recursive` parancsra ami a test könyvtárban és annak alkönyvtáraiban lévő teszteket futtatja le

### Összefoglalás
Miután a test mappában lettek kész tesztek onnantól minden pull requestnél és master branchen végzett commitnál látszott az actions fülön, hogy lefutottak a tesztek és, hogy sikeresek voltak-e.