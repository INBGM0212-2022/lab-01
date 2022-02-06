# Miniconda környezetek

Az útmutató elsődlegesen a Miniconda környezet otthoni kialakításához nyújt segítséget. Előfordulhat, hogy néhány parancs a tantermi gépeken eltérő paraméterezést igényel, amiért több gyakorlatot is ugyanabban a teremben tartunk.

## Miniconda letöltése és telepítése

* Letöltés: https://docs.conda.io/en/latest/miniconda.html
* Telepítés:
    * Windows: https://docs.conda.io/projects/conda/en/latest/user-guide/install/windows.html
    * Linux: https://docs.conda.io/projects/conda/en/latest/user-guide/install/linux.html

## Miniconda környezet kialakítása

### Conda terminál megnyitása

Az alábbi parancsokat egy Conda parancssorban kell kiadni. Windows operációs rendszeren az *Anaconda prompt (miniconda3)* kifejezés kezdetére érdemes rákeresni, majd megnyitni a konzol ablakot.

Sikeres elindítés esetén egy hasonló prompt látszik:

```
(base) C:\Users\Robert>
```

A `(base)` perfix azt jelenti, hogy az alapértelmezett környezetet használjuk. A következő feladatokban kialakítunk egy saját környezetet.


## Segédanyagok

* [Anaconda Cheet Sheet](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-python.html)

## Feladatok

1. Környezetek listázása

    ```
    conda env list
    ```

1. Környezet létrehozása (beállítások nélkül)

    ```
    conda create --name prog1
    ```

2. Környezetek listázása

    ```
    conda env list
    ```

3. Könyvtárak ellenőrzése

    Windows esetében a `C:/Users/<<felhasználónév>>/miniconda3/envs/` mappában találhatók a környezetek. Az előbb létrehozott környezet `prog1` mappáját megnyitva azt látjuk, csak gyakorlatilag üres.

4. A `prog1` környezet aktiválása

    ```
    conda activate prog1
    ```

    A prompt a parancs végrehajtása után a `(prog1)` prefixszel kezdődik.

5. Csomagok listázása

    ```
    conda list
    ```

    A környezet üres, ezért nincs egyetlen telepített csomag sem.

6. Python telepítése

    * Automatikus verzió választás

        ```
        conda install python
        ```

    * Explicit verzió választás
    
        ```
        conda install python=3.10
        ```

7. Csomagok listázása

    ```
    conda list
    ```

    A csomagok listája ezúttal bővebb: nemcsak a Python interpreter, hanem számos kapcsolódó csomag is feltelepült. Ellenőrizd a környezethez tartozó mappát is. Azt láthatod, hogy a csomagok forrásai ebbe a mappába kerültek.

8. Környezet deaktiválása

    ```
    conda deactivate
    ```

    A prompt ezzel újból a `(base)` prefixet tartalmazza.

9.  Környezet újbóli aktiválása

    ```
    conda activate prog1
    ```

10. Python verzió ellenőrzése

    ```
    python --version
    ```