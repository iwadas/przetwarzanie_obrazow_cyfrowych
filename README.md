# Przetwarzanie Obrazów Cyfrowych - Laboratoria

Niniejsze repozytorium zawiera materiały, skrypty oraz zadania domowe realizowane w ramach kursu Przetwarzania Obrazów Cyfrowych (Digital Image Processing). Poniżej znajduje się szczegółowy spis treści i opis poszczególnych laboratoriów.

---

## 📚 Spis treści

### Lab 2: Przekształcenia punktowe (Point transformations)
**Plik:** `lab_2.ipynb`

Podstawowe operacje bezkontekstowe na obrazach cyfrowych:
* **Operacje jednoargumentowe (LUT - Look-Up Table):** szybkie mapowanie wartości pikseli.
* **Operacje arytmetyczne (dwuargumentowe):** dodawanie, odejmowanie, mnożenie, dzielenie obrazów.
* **Operacje logiczne:** AND, OR, XOR, NOT.

### Lab 2 HW: Zadanie domowe
**Plik:** `lab_2_hw.ipynb`

* **Krojenie płaszczyzn bitowych (Bit-plane slicing):** tworzenie obrazów binarnych z poszczególnych bitów obrazu oryginalnego.
* **Rekonstrukcja obrazu:** odtwarzanie obrazu przy użyciu mniejszej liczby płaszczyzn bitowych (kompresja stratna).

---

### Lab 3: Histogram obrazu i jego wyrównywanie
**Plik:** `lab_3.ipynb`

* Pojęcie histogramu obrazu dla obrazów w odcieniach szarości oraz kolorowych.
* Metody modyfikacji histogramu: rozciąganie (stretching), wyrównywanie (equalization), dopasowywanie (matching).

### Lab 3 HW: Zadanie domowe - BBHE i DSIHE
**Plik:** `lab_3_hw.ipynb`

Implementacja zaawansowanych metod wyrównywania histogramu, mających na celu eliminację wad klasycznego HE (które często przesuwa średnią jasność do środkowego poziomu szarości):
* **BBHE (Bi-Histogram Equalization):** podział obrazu na podstawie średniej jasności.
* **DSIHE (Dualistic Sub-Image Histogram Equalization):** podział obrazu na dwa sub-obrazy o takiej samej liczbie pikseli.

---

### Lab 4: Binaryzacja obrazów
**Plik:** `lab_4.ipynb`

Segmentacja obiektów za pomocą binaryzacji:
* Binaryzacja na podstawie histogramu (globalna).
* Automatyczne metody wyznaczania progu: Otsu, Kittler, Kapur.
* Binaryzacja lokalna: metoda średniej oraz metoda Sauvola.
* Binaryzacja dwuprogowa.

---

### Lab 5: Przekształcenia geometryczne i interpolacja
**Plik:** `lab_5.ipynb`

* Przekształcenia geometryczne obrazów.
* Metody interpolacji pikseli, ze szczególnym uwzględnieniem **interpolacji dwusześciennej (Bicubic interpolation)**.

---

### Lab 6: Przetwarzanie wstępne i filtracja kontekstowa
**Plik:** `lab_6.ipynb`

Pojęcie kontekstu oraz splotu (convolution) w przetwarzaniu obrazów. 
Wybrane filtry:
* **Liniowe filtry dolnoprzepustowe:** uśredniający, filtr Gaussa.
* **Filtry nieliniowe:** filtr medianowy (również dla obrazów kolorowych).
* **Liniowe filtry górnoprzepustowe:** Laplasjan, operatory Robertsa, Prewitta i Sobela.

---

### Lab 7: Filtracja bilateralna
**Plik:** `lab_7.ipynb`

* Splot obrazu z filtrem o zadanych współczynnikach.
* **Filtracja bilateralna:** adaptacja współczynników filtra do lokalnego otoczenia w celu wygładzenia obrazu przy jednoczesnym zachowaniu ostrych krawędzi (uniknięcie rozmycia).

---

### Lab 8: Transformata Fouriera
**Plik:** `lab_8.ipynb`

* Wykorzystanie transformaty Fouriera w przetwarzaniu obrazów cyfrowych.
* Pojęcie F-obrazu (amplituda i faza) oraz własności transformaty.
* Filtracja obrazów w dziedzinie częstotliwości.

---

### Lab 9: Detekcja krawędzi
**Plik:** `lab_9.ipynb`

* Przypomnienie podstawowych metod detekcji krawędzi (Sobel, Prewitt, Roberts).
* Implementacja i analiza zaawansowanych detektorów: **Laplasjan z Gaussa (LoG)** oraz **detektor Canny'ego**.

---

### Lab 10: Operacje morfologiczne
**Plik:** `lab_10.ipynb`

* Podstawowe przekształcenia morfologiczne: erozja, dylatacja, otwarcie, zamknięcie, transformacja trafi-nie-trafi (hit-or-miss).
* Złożone operacje wykorzystujące rekonstrukcję morfologiczną.
* Operacje morfologiczne dla obrazów w odcieniach szarości: erozja, dylatacja, otwarcie, zamknięcie oraz filtry top-hat i bottom-hat.

---

### Lab 11: Transformacja Hougha
**Plik:** `lab_11.ipynb`

* Idea transformacji Hougha dla pojedynczego punktu, kilku punktów i prostych figur geometrycznych.
* Praktyczne wykorzystanie transformacji Hougha do detekcji linii prostych na rzeczywistych obrazach.

---

### Lab 12: Segmentacja obrazów
**Plik:** `lab_12.ipynb`

* Zapoznanie z metodami segmentacji:
    * **Segmentacja przez rozrost (Region growing).**
    * **Segmentacja przez podział i scalanie (Split and merge).**