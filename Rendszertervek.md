# ﻿Rendszerterv

## 1.Rendszer célja
A rendszer célja, hogy a játékos legyőzze a gépet a Blackjack kártyajátékban.
Ha a játékos nyer, akkor a feltett tét duplája hozzáadódik a nyert összeg számlálójához.
Ha a gép nyer, a feltett tét elvész, döntetlennél pedig visszaadódik a számlálóba. 
A játék használatához nem szükséges regisztrálni, viszont ha elhagyjuk az oldalt akkor a pontszám törlődik.
A játék az eredeti szabályok szerint megy, a 21-hez közelebbi szám nyer, azonos pontszámnál a kevesebb lap nyer, az ász pedig a többi laptól függően érhet 1-et vagy 11-et.

## 2.Projekt terv
	A projektet weblapra fejlesztjük front- és backend segítségével. Az elkülönített feladatokon más-más emberek dolgoznak.
	Frontend fejlesztése HTML/CSS segítségével
	Frontend felelősök:

	A feladat célja, hogy egy letisztult, könnyen kezelhető, igényes weblapot nyújtson a felhasználó számára.

	Backend felelősök:

	Feladatuk a háttérben működő programok megírása, randomizálás, JavaScript kód, és az eredmény kiértékelés.
	
## 3. Üzleti folyamatok modellje
![Rendszerterv_ÜFM](https://user-images.githubusercontent.com/82752886/135045846-c1ea8490-7fe1-4f7f-b73f-8c2b4a14c746.png)


## 4.Követelmények
	A rendszer fejlesztése HTML/CSS valamint JavaScript és php segítségével történik.
	A weblap felépítése, valamint dizájnolása a HTML/CSS nyelv implementálásával valósítandó meg.
A weboldal használatához egy egyszerű böngészőre van szükség.

## 5.Funkcionális terv
Rendszerszereplők:
-Játékos: Rendszerünknek nincs más szereplője, csak a játékos, mert nincs értelme több, pl. egy admin szereplő hozzáadásának.
A játékos képes kiválasztani, hogy a jelenlegi lapokra ráhúz, tétet rak, vagy kiszáll.

## 6. Fizikai környezet
    A rendszer fejlesztése HTML/CSS valamint JavaScript és php segítségével történik.
        A weblap felépítése, valamint dizájnolása a HTML/CSS nyelv implementálásával valósítandó meg.
    A weboldal használatához egy egyszerű böngészőre van szükség.
    A rendszert bármilyen operációs rendszeren és böngészőben haszálható lesz, valamint telefonról is.

## 7. Archtitekturális terv
A rendszerhez mindössze egy webböngészőre van szükség, amely képes JavaScript kódot futtani. Mivel az egész a kliens oldalon fut, akár a HTML fájl megnyitásával futtatható a játék alkalmazás.

## 8. Tesztterv
Az alkalmazás elkészítése során szükség van a folyamatos tesztelésre.
Tesztelni kell a gombok működését, valamint a pontszám változását, ha a játékos vagy a gép nyer, illetve az új játék kezdésénél a pontszám nullázását.

## 9. Telepítési terv
Az alkalmazás futtatásához egy általános felhasználású böngészőre van szükség.

## 10. Karbantartási terv
Az alkalmazás bővítési lehetőségét fenntartjuk. A későbbiekben többjátékos mód is hozzáadható.
