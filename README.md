# 1. hét
Kiválasztottuk, hogy melyik témán fogunk dolgozni. A Freelancer fuvarozó appra esett a választásunk. Ezek után megbeszéltük hogy ki, melyik részén fog dolgozni a projektnek. Matyi és Tibi az Androidos részen, Peti az admin felületen, a két Tomi pedig a backenddel fognak foglalkozni.
Az alapkövetelményeket is átbeszéltük, ehhez egy Google Docs filet csináltunk, ami [itt](https://docs.google.com/document/d/1WAVCBwguPUmWpYPLFZEydfawg5oTvkpmgPByFnkI8vU/edit) érhető el.
# 2. hét
Megterveztük az app kinézetét telefonon és weben is, ehhez a draw.io oldalt használtuk.
![A tervet itt lehet megnézni](https://raw.githubusercontent.com/Movesy/movesy/main/docs/mockup.png)
Létre is hoztunk a projektnek egy github organisationt, amiben létrehoztunk 4 repositoryt. Egyet-egyet a haladásunk követéséhez, az admin felülethez, az androidos részhez és a backendhez. Ez [itt](https://github.com/Movesy) érhető el.

# 3. hét

Megterveztük az app adatmodelljét, amihez ismét a draw.io-t használtuk. Itt kicsi problémát jelentett, hogy a vonalakat nehéz volt mozgatni, ami meghosszabbította a munkát. Ezen túl nehézséget okozott eldöntenünk hogy az entitások közötti kapcsolatot hogyan jelezzük a modellen úgy, hogy az a lehető legolvashatóbb legyen. Az első lehetőség ami szóba jött az az, hogy csak feltüntessük a kapcsolatban lévő entitás ID-ját attribútumként, a másik meg az, hogy az ER diagram szerinti kapcsolattal kössük őket össze. A végleges modell így néz ki:

![](https://github.com/Movesy/movesy/blob/main/docs/datamodel.png?raw=true)

Elkezdtük összerakni az [endpointokat](https://github.com/Movesy/movesy/blob/main/docs/endpoints.txt) szövegszerkesztővel, amik közben rájöttünk, hogy nem tudjuk hogyan kellene rendesen kezelni az adminokat. Az egész bejelentkezés témakör kicsit homályos egyelőre.
Ezekkel a célunk, hogy könnyebben össze tudjuk majd rakni Swaggerben az [API dokumentációját](https://app.swaggerhub.com/apis/Mov/MovesyAPI/1.0.0#/).


Peti az Angularral is elkezdett foglalkozni, ehhez a haladásinaplója [itt található](https://github.com/Movesy/movesy-admin/blob/main/haladasinaplo.md).

