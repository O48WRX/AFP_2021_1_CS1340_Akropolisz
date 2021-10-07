# ﻿Rendszerterv

## 1.Rendszer célja
A rendszer célja, hogy a felhasználó próbára tegye szerencséjét, valamint tudását a program ellen, a megszokott Blackjack/21 szabályai szerint költségmentesen.
Fontos, hogy a játékos könnyen el tudjon igazodni a felületen, ezért egy minimalista felhasználói felületet kap a program.
Egyetlen szerepkör van a program használatánál, a felhasználó, de az csak a játék végigvezetéséhez szükséges funkciókhoz ad hozzáférést,
a program működésének megváltoztatásához, a kódhoz nem fér hozzá közvetlenül.
Az alkalmazás webes felületen lesz elérhető, ezért arra törekszünk, hogy minél több böngészővel legyen kompatibilis.
A játékos minden nyert kör után a tétje dupláját kapja vissza, vesztett kör után pedig elveszti a tétjét, addig megy a játék, ameddig
ki nem fogynak a tétnek felrakható összegből, vagy fel nem adják a játékot.

## 2.Projekt terv
	A projektet weblapra fejlesztjük front- és backend segítségével. Az elkülönített feladatokon más-más emberek dolgoznak.
	Frontend fejlesztése HTML/CSS segítségével
	Frontend felelősök: Riczkó Henrik (D5GPJ6), Balogh Mihály(GUFVXA)
		-HTML, CSS és oldal dizájn

	A feladat célja, hogy egy letisztult, könnyen kezelhető, igényes weblapot nyújtson a felhasználó számára.

	Backend felelősök: Kardos Zsolt(O48WRX), Hadobás Dávid (TB3376)
		-Javascript és tesztelés

	Feladatuk a háttérben működő programok megírása, randomizálás, JavaScript kód, és az eredmény kiértékelés.
	
## 3. Üzleti folyamatok modellje
![Rendszerterv_ÜFM](https://user-images.githubusercontent.com/82752886/135045846-c1ea8490-7fe1-4f7f-b73f-8c2b4a14c746.png)


## 4.Követelmények
	- Webes megvalósítás.
	- A rendszer fejlesztése HTML/CSS valamint JavaScript segítségével történik.
	- A weblap felépítése, valamint dizájnolása a HTML/CSS nyelv implementálásával valósítandó meg.
	- A weboldal használatához egy egyszerű böngészőre van szükség.
	- Megszakításmentes játékmenet.

## 5.Funkcionális terv
Rendszerszereplők:
	- Játékos: Rendszerünknek nincs más szereplője, csak a játékos, mert nincs értelme több, pl. egy admin szereplő hozzáadásának.
A játékos ki tudja választani, hogy a jelenlegi lapokra ráhúz, tétet rak, dupláz, vagy kiszáll.

## 6. Fizikai környezet
    A rendszer fejlesztése HTML/CSS valamint JavaScript segítségével történik.
        A weblap felépítése, valamint dizájnolása a HTML/CSS nyelv implementálásával valósítandó meg.
    A weboldal használatához egy egyszerű böngészőre van szükség.
    A rendszer bármilyen operációs rendszeren és böngészőben haszálható lesz, valamint telefonról is.

## 7. Archtitekturális terv
A rendszerhez mindössze egy webböngészőre van szükség, amely képes JavaScript kódot futtatni. Mivel az egész a kliens oldalon fut, akár a HTML fájl megnyitásával futtatható a játék alkalmazás.

## 8. Tesztterv
Az alkalmazás elkészítése során szükség van a folyamatos tesztelésre.
Tesztelni kell a gombok működését, valamint a pontszám változását, ha a játékos vagy a gép nyer, illetve az új játék kezdésénél a pontszám nullázását.

Unit teszt: 
	2021.10.06: Metódusok működése és működésének biztosítása teszt során megtörtént és hiba nélkül lefutott. - Kardos Zsolt
Alpha teszt:
	2021.10.07: A projektet leteszteltük Mozilla Firefox, Google Chrome és Microsoft Edge környezetben, kisebb vizuális torzulással de működését megőrizte. - Kardos Zsolt, 	Riczkó Henrik, Hadobás Dávid
Béta teszt:
	2021.10.07: A projekt letesztelése különböző böngészőkben, különböző felbontásokban és telefonon, kisebb vizuális torzulás de a funkciók működése megmaradt. - Balogh Mihály 

## 9. Telepítési terv
Az alkalmazás futtatásához egy általános felhasználású böngészőre van szükség, nem igényel külön telepítést.

## 10. Karbantartási terv
Az alkalmazás bővítési lehetőségét fenntartjuk. A későbbiekben többjátékos mód is hozzáadható.

## 11. Implementációs terv
A felület HTML és CSS nyelven fog készülni valamint JavaScript-et is felhasználunk az alkalmazás készítéséhez. A jobb átláthatóság és a továbbfejleszthetőség érdekében elkülönítve szeretnénk kezelni ezeket a technológiákat és utólag kapcsoljuk össze őket. 
