# I. Wprowadzenie do środowiska Processing

## Pojęcia do omówienia:
- przegląd strony oraz repozytorium projektu 
- przegląd projektów siostrzanych
- pobieranie i instalacja środowiska
- interfejs środowiska
- instalacje i import dodatkowych bibliotek 
- narzędzia wbudowane (np. color selector) i narzędzia zewnętrzne 
- możliwość korzystania z innych języków programowania
- preferencje środowiska
- funkcje setup() i draw()
- rozmiary okna i tryb pełnoekranowy
- zmiana koloru tła 
- wprowadzanie podstawowych kształtów (linia, elipsa, prostokąt, trójkąt)
- wypełnienie i obrys (fill, stroke, noStroke, lineWidth)
- budowanie bardziej skomplikowanych kształtów (blok beginShape/endShape)
- podstawowe transformacje kształtów (funkcje translate, rotate, pushMatrix)
- układ współrzędnych
- reprezentacja barw w systemie RGB (systemy dziesiętne i szesnastkowe)

---

### Zadanie 1.1
Korzystając ze środowiska Processing utwórz program, w którym wywołasz okno o rozmiarze 600 x 400 px, a następnie ustawisz kolor tła na: 
- turkusowy, 
- łososiowy. 

Zadanie wykonaj zarówno wyszukując kolor z wykorzystaniem kodu RGB oraz za pomocą narzędzia "color selector" i kodu szesnastkowego.

---

### Zadanie 1.2
Korzystając z funkcji ellipse() wykonać obraz przypominający kolorowy kwiat (okrąg w centrum ekranu oraz cztery elipsy po stronach: prawo, lewo, góra, dół)..

---

### Zadanie 1.3
Korzystając z funkcji ellipse() wykonać obraz pięciu kół przypominających kółka olimpijskie (nie muszą się przecinać).

---

### Zadane 1.4
Korzystając z funkcji rect() wykonać obraz przypominający symbol polskiej szachownicy lotniczej.

---

### Zadanie 1.5
Korzystając z funkcji rect(), ellipse() oraz triangle() wykonać grafiki przycisków play/stop/pause. 

---

### Zadanie 1.6
Korzystając z funkcji ellipse() i triangle() wykonać ilustrację porcji lodów w waflowym rożku.

---

### Zadanie 1.7
Korzystając z funkcji ellipse wykonać ilustrację księżyca w kształcie rogalika.

---

### Zadanie 1.8 
Plansza do Go - korzystając z funkcji line() podzielić okno na siatkę (plansza do gry w Go o rozmiarze 9 x 9 linii).

---

### Zadanie 1.9
Korzystając z poznanych narzędzi utwórz obraz zawierający obszar reprezentujący trawę (zielony prostokąt), niebo (niebieski prostokąt) i chmurkę (zestaw trzech elips).

---

### Zadanie 1.10
Korzystając z bloku beginShape / endShape zbudować pięciokąt. 

---

# II. Zmienne i podstawowe typy danych

## Pojęcia do omówienia
- pojęcie zmiennej
- podstawowe typy danych (liczby całkowite, liczby zmiennoprzecinkowe, zmienne logiczne, łańcuchy znaków, tablice, listy, wektory)
- rzutowanie/konwersja typu (int(), float(), str())
- zmienne systemowe (na przykładzie width, height, mouseX, mouseY)
- konsola i wypisywanie komunikatów za pomocą polecenia println()
- polecenie text() i wypisywanie danych w oknie programu
- operacja modulo
- funkcje trygonometryczne i sposoby miary kąta
- liczby losowe
- instrukcja frameRate()
- instrukcja frameCount
- eksport aplikacji


---

### Zadanie 2.1
Korzystając z wbudowanych zmiennych mouseX, mouseY utworzyć elipsę, której pozycję i kolor będzie zależeć od położenia kursora myszy. Możesz sprawdzić wartości przechowywane przez zmienne systemowe mouseX i mouseY korzystając z polecenia println(), które wyświetli je w konsoli środowiska.

