# Neurális háló alapú osztályozás – Exam Score Dataset

## 1. Bevezetés
A beadandó célja egy neurális háló alapú osztályozó modell készítése TensorFlow segítségével.  
A modell egy Kaggle-ről származó adathalmazt használ, amely tanulók jellemzői alapján egy előre definiált kategóriába sorolja az eredményüket (pl. sikeres / sikertelen).

## 2. Adathalmaz bemutatása
A projektben az **Exam Score Prediction Dataset** kerül felhasználásra, amely numerikus jellemzőket tartalmaz a tanulók teljesítményével kapcsolatban.

- Forrás: Kaggle
- Adattípus: strukturált, numerikus
- Feladat típusa: osztályozás
- Célváltozó: kategóriává alakított vizsgaeredmény (pl. alacsony / közepes / magas)

## 3. Adatelőkészítés
Az adatok betöltése után az alábbi lépések történnek:
- hiányzó értékek eltávolítása
- a célváltozó osztályokká alakítása
- bemeneti és kimeneti adatok szétválasztása
- adatok skálázása
- tanító és teszt adathalmaz létrehozása

## 4. Neurális háló architektúra
A modell egy egyszerű, többrétegű neurális háló TensorFlow / Keras segítségével.

- bemeneti réteg a jellemzők számával
- rejtett rétegek ReLU aktivációval
- kimeneti réteg Softmax aktivációval
- veszteségfüggvény: categorical / sparse categorical crossentropy
- optimalizáló: Adam

## 5. Tanítás folyamata
A neurális háló több epochon keresztül kerül betanításra.  
A tanítás során a modell a tanító adatok alapján tanulja meg az osztályok közötti különbségeket, miközben validációs adatokon ellenőrizzük a teljesítményt.

## 6. Kiértékelés
A modell teljesítményét a teszt adathalmazon értékeljük ki.

Használt metrikák:
- pontosság (accuracy)
- veszteség (loss)

Az eredmények alapján megállapítható, hogy a modell képes a bemeneti adatok helyes osztályba sorolására.

## 7. Következtetések
A TensorFlow-alapú neurális háló hatékony megoldást nyújt az osztályozási feladatra.  
A modell tovább fejleszthető a rétegek számának módosításával, több adat használatával vagy más regularizációs technikák alkalmazásával.
