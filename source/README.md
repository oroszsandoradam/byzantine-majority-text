# Forrásfájlok

Ez a mappa tartalmazza a Bizánci Szövegforma forrásfájljait, amelyeket Dr. Maurice A. Robinson hozott létre és tart fenn. Ezek a fájlok tekinthetők a legvégső hivatkozási alapnak minden olyan esetben, amikor a jelen repozitóriumban szereplő Unicode-fájlokkal kapcsolatban kérdés merülne fel.

A fájlok **Betakód** formában íródtak. Ez a Betakód külsőleg eltér a `beta-code` könyvtár által alkalmazott szabványtól (amely a Unicode-átalakításhoz használt eszköz). A részletes eltéréseket a `scripts/beta_to_unicode_custom/beta_to_unicode_custom.py` állomány `standardise_beta_code()` függvényének dokumentációja és kódja tartalmazza.

A `CCAT` mappában lévő fájlok tartalmazzák az ékezeteket és változatokat, míg a `Strongs` mappában található fájlok Strong-számokat és elemzési kódokat is tartalmaznak.

## Változati kódok

A `CCAT` mappában szereplő fájlok a következő jelölés szerint tartalmazzák a változatokat:

* `N`: Nestle-Aland változat
* `B`: Bizánci változat
* `C`: NA27/28 változat
* `M`: ECM (*Editio Critica Maior*) változat
* `S`: NA27 változat
* `E`: NA28 változat

## Elemzési kódok és Strong-számok

A `Strongs` mappában szereplő fájlok Strong-számokat és nyelvtani elemzési kódokat tartalmaznak. A kódolási rendszer Dr. Robinson munkája alapján készült, eredetileg [ebben a dokumentumban (2009)](https://github.com/byztxt/robinson-documentation/blob/master/doc/PARSING.COD) rögzítve.

### Elemzési kódok

Ezek a kódok a "The Analytical Greek Lexicon" (Bagster, 1859) című mű bövített és javított változatán alapulnak. Az összevetés megtörtént Wesley J. Perschbacher "The New Analytical Greek Lexicon" (1990) művével is, amelyben több mint 600 hibát nem javítottak ki. Ezeket Robinson itt korrigálta.

Az elemzési rövidítések önálló rendszerben kerültek kidolgozásra, de hasonlóak Timothy és Barbara Friberg rendszeréhez is.

A teljes Újszövetségi igék összes alakja szerepel. A kódok az előfordulás szerinti értelmezést tükrözik. Nem állítjuk, hogy hibátlanok; az esetleges hibák bejelenthetők.

Az igék az alábbi formák egyikében szerepelnek:

1. V-idő-mód-nem
2. V-idő-mód-nem-személy-szám
3. V-idő-mód-nem-eset-szám-nem

### Rövidítések

**Idők:**

| Idő                   | Jelölés |
| --------------------- | ------- |
| Jelen                 | P       |
| Múlt idejű folyamatos | I       |
| Jövő                  | F       |
| Másodlagos jövő       | 2F      |
| Aorisztosz            | A       |
| Másodlagos aorisztosz | 2A      |
| Befejezett            | R       |
| Másodlagos befejezett | 2R      |
| Régmúlt (pluperf.)    | L       |
| Másodlagos pluperf.   | 2L      |

**Nemek:**

| Nem      | Jelölés |
| -------- | ------- |
| Férfi    | M       |
| Nő       | F       |
| Semleges | N       |

**Számok:**

| Szám   | Jelölés |
| ------ | ------- |
| Egyes  | S       |
| Többes | P       |

**Személyek:**

| Személy  | Jelölés |
| -------- | ------- |
| Első     | 1       |
| Második  | 2       |
| Harmadik | 3       |

**Igenem (igei nem):**

| Igenem            | Jelölés |
| ----------------- | ------- |
| Aktív             | A       |
| Közép             | M       |
| Passzív           | P       |
| Közép vagy passz. | E       |
| Közép deponens    | D       |
| Passzív deponens  | O       |
| Vegyes deponens   | N       |

**Módok:**

| Mód               | Jelölés |
| ----------------- | ------- |
| Kijelentő         | I       |
| Kötőmód           | S       |
| Óhajtó mód        | O       |
| Felszólító        | M       |
| infinitívusz      | N       |
| melléknévi igenév | P       |

**Egyéb:**

| Típus        | Jelölés |
| ------------ | ------- |
| Attikai alak | -ATT    |

**Esetek (csak 5 eset):**

| Eset                    | Jelölés |
| ----------------------- | ------- |
| Alanyeset               | N       |
| Birtokos                | G       |
| Részesh.                | D       |
| Tárgyeset $accusativus$ | A       |

### Strong-számok

Minden görög szó mellett szerepel a hozzá rendelt Strong-féle konkordancia-szám. Ezek alapján meghatározható a lexikai tőalapjelentés.

A jelenlegi kiadásban a Strong-számok néhol módosítva vannak, hogy jobban igazodjanak a gyakorlati tőalakhoz. Pl. az "eipon" (Strong 2036) már a "legw" (Strong 3004) gyök alá sorolt. Az "eidon" átkerült az "oraw" (3708) és "oida" (1492) alá jelentés szerint.

Az átdolgozás folyamatos. Hibabejelentések alapján javítások történnek.

### Egyes esetek megjegyzései:

* Az "h" forma a "lenni" igében ritkán fordul elő (1510, Strong 5600), de gyakori más jelentésben (pl. névmás, írásjel).
* Az "ei" lehet az "lenni" ige 2. sz. jelen (1488), de gyakrabban feltételes part.
* Az "hn" gyakori ígében (2258), de lehet névmás is.
* A "wsin" Strong szerint participium (5607), valójában subjunctivus. Lehet főnév is.
* A "hv" lehet subjunctivus vagy imperfectum, mindkettő a 1510 gyökről ered.

### Kódolási példák

| Perschbacher                       | Robinson       |
| ---------------------------------- | -------------- |
| agayopoihsai (15) aor. act. inf.   | V-AAN     <15> |
| agayopoihte (15) 2 pl. pres. s.    | V-PAS-2P  <15> |
| agayopoiountav (17) acc. pl. m. p. | V-PAP-APM <17> |
