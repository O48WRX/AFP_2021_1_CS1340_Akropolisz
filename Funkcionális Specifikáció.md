# Funkcionális Specifikáció

## 1. Áttekintés

Egy olyan kliensoldali alkalmazást fejlesztünk, ami a kaszinókban elterjedt, híres Blackjack/21 kártyajátékot nyújtja
a felhasználók számára ingyenesen, regisztrációmentesen és személyes adatok felhasználása nélkül. 
Lehetőségünk van ezt a játékot egy szélesebb körben terjeszteni, megismertetni és gyakoroltatni azokkal,
akiknek másképp nem lenne könnyen elérhető módja erre. 
Az alkalmazást bármikor el lehet érni böngészőből, letöltést nem igényel, valamint mivel kliens-oldalon fut, 
így még a szerver hibák lehetősége sem áll fenn, hogy megállítsa a felhasználót a játék élvezésében. 
A játék a megszokott Blackjack/21 szabályai szerint fog működni, amivel a felhasználó próbára teheti szerencséjét.


## 2. Jelenlegi helyzet

A megrendelő szeretne egy letisztult oldallal rendelkező, ingyenes, letöltést nem igénylő Blackjack gyakorló webes alkalmazást, ami nem szerverfüggő. 
A rendszer lehetőséget nyújt azoknak, akiknek nem áll módjában fizetni hasonló szolgáltatásokért és/vagy nem hajlandóak megosztani adataikat, 
azzal veszélynek kitéve azokat, esetlegesen pedig csak egy gyakorlófelületet keres, ami elmagyarázza a játék szabályait.

## 3. Jelenlegi üzleti folyamatok modellje

Manapság minden ilyen elterjedt szerencsejáték, ami online megtalálható igényel regisztrációt és egy összeg prémium befizetését a játék elkezdéséhez.
Ez leszűkíti a lehetséges felhasználók halmazát, sőt teljesen elijeszt embereket a szerencsejátékoktól. 
Lehetséges felhasználók alternatívákat keresnek, de ha találnak is, akkor általában olyat, ami viszont személyes adatok megadásával játszható csak. 
Ez esetleges data-leak esetén adatlopáshoz vezethet, ami negatív hatással van a felhasználó bizalmára és a cég megbízhatóságára, hírnevére is. 
Általában ezekhez az online szerencsejátékokhoz nem található az adott oldalon egy útmutató, vagy szabályzat sem. 
Ezeket a hibákat ki lehetne küszöbölni azzal, hogy egyrészt ingyenesen elérhető a szolgáltatás, nem igényel regisztrációt
(ezzel kiküszöbölve az esetleges adatlopás lehetőségét), valamint kliens oldali futással érhető el, hogy a szolgáltatás ne függjön a szerver futásától, 
és mindig elérhető legyen a felhasználó számára.

## 4. Igényelt üzleti folyamatok modellje. (TO DO: rajz)

Azért, hogy egy komfortosabb és kölcsönös megbízást érjünk el a felhasználókkal, egy olyan szerencsejáték szolgáltatást hoznánk létre, ami:
	-Nem igényel letöltést, így nem áll fenn a lehetőség, hogy a tárolt adatokhoz egyáltalán hozzáférjen.
	-Nem igényel regisztrációt, így a személyes adatok is biztonságban maradnak.
	-Nem igényel kezdőösszeg befizetést sem, és további költségeket sem.
	-Nem szerveroldalon futtatjuk a szolgáltatást, így elérhető a felhasználó számára, szinte bármikor, szervertől való függés nélkül.
	-A játékhoz szükséges információkat és szabályokat közli a felhasználóval.
	
## 7. Használati esetek

A projektünk a szabványos Blackjack/21 szabályait követi (lásd: 9. Forgatókönyv). 
A szolgáltatás teljesen ingyenes és nem igényel regisztrációt, 
ezáltal nem zárjuk el a felhasználók nagy részét magunktól és adataikat nem tesszük ki a kiszivárgás veszélyének (data-leak), 
valamint olyanoknak is lehetőséget adunk, akik esetleg nem tudnák megfizetni a szükséges kezdőösszeget a játékoknál.
Egy könnyen kezelhető, letisztult, átlátható dizájnnal megfelelünk a könnyen felfoghatóság és átláthatóság feltételének. 
Nem futtatunk szerveroldalon kódot, ezáltal eleget teszünk a folyamatos elérhetőség feltételének.

## 8. Képernyő tervek

![Funk drawio](https://user-images.githubusercontent.com/82752886/135749142-efffc873-8187-4163-84a0-3c5b748e40e6.png)

## 9. Forgatókönyv

Szereplők: A felhasználó és a futó webes alkalmazás.
A felhasználó megnyitja a böngészőjében a szolgáltatást, majd kap egy virtuális kezdőösszeget, 
amivel téteket rakhat a klasszikus Blackjack játékban. 
Ha a felhasználó nem ismeri a játékot, akkor van lehetősége elolvasni a szabályokat és tippeket. 
A felhasználó a tét letétele után kapja meg a kártyáit (2 kezdőkártyát), 
majd a dealer is kioszt magának 2 kártyát, 
ezután eldöntheti, hogy meg akarja-e tartani a kártyáit vagy bedobni, ezután eldöntheti, 
hogy marad-e a jelenlegi kártyaleosztással vagy szeretne több kártyát hívni. 
Hívás esetén, ha a kártyák túlmennek a 21 értéken összegezve, 
akkor a felhasználó vagy a dealer elveszti a kört, ezzel a felrakott tétet is. 
A nyertes felhasználó visszanyeri a felrakott tét dupláját. 
A dealernek kötelező megállni, ha 17-es összeget húz. A dealer nem tud kifogyni a pénzből, 
de ha a felhasználó elveszíti az összes pénzét, 
akkor újra kell kezdenie a játékot és elveszíti az össznyeremény számlálóján látható számot és az lenullázódik. 
A minimum tét növekedik a rendelkezésre álló pénz alapján. A játék mint folyamat a végtelenségig tarthat,
ha a felhasználó ügyes és jól játszik.

## 10. Funkció-követelmény megfeleltetés

A projektünk az ismert Blackjack/21 szabályai alapján fog működni, így az azáltal előírt funkciókat tartalmazni fogja a projekt, 
ezzel eleget téve a szerencsejáték követelménynek.

## 11. Fogalomszótár

Dealer: Kártyaosztó angolul.
data-leak: Adatszivárgás.
