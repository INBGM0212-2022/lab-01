# Forráskód interpretálása

1. Hozz létre egy fájlt `hello.py` néven egy tetszőleges szövegszerkesztővel!

1. Nyisd meg egy szövegszerkesztővel a `hello.py` fájlt!

1. Írasd ki egy `print()` függvényhívással a `Hello, World!` sztringet!
    
    ```python
    print("Hello, World!")
    ```

1. Mentsd el és zárd be a fájlt.

2. Interpretáld a forráskódot.

    ```
    python <<útvonal/>>hello.py
    ```

3. Nyisd meg újból a fájlt, majd a kiírást helyezd a `main()` függvénybe.

    ```python
    def main():
        print("Hello, World")
    ```

4. Mentsd el a fájlt, majd interpretáld újból.

    ```
    python <<útvonal/>>hello.py
    ```

5. Nyisd meg újból a fájlt, majd gondoskodj arról egy belépési ponttal, hogy a modul futtatásakor a `main()` függvény kerüljön meghívásra!

    ```python
    def main():
        print("Hello, World")

    if __name__ == "__main__":
        main()
    ```