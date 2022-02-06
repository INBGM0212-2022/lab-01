
# PyCharm IDE használata

## Előkészületek

1. Szükség esetén töltsd le és telepítsd a szoftvert a következő helyről: https://www.jetbrains.com/pycharm/download/#section=windows

    A tantárgy során elég az ingyenes, *Community* verzió. Ennek ellenére érdemes tudni, hogy egyetemi email címmel (pl. `mailbox.unideb.hu`) ingyenes, egy éves licensz igényelhető a *Professional* verzióhoz is.


### Új projekt létrehozása és konfigurálása

1. Indítsd el a *PyCharm*-ot!

1. Hozz létre egy projektet `prog1-lab` néven!
    
    1. Menüpont: **File > New project**, ha egy másik projekt már meg van nyitva. Ellenkező esetben csak kattints a **New Project** gombra.

    1. A projekt típusa: **Pure Python**

    1. A projekt helyét tetszőlegesen választhatod meg.
   
        A kari gépeken a `C:/Users/hallgato` mappát (és almappáit) érdemes használni. Ezekben van írási és olvasási jogosultságunk is. Érdemes azonban a gyakorlat időpontjával vagy a neveddel egy saját mappát létrehozni, mert más is dolgozhat ugyanezen a gépen, illetve próbálhat azonos nevű projekteket is létrehozni.

    2. Nyisd le az elérési út alatt található, **Python interpreter...** fület.

    3. Válaszd ki a **Previously configured interpreter** opciót.

    4. Válaszd ki a Miniconda környezetedben lévő, 3.10-es interpretert:

        * Szerencsés esetben a lenyíló listában szerepel az interpreter, ekkor csak ki kell választani.

        * Egyébként ki kell tallózni a környezet mappájában szereplő `python.exe` fájlt. Ehhez a felbukkanó ablak bal oldalán válaszd ki a **Conda Environment** opciót, majd addd meg az elérési útvonalat.

    5. A pipát szedd ki a **Create a main.py welcome script** opcióból.

    6. Kattints a **Create** gombra.

2. Hozz létre egy `src` mappát, majd jelöld meg projekt gyökereként!
    1. Jobb klikk a projekt nevére > **New** > **Directory**

    2. Add meg az `src` nevet, majd nyomj egy **Enter**-t.

    3. Jobb klikk a mappa nevére > **Mark directory as...** > **Sources Root**

3. Hozz létre egy `lab01` csomagot!
    1. Jobb klikk az `src` mappára > **New** > **Python package**

    2. Add meg a `lab01` nevet, majd nyom egy **Enter**-t.

4. Hozz létre egy `hello` modult a `lab01` csomagban!
    1. Jobb klikk az `src` mappára > **New** > **Python module**

    2. Add meg a `hello` nevet, majd nyom egy **Enter**-t.
    
5. Írd ki a `Hello, World!` üzenetet egy `print()` függvényhívással!

    ```python
    print("Hello, World!")
    ```
6. Interpretáld a kódot!

    * Jobb klikk a modul nevére > **Run**

        Megjelenik az integrált terminál, melynek első sora az interpreter, valamint a szkript elérési útvonalát is tartalmazza. Ha az interpreter elérési útvonala nem a *Miniconda* környezetre mutat, akkor hajtsd végre a következő lépést:
        
        **Help** > **Find Action** > **Switch Python interpreter** > interpreter kiválasztása.

7. Egészítsd ki a forráskódot egy belépési ponttal, majd mozgasd át a kiírást a blokkjába!

    ```python
    if __name__ == "__main__":
        print("Hello, World!")
    ```

    Ekkortól már az `if` utasítás mellett is megjelenik egy futtatást jelentő gomb.

8. Egészítsd ki a forráskódot egy `main()` függvénnyel, majd mozgasd át a kiírást a törzsébe!

    ```python
    def main():
        print("Hello, World!")

    if __name__ == "__main__":
        main()
    ```

### Integrált Python konzol elérése

Az IDE alsó sávjában megjelenik egy **Python Console** fül is, melyre válts át. A megjelenő felületen interaktív üzemmódban tudod az interpretert használni. A terminál első sorában itt is ellenőrizni kell az elérési útvonalat, szükség esetén meg kell azt változtatni.