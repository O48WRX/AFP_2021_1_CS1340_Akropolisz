# Követelmény Specifikáció

## 1. Áttekintés
A projektünk egy online Blackjack játék lenne, ami ingyenes, nem igényel regisztrációt, valamint letisztult felülettel rendelkezik.
A megvalósításához HTML+CSS-t és Javascriptet szeretnénk felhasználni.

## 2. Jelenlegi helyzet
Nagyon sok online Blackjack játék van, és mellesleg jelentős része nem ingyenes, hanem már mikrotranzakciós szerencsejáték.
Úgy éreztük, hogy nincs egy igazán letisztult, könnyen érthető vagy éppen könnyen kezelhető és ingyenes verzió.
Elég sok oldalon, ahol ingyenes is, még a regisztráció is elvárt, valamint egyes helyeken a weboldal dizájnját is giccsesnek vagy túlbonyolítottnak gondoltuk.
Többek között egy olyan szolgáltatást akarunk nyújtani, ahol még az is, aki szeret szerencsejátékokkal játszani gyakorolhat vagy megértheti a játék szabályait és taktikáit.

## 3. Vágyálomrendszer
A csoportunk célja, hogy létrehozzunk a projekt keretében egy olyan Blackjack játékot egy weboldalon, ami regisztrációmentes, ingyenes és letisztult (nem túlbonyolított dizájn), valamint elmagyarázza a szabályokat a játék oldalán a felhasználó számára.
A játékban a felhasználó próbára teheti szerencséjét és logikus/matematikai gondolkodását és játszhat egy virtuális dealer (a program) ellen.
Az oldal megadja a kezdő tétet, amivel elindul a felhasználó és megjeleníti, ha az esetleg változna, valamint megjeleníti az eddig nyert összeg értékét is.
Ha a felhasználó kifogyna az összegből, amit kapott és/vagy nyert, akkor újra kell kezdenie a játékot és a nyereményszámláló lenullázódik.

## 4. Funkcionális követelmények
A projekt funkcionálisan nem bonyolult vagy terjengős. Egy böngésző szükséges a használatához, ami támogat Javascriptet, és kliens oldalon fut.
Rendelkezik egy, a felhasználó rendelkezésére álló összeg számlálójával, ha nulla, vagy az alá esik, véget ér a játék és újra kell kezdeni,
továbbá egy, a jelenlegi játék alatt nyert összeg számlálójával, a játékosnak feltünteti a kiosztott lapokat és szintúgy a virtuális dealer lapjait.

## 5. Rendszerre vonatkozó törvények, szabványok, ajánlások
++TODO LISTÁZÁS++
A projektünket az ismert kaszinó Blackjack vagy 21 szabályai alapján készítjük el. A projekt nem tartalmaz pénzfeltöltési vagy kezelési funkciót,
nem folyik át rajta pénz semmilyen módon, valamint nem igényel regisztrációt vagy bármiféle adatot a felhasználótól, így egy közönséges játéknak
vagy gyakorló játéknak/demo játéknak nevezhető, éppen ezért mondhatni, hogy nem ütközik semmilyen jogszabályba, valamint nem használunk fel jogszabályt fejlesztési alapnak.

## 6. Jelenlegi üzleti folyamatok modellje
++TODO MODELL++
Manapság az online szerencsejáték oldalakra szükséges minimum pénzösszeg, és szinte nem is nyújtanak gyakorlási vagy bemutatót a felhasználók számára, hanem
egyből a mélyvízbe dobják. Ezek az oldalak regisztrációt igényelnek személyes adatokkal, valamint bizonyos esetekben lehet, hogy az oldalak bonyolultak és
nehezen kezelhetőek felhasználók számára és így nem tudják kiélvezni a játékot vagy egyáltalán belekezdeni. Ez sokakat elijeszt az ilyesféle online játékok használatától.

## 7. Igényelt üzleti folyamatok
Projektünkkel igyekszünk egy letisztult weboldalon lévő játékot nyújtani, ami könnyen elérhető böngészőből, nem igényel regisztrációt és egyéb adatot a felhasználótól,
valamint nem igényel financiális beruházást sem a játék elkezdéséhez, vagy további játszáshoz sem. A projekt a Blackjack/21 megszokott szabályai alapján működik, emiatt nem kell változtatnunk rajta.
A szolgáltatásunk könnyen és komfortosan kezelhetőségével szeretnénk kitűnni a tömegből, valamint azzal, hogy nem igényel személyes adatokat.
Manapság a személyes adatok megadása egy oldalon sok veszélynek teszi ki adatainkat, bizonyos data leak-ek során olyan emberek kezébe is juthatnak adataink,
akik nem a legális térben mozognak, ezt szeretnénk kiküszöbölni azzal, hogy egyáltalán nem kérünk semmiféle regisztrációt és semmilyen személyes adatot a
felhasználóktól, továbbá kliens oldalon fut, így még egy szerver sem kezel semmit, amit a felhasználó tudta nélkül küldene az eszköze.

## 8. Fogalomtár
- Blackjack: Sokak által ismert kaszinójáték, elterjedt neve még a huszonegy.

- Dealer: Angolul az 'osztó'-t jelenti.

- Data leak: Adatszivárgás. Amikor egy szervezettől, vagy cégtől kiszivárognak adatok. Jelen kontextusban olyan adatszivárgásról van szó, ami a felhasználók személyes adatainak kiszivárgását jelenti.
Általában csak e-mailek és jelszavak szoktak kiszivárogni, de súlyosabb esetek is léteznek.

