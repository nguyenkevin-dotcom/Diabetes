# Diabetes

# tl;dr
Semestrální skupinová práce. Cílem bylo zjistit hlavní faktory ovlivňující výskyt diabetu u žen pomocí dat a strojového učení. Použit byl dataset  https://www.openml.org/search?type=data&amp;sort=runs&amp;status=active&amp;id=37.

# Úvod
Tématem našeho semestrálního projektu byla analýza výskytu diabetu u žen pomocí různých metod strojového učení. Cílem bylo vytvořit prediktivní model, který by dokázal identifikovat faktory ovlivňující výskyt diabetu, a následně tyto informace využít k predikci onemocnění na základě vstupních dat.

# 🔬 Použitý dataset
Pracovali jsme s klasickým datasetem zaměřeným na ženy indiánského původu ve věku 21 let a více. Dataset obsahoval atributy jako:

    Plazmatická glukóza (plas),

    Tělesná hmotnost (BMI),

    Počet těhotenství,

    Tlak,

    Atd.

# 🧹 Předzpracování dat
Data jsme očistili od chybějících nebo nepravděpodobných hodnot a následně je rozdělili na trénovací a testovací množinu v poměru 70:30.

# 🤖 Modelování
Použili jsme jak supervised (učení s učitelem), tak unsupervised (učení bez učitele) přístupy:
- **Supervised learning**:

    Decision Tree (rozhodovací strom) – nejlepší výkon:

        Accuracy: 74,68 %,

        F1-score: 75,03 %

    Random Forest

    Baseline model – náhodný klasifikátor pro porovnání

- **Unsupervised learning**:

    K-means clustering

    Silhouette skóre: 0,512 (střední kvalita)

    Hierarchické shlukování s Wardovou metodou

# 📊 Vyhodnocení a interpretace
- **Decision Tree** se ukázal jako nejvýkonnější model a zároveň snadno interpretovatelný.
- Mezi nejvýznamnější atributy patřila **plazmatická glukóza (`plas`)**, která výrazně ovlivňovala rozhodnutí modelu.
- Shlukovací metody ukázaly potenciál pro segmentaci pacientů na základě podobných charakteristik.