---

### Zadanie 2.2
Przemieszczająca się elipsa - utwórz program z dwiema zmiennymi, których wartość będzie kontrolować położenie elipsy na ekranie. Niech wraz z działaniem programu ich wartość się zwiększa i przemieszcza elipsę:
- od prawej do lewej,
- od lewej do prawej,
- z góry na dól,
- z dołu do góry.

Wypróbuj różne prędkości ich przemieszczania.

---

### Zadanie 2.3
Korzystając z operacji modulo wprowadź do programu z poprzedniego zadania (Przemieszczająca się elipsa) tzw. periodyczne warunki brzegowe:
- jeżeli elipsa dotrze do prawej krawędzi okna, zostanie przeniesiona na krawędź lewą,
- jeżeli elipsa dotrze do lewej krawędzi okna, zostanie przeniesiona na krawędź prawą,
- jeżeli elipsa dotrze do górnej krawędzi okna, zostanie przeniesiona na krawędź dolną,
- jeżeli elipsa dotrze do dolnej krawędzi okna, zostanie przeniesiona na krawędź górną.

---

### Zadanie 2.4
Błądzenie chaotyczne - korzystając z funkcji random(), sin() i cos() utwórz program obrazujacy zagadnienie błądzenia chaotycznego - program startuje z niewielką elipsą w środku okna. W każdym kroku program losuje kąt o jaki ma się obrócić kierunek ruchu i przemieszca elipsę o ustalony krok. Uwaga - w tym ćwiczeniu warto wyłączyć opcję odmalowywania tła w funkcji draw(). 

---

### Zadanie 2.5
Wykonaj animację ruchu czterech pierwszych planet wokół Słońca wraz z ich księżycami. Skorzystaj z funkcji translate() i rotate(). Lokalne korzystanie z ustawień translacji i rotacji w obrębie funkcji draw() umożliwia konstrukcja push()/pop().  

---

### Zadanie 2.6
Symulacja wahadła - wykonaj symulację wahadła na sprężystej gumce. Punkt zaczepienia wahadła powinien być wskazywany przez współrzędne kursora myszy. 

---

### Zadanie 2.7
Korzystając z listy (Array) i wektorów wykonaj przemieszczający się na ekranie łańcuch pięciu elips.

---

### Zadanie 2.8
Wróć co zadania "Przemieszczająca się elipsa" i uprość program korzystając z wektorów.

---

### Zadanie 2.9
Wróć do zadania "Błądzenie chaotyczne" i uprość program korzystając z wektorów.

---

### Zadanie 2.10
Wróć do zadania "Symulacja wahadła" i uprość program korzystając z wektorów.

---

# III. Instrukcje warunkowe

## Pojęcia do omówienia:
- składnia instrukcji warunkowej
- zmienne logiczne - przypomnienie
- zmienne systemowe: keyPressed, keyCode, key, mousePressed
- instrukcja setup()
- instrukcja loop()/noLoop()

---

### Zadanie 3.1

Napisz program, w którym na środku ekranu będzie widoczna elipsa. Jej kolor powinien zmieniać się w zależności od warunku, czy naciśnięty został klawisz myszy. 

Wariant 1 - elipsa jest początkowo biała:
- jeżeli naciśnięto dowolny przycisk myszy - jej wypełnienie zmienia kolor na czarny,
- jeżeli zwolniono dowolny przycisk myszy - jej wypełnienie wraca do koloru białego.

Wariant 2 - elipsa jest początkowo biała:
- jeżeli naciśnięto dowolny przycisk myszy - jej wypełnienie zmienia kolor na czarny i pozostaje czarne nawet po zwolnieniu przycisku myszy,
- ponowne naciśnięcie dowolnego przycisku myszy powoduje zmianę kloru wypełnienia na biały.

### Zadanie 3.2

Utworzyć program, w którym okno zostanie podzielone na 9 równych kwadratów (siatka 3 x 3). Kwadraty będą zmieniać śwoje kolory w zależności od tego, czy w ich obszarze znajduje się kursor myszy, czy też nie. 

