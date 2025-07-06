# Az Újszövetség eredeti görög nyelven: Bizánci szövegforma

![GitHub release (latest by date)](https://img.shields.io/github/v/release/ByzTxt/byzantine-majority-text?style=for-the-badge)

Üdvözlünk **Dr. Maurice A. Robinson** görög szövegeinek hivatalos GitHub-oldalán, amely tartalmaz változatokat, morfológiai elemzést és Strong-számokat.

Ez a repozitórium tartalmazza a **Robinson–Pierpont-féle görög Újszövetség** kiadását, az eredeti görög nyelven, **bizánci többségi szövegként**.
A szöveg jelenlegi formája 2023. július 20-i állapotot tükrözi, és az **RP2018 (Robinson–Pierpont 2018)** kiadást képviseli (néhány kisebb módosítással a kritikai apparátusban).

A 2005-ös kiadás PDF formátumban **szabadon letölthető** az Internet Archívumból [innen](https://archive.org/details/newtestamentrobinsonpierpontbyzantine/).
A 2018-as kiadás letölthető [erről a linkről](https://archive.org/details/robinson-pierpont-2018-gnt-edition).
**Minden gyakorlati célra** az **RP2018** kiadás ajánlott az RP2005 helyett (részletek lentebb olvashatók).
További anyagok letölhetők innen: [https://www.byzantinetext.com](https://www.byzantinetext.com).

Elolvasható **Robinson professzor esszéje** is, amelyben a bizánci szövegforma elsőbbsége mellett érvel:
[itt olvasható](https://byzantinetext.com/wp-content/uploads/2016/11/editions-rp-11-appendix.pdf).
Az esszé **spanyol fordítása** is szabadon letölthető [innen](https://archive.org/details/libro-robinson-traducido/LIBRO%20ROBINSON%20TRADUCIDO/).
Az esszé **sima szöveges formában** is megtalálható a repozitórium `essay` nevű mappájában.

## Elérhető változatok:

1. Elemzett változat BETA formátumban, ékezetek nélkül (`source/Strongs` mappa).

2. Teljes változat BETA formátumban, ékezetekkel, hehezettel, dierezissel, ióta alsóindexekkel és kritikai apparátussal, amely tartalmazza a bizánci változatokat, valamint a Nestle-Aland és *Editio Critica Maior* eltéréseket (`source/CCAT` mappa).

3. Unicode változatok CSV formátumban (`csv-unicode` mappa; további információ a `README`-ben).

4. TEI-XML változatok (`tei-xml-unicode` mappa) az [IGNTP XML transzkripciós iránymutatásainak](http://epapers.bham.ac.uk/1892/5/IGNTP_XML_guidelines_1-5.pdf) megfelelően. Ezek a [CollateX](https://collatex.net/) szoftverrel összevethetők a *Editio Critica Maior*-ban használt [Münster INTF transzkripciókkal](https://ntvmr.uni-muenster.de/home).

Az **1. és 2. pontban szereplő hivatalos fájlokat Robinson professzor készítette**. A többi változat a `scripts` mappában található eszközökkel generált. Robinson professzor fájljai a hiteles alap.

Ha kérdésed van vagy hibát találsz, nyiss egy GitHub issue-t vagy pull requestet. A karbantartók megvizsgálják, és ha kell, kapcsolatba lépnek Dr. Robinsonnal.

## Verzók

A Bizánci Szövegforma két hivatalos nyomtatott kiadása az **2005-ös és 2018-as**. Ezek PDF-ben és nyomtatásban is széles körben elérhetők. Ez a repozitórium mindkettő adatait tartalmazza. Mivel azonban 2022 előtt nem volt hivatalos verzókövetés, a 2005 és 2018-as szöveg pontos visszakeresése nem egyértelmű a Git-történet alapján.

**Erősen ajánlott** a `3.x.x` verzók használata a korábbiak helyett az alábbi okok miatt:

* A `1.0.0` előtti verzókban **nem volt Unicode-változat**. A forrásfájlok sajátos BETA-kóddal készültek.

* A `1.0.0` verzóban megjelent ugyan Unicode-konvertáló, de hibásan működött. Ezeket a hibákat a `2.0.3` javította. Ha valaki az RP2005-höz legközelebbi Unicode szöveget keres, a `2.0.3` kiadást használja. A `2.0.3` előtti Unicode fájlok hibásak (de a BETA-kódos forrás nem változott a `1.0.0` és `2.0.3` között, és ezek hivatalosak, mivel közvetlenül Robinson professzortól származnak).

* A `3.0.0` bevezette az RP2018 szöveget kisebb frissítésekkel. Robinson professzor **kifejezett ajánlása szerint** az RP2005 **nem használandó** az RP2018 helyett, mert az RP2005-ben "számos ékezet-, lehelet- és írásjelhiba volt (a NA27 fájl alapján való átümás miatt, ahol csak a Bizánci szöveg eltért, azt módosították)". A 2018-as kiadás ezeket kijavította. A szöveg csak "igen kevés helyen" változott, de az apparátust is frissítették, hogy tückrözze az NA28 és ECM eltéréseit az általános levelekben és az Apostolok Cselekedeteiben. Fontos: a **hangjel nélküli** szöveg rendkívül stabil maradt RP2005 és RP2018 között.

## Archiválás

A repozitórium tükörmásolata elérhető a [Software Heritage Archívumban](https://archive.softwareheritage.org/browse/origin/directory/?origin_url=https://github.com/byztxt/byzantine-majority-text).

## Szerzői jog

A mappában található összes kód és szöveg **közkinccsé** lett nyilvánítva (Public Domain).
