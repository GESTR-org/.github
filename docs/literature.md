# Przegląd literatury

Przegląd literatury obejmuje zarówno dokumentacje techniczne wykorzystywanych narzędzi, jak i artykuły oraz inne materiały naukowe opisujące podejścia stosowane w kontekście realizowanego projektu.


## Materiały naukowe
| Tytuł                 | Link      | Opis      |
|:----------------------|:----------|:----------|
| "Interpretability Beyond Feature Attribution: Quantitative Testing with Concept Activation Vectors (TCAV)"       | https://arxiv.org/pdf/1711.11279 | Metoda TCAV wykorzystująca koncepcję wektora aktywacji do ilościowego testowania, w jakim stopniu badane pojęcie wpłynęło na ostateczny wynik modelu (oblicza, jaki odsetek wszystkich obrazów z danej klasy zyskał pozytywną ocenę dzięki badanemu pojęciu). <br>  Metoda stosowana do wykrywania i badania uprzedzeń modelu.|
| "Image Data Augmentation Approaches: A Comprehensive Survey and Future directions"         | https://arxiv.org/pdf/2301.02830 | Przegląd metod augmentacji danych obrazowych, stosowanych w celu poprawy skuteczności modeli głębokiego uczenia i zapobiegania ich nadmiernemu dopasowaniu.|
"MediaPipe Hands: On-device Real-time Hand Tracking"	| https://arxiv.org/abs/2006.10214	| Praca przedstawia wydajny pipeline do detekcji i śledzenia dłoni w czasie rzeczywistym, oparty na modelu detekcji dłoni oraz estymacji 21 punktów charakterystycznych (landmarków). Podejście umożliwia reprezentację gestów jako wektorów punktów zamiast obrazów RGB, co znacząco redukuje koszt obliczeniowy i zwiększa odporność na zmienne warunki jak oświetlenie i tło.
"Online Detection and Classification of Dynamic Hand Gestures with Recurrent 3D Convolutional Neural Networks"	| https://research.nvidia.com/publication/2016-06_online-detection-and-classification-dynamic-hand-gestures-recurrent-3d	| Praca dotyczy rozpoznawania dynamicznych gestów dłoni w strumieniu wideo w trybie online, bez konieczności wcześniejszego segmentowania danych. Zaproponowane podejście wykorzystuje modele 3D CNN oraz sieci rekurencyjne do jednoczesnej detekcji i klasyfikacji gestów oraz identyfikacji momentu ich wystąpienia.
| "Fast Learning of Dynamic Hand Gesture Recognition with Few-Shot Learning Models" | https://arxiv.org/abs/2212.08363 | Zaproponowany system rozpoznawania gestów dłoni wykorzystuje nagrania RGB, z których za pomocą MediaPipe Hands wyodrębniane są trójwymiarowe punkty szkieletu dłoni. Dane te trafiają do modelu Few-Shot Learning opartego na Relation Network z LSTM, który porównuje gesty i zwraca prawdopodobieństwo dopasowania. <br> Model trenowano na zmodyfikowanym zbiorze Jester, gdzie utworzono 676 złożonych klas poprzez łączenie gestów w sekwencje. Pomimo użycia jedynie 1–5 próbek na klasę, osiągnięto wysoką skuteczność (do ok. 88–91%). Kluczowym wynikiem jest znaczne ograniczenie zapotrzebowania na dane - nawet o ponad 1200 próbek względem tradycyjnych metod, przy zachowaniu podobnej dokładności.
| "Deep Learning Model for Dynamic Hand Gesture Recognition for Natural Human-Machine Interface on End Devices" | https://www.igi-global.com/gateway/article/306636 | Model E3D (Enhanced 3D-CNN) to system rozpoznawania gestów działający w czasie rzeczywistym, oparty na dwustopniowym pipeline: detekcji i klasyfikacji. W fazie treningowej w chmurze uczone są dwa modele: Tiny-YOLOv2 do wykrywania dłoni oraz 3D-CNN (ResNeXt) do rozpoznawania gestów, a następnie optymalizowane i wdrażane na urządzenia brzegowe. <br> Podczas działania system analizuje ciągły strumień wideo. Najpierw Tiny-YOLOv2 wykrywa dłoń i wyznacza początek gestu, po czym obraz jest centrowany, a kolejne klatki trafiają do bufora. Tak przygotowana sekwencja przekazywana jest do 3D-CNN, który rozpoznaje gest. <br> Kluczową zaletą pipeline’u jest rozdzielenie detekcji i klasyfikacji, co pozwala dokładnie uchwycić początek ruchu i znacząco poprawia skuteczność (ponad 92%) przy zachowaniu działania w czasie rzeczywistym. <br> Do ewaluacji wykorzystano zbiory Jester (20BN-JESTER), COCO oraz Cambridge Hand Gesture Dataset, a dodatkowo zastosowano własny zbiór danych rozszerzony o syntetyczne obrazy dłoni na różnych tłach.



## Dokumentacje techniczne
| Narzędzie                  | Link      | Opis                          |
|:----------------------|:---------:|----------------------------------------|
| OpenCV | https://docs.opencv.org/4.x/ | biblioteka umożliwiająca modyfikowanie obrazów, pomocna w kontekście augmentacji danych |