---

Zadanie 3.3

Utwórz program imitujący tarczę zegara z dwiema wskazówkami. Niech prędkości kątowe wskazówek będą sterowane klawiszami klawiatury:
- q - zwiększanie prędkości kątowej dużej wskazówki,
- a - zmniejszanie prędkości kątowej dużej wskazówki,
- w - zwiększanie prędkości kątowej małej wskazówki,
- s - zmniejszanie prędkości kątowej małej wskazówki.

---

### Zadanie 3.4
W oparciu o zadanie "Przemieszczająca się elipsa" wprowadź w programie możliwość odbicia elipsy od krawędzi okna.

---

### Zadanie 3.5
W oparciu o zadanie "Przemieszczająca się elipsa" i korzystając z instrukcji warunkowych, utwórz program, w którym będziesz sterować pozycją i szybkością elipsy za pomocą klawiatury:
- strzałka w prawo - rych w prawo
- strzałka w lewo - ruch w lewo
- strzałka w dół - ruch w dół
- strzałka w górę - ruch w górę
- klawisz 'q' - zwiększanie szybkości
- klasisz 'w' - zmniejszanie szybkości

Dodatkowo, możesz napisać rozbudowaną wersję programu, wyświetlającą aktualny czas za pomocą poleceń second(), minute(), hour().

---

### Zadanie 3.6

Utworzyć program losujący (typu kostka do gry). Program powinien posiadać w środku ekranu kwadrat wyświetlający w formie cyfr od 1 do 6, oraz przycisk, który po naciśnięciu klawiszem muszy wykona losowanie. 

---

### Zadanie 3.7

Korzystając z funkcji random() oraz instrukcji warunkowych utworzyć program do szacowania wartości liczby pi (za pomocą tzw. algorytmu całkowania Monte Carlo).

---

### Zadanie 3.8

Utworzyć program do gry typu Pong dla dwóch graczy. Gracze za pomocą klawiszy klawiatury (np. w, s, p, l) sterują swoimi paletkami i odbijają między sobą ruchomą piłkę. Piłka, gdy uderzy w górną lub dolną krawędź okna - ulega odbiciu, z kolei kiedy ominie paltetkę gracza i wpadnie na krawędź prawą lub lewą - zostaje przeniesiona na środek ekranu, a gracz przeciwny otrzymuje punkt. 

---

Zadanie 3.9

Utworzyć program z modelem samochodu (widok z góry), sterowanym za pomocą klawiszy klawiatury w, a, s, d z wizualizacją skrętu przednich kół. Kształt samochodu należy wykonać z prostokątów (nadwozie, koła, okna, światła). Dodatkowo klawisz q powinien zmieniać kolor kwadratów reprezentujących światła (wizualizacja włączania lub wyłączania świateł) natomiast hamowanie powinno powodować zmianę koloru tylnych lamp. Do sterowania samochodem wykorzystaj instrukcje translate() i rotate().

---

### Zadanie 3.10

Utworzyć program do rysowania. Program powinien posiadać do rysowania przynajmniej 3 narzędzia i 6 kolorów. Do zapisu utworzonego obrazu wykorzystaj funkcję save(), natomiast do czyszczenia ekranu funkcję setup(). 

---

# IV. Pętle

## Zagadnienia do omówienia:
1. Co to jest pętla
2. Rodzaje pętli (pętla draw, pętla while i pętla for)
3. Polecenie noLoop()
4. Wykorzystanie iteratora w charakterze zmiennej
5. Zastosowanie instrukcji warunkowych w obrębie pętli

---

### Zadanie 4.1
Korzystając z pętli for utwórz łańcuch conajmniej 20 elips rozmieszczonych po przekątnej okna.

---

### Zadanie 4.2
Wróć do zadania "Plansza do Go". Wykonaj planszę do gry w Go, ale tym razem o wymiarze 19 x 19 linii z wykorzystaniem pętli for.

---

