# Prototyp rozwiązania

## Augmentacja danych

### Zmiana koloru skóry

Procedura:
1. Konwersja przestrzeni barw z BGR na HSV
2. Wyznaczenie maski skóry poprzez zdefiniowanie zakresów wartości HSV odpowiadającym kolorowi skóry
3. Oczyszczenie maski z wykorzystaniem operacji morfologicznych, wygładzenia Gaussa oraz progowania
4. Modyfikacja jasności pikseli należących do maski

Wstępne wyniki:

<div style="display: flex; gap: 20px; justify-content: center;">

<figure style="text-align: center;">
    <img src="../images/original.jpg" width="500">
    <figcaption>Oryginalna ręka</figcaption>
</figure>

<figure style="text-align: center;">
    <img src="../images/mask_raw.jpg" width="500">
    <figcaption>Maska skóry na podstawie wartości HSV</figcaption>
</figure>

</div>

<div style="display: flex; gap: 20px; justify-content: center;">

<figure style="text-align: center;">
    <img src="../images/mask_clean.jpg" width="500">
    <figcaption>Wygładzona maska</figcaption>
</figure>

<figure style="text-align: center;">
    <img src="../images/result.jpg" width="500">
    <figcaption>Ręka po augmentacji</figcaption>
</figure>

</div>
