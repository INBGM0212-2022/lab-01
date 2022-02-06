# GitHub műveletek

Ebben a jegyzetben azokat a műveleteket nézzük meg, melyek szükségesek a Git tárolók további használatához.

## Új fájl hozzáadása

Ha a projekt hozzá van kapcsolva egy GitHub tárolóhoz, akkor minden új fájl pirosan jelenik meg a *Package Explorer*-ben. Ekkor alapértelmezésként megkérdezi a PyCharm, hogy a fájlt hozzáadja-e a nyomkövetéshez. Ha az adott fájlt tényleg fel szeretnéd majd tölteni a tárolóba, akkor kattints az **Add** gombra. A követett fájl zölddé válik.

Másik lehetőség: jobb klikk a fájl nevére (vagy több kijelölésére) > **Git > Add**

## Módosítások mentése (`commit`)

Időnként érdemes a módosításokat menteni, amolyan mentési pontot létrehozva.

```
Git > Commit
```

A felbukkanó ablak mutatja a mentett és a  mentetlen módosításokat, azokat ki lehet választani. Az ablak alsó részében lehet egy módosításokat leíró üzenetet, az úgynevezett *Commit Message*-et megadni.

Az ablak alján két gomb jelenik meg:

* A **Commit** gombbal csak mentjük a módosításokat, azok a saját gépünkön gyűlnek.

* A **Commit and Push** gombbal a változásokat egyből fel is töltjük a GitHub szerverre.

## Módosítások feltöltése (`push`)

Az elvégzett módosításokat ezzel a művelettel lehet feltölteni a GitHub szerverre. Az előző lépés mellett a *Git* menüből is behozható. A felbukkanó ablak kijelzi a feltöltendő *commit*okat. Kattints a **Push** gombra. Sikeres feltöltés esetén egy megerősítő értesítés jelenik meg.

## Módosítások letöltése (`pull`)

Előfordulhat, hogy az online kód frissebb, mint a gépeden lévő. Ez nálunk akkor fog előfordulni, ha több gépről is dolgozol, valamint ha a gyakorlatvezetőd házi feladatot tűzött ki a közös tárolóban.

**Git > Pull**

## Konfliktusok kezelése

A Git jóval több lehetőséget hordoz magában, mint amit mi használni fogunk. Előfordulhat, hogy online és a gépeden konfliktus lép fel fájlok között. Példa: otthon is szerkesztetted a kódot, valamint a tantermi gépen is, amit *push*-oltál is. Ekkor a Git érzékeli azt, hogy ellentmond a két állapot egymásnak, és nem tudja, melyiket írja felül a másikkal. Ennek megoldása nem feltétlenül egyszerű, ilyen esetben jobb, ha egy másik mappába letöltöd (*clone*-ozod) a projektet ismét, és ott dolgozol tovább.