### Zadanie 4.3
Korzystając z pętli for utwórz klasyczną szachownicę (8 x 8 pól) wraz z opisem literowym i cyfrowym pozycji pól.

---

### Zadanie 4.4

Utwórz program do generowania kolorowych tekstór złożonych z kwadratów o losowym kolorze z pewnego zakresu barw. Generowane obrazy powinny imitować tekstury bloków znane m. in. z gier otwartego świata typu Minecraft. Program można rozbudować o możliwość zapisu tworzonych tekstur za pomocą polecenia save(). 

---

### Zadanie 4.5
Korzystając z instrukcji warunkowych oraz pętli for, utworzyć program sortujący losowo wybrany zestaw prostokątów o równych podstawach i różnych wysokościach (można zastosować dowolny algorytmnia).

---

### Zadanie 4.6

Rozbuduj program "Przemieszczająca się elipsa" - dodaj do niej kolejne elipsy tak, żeby na ekranie poruszało się ich minimum 10. W zadaniu należy skorzystać z pętli i z list (Array).

---

### Zadanie 4.7
Rozbuduj program "Symulacja wahadła", dodaj do niego kolejne wahadła tak, aby na ekranie symulowana była dynamika zestawu wahadeł (minimum 10). W zadaniu należy skorzystać z pętli i z list (Array).

---

### Zadanie 4.8
Spirala - korzystając z pętli utwórz program generujący (za pomocą małych kwadratów) kwadratową spiralę.

---

### Zadanie 4.9
Rozbuduj program "Spirala" tak, aby kolor kolejnych kwadratów zależał od tego, czy numer danego kwadratu jest liczbą pierwszą (spirala Ulama).

---

### Zadanie 4.10
Utwórz grę typu snake - sterujemy imitacją węża, który zwiększa swoją długość po kolizji z celem, równocześnie zdobywając punkty. Gracz przegrywa, jeżeli doprowadzi do kolicji głowy węża z jego ciałem.  

---

# V. Funkcje własne

## Zagadnienia do omówienia:
1. Co to jest funkcja?
2. Co to są argumenty?
3. Co może zwracać funkcja?
4. Co oznacza słowo void?

---

### Zadanie 5.1

Funkcja sprawdzająca czy liczba jest pierwsza

---

### Zadanie 5.2

Obliczanie pola i obwodu figur płaskich

---

### Zadanie 5.3

Funkcje wywołujące przemieszczanie figury po określonej trajektorii

---

### Zadanie 5.4

Rysowwanie celu - argumentem ilość pierścieni

---

### Zadanie 5.5

Rysowanie wielokąta - argumentem ilość ścian

---

### Zadanie 5.6

Rysowanie gwiazdy - argumentem liczba ramion

---

### Zadanie 5.6

Rysowanie spirali

---

### Zadanie 5.7 

Rysowanie spirali liczb pierwszych (Ulama)

---

### Zadanie 5.8

Rysowanie szachownicy

---

### Zadanie 5.9

Rysowanie przycisków

---

### Zadanie 5.10

Rysowanie samochodu

---

# VI. Podstawy programowania obiektowego i zagadnienia dodatkowe 

## Zagadnienia do omówienia:
1. Co to jest klasa i obiekt
2. Co to są pola i metody
3. Co to jest konstruktor
4. Jak wczytywać dane
5. Co to jest port szeregowy i jak pobierać dane wysyłane z Arduino?
6. Jak tworzyć wykresy?

---

### Zadanie 6.1

Przerobić program "Przesuwająca się elipsa"

---

### Zadanie 6.2

Przerobić program "Błądzenie chaotyczne"

---

### Zadanie 6.3

Przerobić program "Oscylator"

---

### Zadanie 6.4

Układ cząsteczkowy

---

### Zadanie 6.5

Arkanoid

---

### Zadanie 6.6

Processing Hero

---

### Zadanie 6.7

Wczytywanie danych

---

### Zadanie 6.8

Robienie wykresów

---

Zadanie 6.9

Łączenie Processingu z Arduino

---

### Zadanie 6.10

Podłączanie kamery

---
