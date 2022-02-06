# GitHub autentikáció PyCharm-ban

Ebben a jegyzetben azt nézzük meg, miképp lehet a PyCharm IDE-vel bejelentkezni GitHub-ra.


## PyCharm bejelentkeztetése GitHub-ra

1. ***Help* > *Find action* > *Github (Settings)***

    Ez a menüpont sajnos el van rejtve, legegyszerűbben talán így a legkönnyebb elérni.

2. Kattints a **+** gombra > **Log in with Token**

3. Kattints a **Generate** gombra, majd jelentkezz be a megnyíló böngésző ablakban.

4. A **Note** mező értékeként adj meg egy olyan azonosítót, mely másik aktív kulcsnál nem szerepel. Példa: `prog1-lab`.

5. Az esetleges engedélyezés után válaszd ki a token érvényességét, valamint jelölj be **minden** opciót az engedélyeknél. A lap alján kattints a **Generate token** gombra. Az érvényesség a saját gépeden nyugodtan lehet **never expires**.

6. Másold vágólapra a generált tokent, majd illeszd be a *PyCharm* **Token** mezőjébe. Kattints az **Add Account** gombra.

7. Zárd be az ablakot.

Az adott PyCharm programban be vagy jelentkezve a GitHub felhasználóddal. Ez azt jelenti, hogy eléred a privát tárolóidat, valamint újakat is tudsz létrehozni. Viszont ezt nem csak te tudod megtenni, hanem az a személy is, aki még használja a gépet. Éppen ezért figyelj arra, hogy nem saját gépen mindig érvénytelenítsd a tokent az óra végén, illetve jelentkezz ki.

## PyCharm kijelentkeztetése GitHub-ról

### Token érvénytelenítése

1. Látogass el a [GitHub Tokens](https://github.com/settings/tokens) oldalra.

1. Kattins a token melletti **Delete** gombra.

### Kijelentkezés

1. **Help > Find action > Github (Settings)**

2. Kattints a profilod melletti **-** gombra, ha még látszódik.