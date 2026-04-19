# Przegląd literatury

Przegląd literatury obejmuje zarówno dokumentacje techniczne wykorzystywanych narzędzi, jak i artykuły oraz inne materiały naukowe opisujące podejścia stosowane w kontekście realizowanego projektu.


## Materiały naukowe
| Tytuł                 | Link      | Opis      |
|:----------------------|:----------|:----------|
| "Interpretability Beyond Feature Attribution: Quantitative Testing with Concept Activation Vectors (TCAV)"       | https://arxiv.org/pdf/1711.11279 | Metoda TCAV wykorzystująca koncepcję wektora aktywacji do ilościowego testowania, w jakim stopniu badane pojęcie wpłynęło na ostateczny wynik modelu (oblicza, jaki odsetek wszystkich obrazów z danej klasy zyskał pozytywną ocenę dzięki badanemu pojęciu). <br>  Metoda stosowana do wykrywania i badania uprzedzeń modelu.|
| "Image Data Augmentation Approaches: A Comprehensive Survey and Future directions"         | https://arxiv.org/pdf/2301.02830 | Przegląd metod augmentacji danych obrazowych, stosowanych w celu poprawy skuteczności modeli głębokiego uczenia i zapobiegania ich nadmiernemu dopasowaniu.|
"MediaPipe Hands: On-device Real-time Hand Tracking"	| https://arxiv.org/abs/2006.10214	| Praca przedstawia wydajny pipeline do detekcji i śledzenia dłoni w czasie rzeczywistym, oparty na modelu detekcji dłoni oraz estymacji 21 punktów charakterystycznych (landmarków). Podejście umożliwia reprezentację gestów jako wektorów punktów zamiast obrazów RGB, co znacząco redukuje koszt obliczeniowy i zwiększa odporność na zmienne warunki jak oświetlenie i tło.
"Online Detection and Classification of Dynamic Hand Gestures with Recurrent 3D Convolutional Neural Networks"	| https://research.nvidia.com/publication/2016-06_online-detection-and-classification-dynamic-hand-gestures-recurrent-3d	| Praca dotyczy rozpoznawania dynamicznych gestów dłoni w strumieniu wideo w trybie online, bez konieczności wcześniejszego segmentowania danych. Zaproponowane podejście wykorzystuje modele 3D CNN oraz sieci rekurencyjne do jednoczesnej detekcji i klasyfikacji gestów oraz identyfikacji momentu ich wystąpienia.



## Dokumentacje techniczne
| Narzędzie                  | Link      | Opis                          |
|:----------------------|:---------:|----------------------------------------|
| OpenCV | https://docs.opencv.org/4.x/ | biblioteka umożliwiająca modyfikowanie obrazów, pomocna w kontekście augmentacji danych |


