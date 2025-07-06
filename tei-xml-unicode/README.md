# A Bizánci Szövegforma TEI-XML fájljai

Ez a mappa az Újszövetség teljes szövegét tartalmazza XML-formátumban (a `BYZ` almappában), valamint könyvenként is.  
Ezek a fájlok **nem tartalmaznak ékezeteket és szövegvariánsokat** – kizárólag a Bizánci Szövegforma főszövegét képviselik.

A fájlokat egy szkript konvertálja, amely a `scripts` mappában található (lásd ott a részleteket).  
A forrásfájlok a `source/Strongs` mappában vannak.

## A CollateX használata

A CollateX szoftver letölthető erről az oldalról:  
https://collatex.net/download/

Tegyük fel, hogy össze szeretnéd hasonlítani a P66 kódexet a János evangéliuma 1. fejezetének bizánci szövegével.  
A P66 transzkripciója letölthető innen (az INTF adatbázisból):  
https://ntvmr.uni-muenster.de/community/vmr/api/transcript/get/?docID=10066&indexContent=John%201&pageID=ALL&format=teiraw

A Bizánci szöveg itt, ebben a mappában található.

Ehhez a bemutatóhoz előkészítettünk egy TEI-fájlt, amely csak a János 1. fejezetet tartalmazza.  
Ez megtalálható itt: [demo_john_1.xml](assets/demo_john_1.xml)  
(Ha a teljes könyvön próbálod futtatni a CollateX-et, az sok időt vehet igénybe.)

Mentsd le a fájlokat például `p66.xml` és `demo_john_1.xml` néven.

Ezután futtasd a CollateX-et az alábbi paranccsal:

```bash
java -jar collatex-tools-1.7.1.jar -xp '//w' -xml -f csv -t demo_john_1.xml p66.xml > collation.csv
```

![](assets/coll.png)
