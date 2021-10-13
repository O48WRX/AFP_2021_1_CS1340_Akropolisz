# Tesztjegyzőkönyv

## 1. Bevezetés
A tesztelés az alkalmazás fejlesztés egyik, hanem a legfontosabb mellékteendője,
mivel ezekből a tesztekből derül ki, hogy mik vannak teljesen készen, és miket kell a későbbiekben javítani.
Ezeket a teszteket a fejlsztők hajtják végre, általában a saját részükön, hogy pontosan tudják,
hogy hol keressék az esetleges hibákat.

## 2. Tesztelési terv hatóköre, célja:
Ahogy a bevezetésben is leírtuk, a tesztelés legfontosabb célja, hogy a fejlesztők kiszűrjék a program hibáit
és azokat minnél hamarabb és minnél hatékonyabban javítsák ki.
A frontend fejlesztők a frontend részt nézik át, a backend fejlesztők pedig a saját, backend részüket tesztelik.

## 3. Tesztek
A tesztelést és hibajavítűst mind a 4 fejlesztőre kiosztottuk, a saját terület-felelősségük alapján

## 3.1 Kardos Zsolt - O48WRX

### Sikeres Tesztek

| Sorszám | Teszt neve | Leírása |
|---|---|---|
| 1. | **Logikai teszt** | A program logikai hátterének sikeres működéstesztje. |
| 2. | **Függvény teszt** | A program függvényeinek működésének és helyes meghívásának sikeres tesztje. |
| 3. | **Függvény-szabály összefüggés tesztje** | A függvény logikai összefüggésének tesztelése a játékszabályzattal. |
| 4. | **Gombok funkcionális tesztje** | A gombok sikeres függvényes összekötése után az adott gombok sikeres működéstesztje jött. |
| 5. | **Javscript formok tesztje** | A tétmegadáshoz szükséges form értékmegadási és logikai, sikeres tesztje. |

### Hibás tesztek

| Sorszám | Teszt neve | Leírása |
|---|---|---|
| 1. | **Crash Course teszt** | A programnak abszurd értékeket adtunk, esetleges hibák fellelésére, ám ezzel nem jutottunk sokra és megzavaródott a logika. Ez a hiba később ki lett javítva. |
| 2. | **Crash Course 2 teszt** | A program gombjait, véletlenszerűen nyomkodjuk, emiatt összezavaródott a logika, ez a hiba a teszt alatt ki lett javítva. |
| 3. | **Kiértékelés teszt** | A program logikájában, a kiértékelés megírásakor végtelen ciklus keletkezett, emiatt volt szükség erre a tesztre. A hiba még a tesztelés során ki lett javítva. |

## 3.2 Riczkó Henrik - D5GPJ6

### Sikeres Tesztek

| Sorszám | Teszt neve | Leírása |
|---|---|---|
| 1. | **Firefox böngésző teszt** | A program kinézete Firefox böngészőben megfelel az elvártaknak. |
| 2. | **Chrome böngésző teszt** | A program kinézete Chrome böngészőben szintén megfelel az elvártaknak. |
| 3. | **Felbontás teszt** | A program különböző felbontásokban is megjelent megfelelően. |


### Hibás tesztek

| Sorszám | Teszt neve | Leírása |
|---|---|---|
| 1. | **Mobil teszt** | A program telefonokon nem jelent meg megfelelő módon, ez később javítva lett de a gombok kisebb készülékeken túl kicsik és nehezen olvashatóak. |
| 2. | **Grafikai hibák** | A felületen megjelenő ikonok nem jelentek meg rendesen de ez javítva lett. |
| 3. | **Animáció hibák** | A blackjack felírat animációja akadozva mozgott néhány böngészőben. |

## 3.3 Balogh Mihály Viktor - GUFVXA

### Sikeres Tesztek

| Sorszám | Teszt neve | Leírása |
|---|---|---|
| 1. | **Megfelelő elkülönítés** | A program felületén a szabályzat és a játék részei jól elkülöníthetőek. |
| 2. | **Megjelenési mechanika** | A weblapon rendezetten jelennek meg a program elemei. |
| 3. | **Személyzet** | A weblappal foglalkozó csapattagok feltüntetése. |


### Hibás tesztek

| Sorszám | Teszt neve | Leírása |
|---|---|---|
| 1. | **Felületi hiba** | A program felületén nem megfelelően jelentek meg a csapattagok. |
| 2. | **Szöveg hiba** | A weblapon az Impresszum cím rossz pozíción foglalt helyet. |

## 3.4 Hadobás Dávid - TB3376

### Sikeres Tesztek

| Sorszám | Teszt neve | Leírása |
|---|---|---|
| 1. | **Crash Course teszt** | A program gombjait, véletlenszerűen nyomkodtuk, de nem dobott abszurd végeredményt, a programfolyás normálisan folyt tovább. |
| 2. | **Gombfunkció teszt** | Korábban a gombok hatására a függvények nem hívták meg egymást, ennek javítása után a teszt sikeres volt. |
| 3. | **A játék végességének tesztje** | Ebben a tesztben a cél a játékbeli összeg 0-ra vitelével próbálkoztunk meg, hogy teszteljük a végességét, sikerrel. |


### Hibás tesztek

| Sorszám | Teszt neve | Leírása |
|---|---|---|
| 1. | **Crash Course 2 teszt** | A programnak határértéken kívüli értékeket adtunk tétnek, amit nem fogadott el, újból feldobta a tétbekérő ablakot. |
| 2. | **Kiíratási teszt** | A program egyes esetekben nem írta ki az ellenfél kártyáit, amikor erre szükség lett volna, ez a hiba ki lett javítva. |
