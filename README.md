\# FIFA 23 Játékos Adathalmaz Elemzése



\## Projekt leírása

Ez a projekt az EA Sports FIFA 23 játékosainak adatait vizsgálja statisztikai módszerekkel és adatvizualizációval.

\- \*\*Felhasznált könyvtárak:\*\* NumPy, Pandas, Plotly

\- \*\*Adatforrás:\*\* Kaggle - FIFA 23 Players Dataset



\---



\## Az 5 vizsgált kérdés és eredmények



\### 1. Melyik életkorban érik el a játékosok a csúcsformájukat?

\- \*\*Módszer:\*\* Korcsoportok szerinti átlagos `Overall` képesség számítása Pandas segítségével, vonaldiagramos ábrázolás.

\- \*\*Megállapítás:\*\* A játékosok átlagos értékelése 27–30 éves kor körül éri el a csúcsot.



\### 2. Milyen kapcsolat van a piaci érték és a heti fizetés között?

\- \*\*Módszer:\*\* Logaritmikus transzformáció és Pearson-korreláció számítása NumPy-val (`np.corrcoef`), Plotly scatter plot ábrázolás.

\- \*\*Megállapítás:\*\* Erős pozitív kapcsolat figyelhető meg a magasabb piaci értékű játékosok bérezésében.



\### 3. Mely pozíciókban a legmagasabb a medián piaci érték?

\- \*\*Módszer:\*\* Pozíciók szerinti csoportosítás és a szélsőértékekre kevésbé érzékeny medián érték oszlopdiagramos ábrázolása.

\- \*\*Megállapítás:\*\* A támadók (CF, ST) és a modern belső középpályások rendelkeznek a legmagasabb piaci értékkel.



\### 4. Mely alapmutatók mutatják a legszorosabb statisztikai összefüggést?

\- \*\*Módszer:\*\* Korrelációs mátrix előállítása NumPy segítségével (`np.corrcoef`), Plotly hőtérképen (Heatmap) renderelve.

\- \*\*Megállapítás:\*\* A pillanatnyi szint (`Overall`) és a játékos fejlődési potenciálja (`Potential`) között van a legerősebb kapcsolat.



\### 5. Mely nemzetek adják a legtöbb elit (Overall >= 85) játékost?

\- \*\*Módszer:\*\* Feltételes szűrés és gyakorisági összesítés (`value\_counts`), Plotly sávdiagramos megjelenítés.

\- \*\*Megállapítás:\*\* Brazília, Franciaország, Spanyolország és Németország adja az elit játékosok zömét.



\---



\## Futtatás

```bash

pip install numpy pandas plotly nbformat

jupyter notebook fifa23\_elemzes.ipynb



