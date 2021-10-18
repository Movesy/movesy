# 1. hét
Kiválasztottuk, hogy melyik témán fogunk dolgozni. A Freelancer fuvarozó appra esett a választásunk. Ezek után megbeszéltük hogy ki, melyik részén fog dolgozni a projektnek. Matyi és Tibi az Androidos részen, Peti az admin felületen, a két Tomi pedig a backenddel fognak foglalkozni.
Az alapkövetelményeket is átbeszéltük, ehhez egy Google Docs filet csináltunk, ami [itt](https://docs.google.com/document/d/1WAVCBwguPUmWpYPLFZEydfawg5oTvkpmgPByFnkI8vU/edit) érhető el.
# 2. hét
Megterveztük az app kinézetét telefonon és weben is, ehhez a draw.io oldalt használtuk.
![A tervet itt lehet megnézni](https://raw.githubusercontent.com/Movesy/movesy/main/docs/mockup.png)
Létre is hoztunk a projektnek egy github organisationt, amiben létrehoztunk 4 repositoryt. Egyet-egyet a haladásunk követéséhez, az admin felülethez, az androidos részhez és a backendhez. Ez [itt](https://github.com/Movesy) érhető el.

# 3. hét

Megterveztük az app adatmodelljét, amihez ismét a draw.io-t használtuk. Itt kicsi problémát jelentett, hogy a vonalakat nehéz volt mozgatni, ami meghosszabbította a munkát. Ezen túl nehézséget okozott eldöntenünk hogy az entitások közötti kapcsolatot hogyan jelezzük a modellen úgy, hogy az a lehető legolvashatóbb legyen. Az első lehetőség ami szóba jött az az, hogy csak feltüntessük a kapcsolatban lévő entitás ID-ját attribútumként, a másik meg az, hogy az ER diagram szerinti kapcsolattal kössük őket össze. A végleges modell így néz ki:

![](https://github.com/Movesy/movesy/blob/main/docs/datamodel_old.png?raw=true)

Elkezdtük összerakni az [endpointokat](https://github.com/Movesy/movesy/blob/main/docs/endpoints.txt) szövegszerkesztővel, amik közben rájöttünk, hogy nem tudjuk hogyan kellene rendesen kezelni az adminokat. Az egész bejelentkezés témakör kicsit homályos egyelőre.
Ezekkel a célunk az volt, hogy könnyebben össze tudjuk rakni Swaggerben az [API dokumentációját](https://app.swaggerhub.com/apis/Mov/MovesyAPI/1.0.0#/). Ezzel egész sok időnk elment, mert meg kellett tanulnunk hogy hogyan működik a Swagger és hogyan kell a generáláshoz szükséges yaml filet elkészíteni. Ha a link nem elérhető vagy hibás/régi kódot mutat, akkor [itt](https://pastebin.com/jJPYBZ53) érdemes megnézni.


Peti az Angularral is elkezdett foglalkozni, ehhez a haladásinaplója [itt található](https://github.com/Movesy/movesy-admin/blob/main/haladasinaplo.md).

# 4. hét

Frissítettük az API dokumentációt, mivel az adatmodellt a megbeszéltek alapján megváltoztattuk. Arra a döntésre jutottunk, hogy egy táblában lesznek tárolva a userek is és a transporterek is és lesz egy plusz 'role' adattagjuk, így könnyebben lehet további szerepekkel bővíteni a modellt. Ezeken felül a packageknek a 'width', 'height', 'depth' helyett csak egy enum típusú 'size' adattagja lesz, ugyan így a transportereknek is, ami azt jelzi, hogy mekkora csomagot képesek elszállítani.
A frissített adatmodell itt látható:

![](https://github.com/Movesy/movesy/blob/main/docs/datamodel.png?raw=true)

A frissített Swaggeres API dokumentáció [itt](https://pastebin.com/Q0BdZpV8) érhető el.

- [Admin haladási napló](https://github.com/Movesy/movesy-admin/blob/main/haladasinaplo.md)
- [Backend haladási napló](https://github.com/Movesy/movesy-backend/blob/master/README.md)
- [Mobil haladási napló](https://github.com/Movesy/movesy-mobile)

Az endpointokat jelenleg [így](https://github.com/Movesy/movesy-backend/blob/master/movesy_backend-openapi.yaml) lehet elérni.
