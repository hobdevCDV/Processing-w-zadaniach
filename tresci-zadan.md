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

### Zadanie 1. 
Korzystając ze środowiska Processing utwórz program, w którym wywołasz okno o rozmiarze 600 x 400 px, a następnie ustawisz kolor tła na: 
- turkusowy, 
- łososiowy. 

Zadanie wykonaj zarówno wyszukując kolor z wykorzystaniem kodu RGB oraz za pomocą narzędzia "color selector" i kodu szesnastkowego.

---

### Zadanie 2. 
Korzystając z funkcji ellipse() wykonać obraz przypominający kolorowy kwiat (okrąg w centrum ekranu oraz cztery elipsy po stronach: prawo, lewo, góra, dół)..

---

### Zadanie 3. 
Korzystając z funkcji ellipse() wykonać obraz pięciu kół przypominających kółka olimpijskie (nie muszą się przecinać).

---

### Zadane 4. 
Korzystając z funkcji rect() wykonać obraz przypominający symbol polskiej szachownicy lotniczej.

---

### Zadanie 5. 
Korzystając z funkcji rect(), ellipse() oraz triangle() wykonać grafiki przycisków play/stop/pause. 

---

### Zadanie 6. 
Korzystając z funkcji ellipse() i triangle() wykonać ilustrację porcji lodów w waflowym rożku.

---

### Zadanie 7. 
Korzystając z funkcji ellipse wykonać ilustrację księżyca w kształcie rogalika.

---

### Zadanie 8. 
Korzystając z funkcji line() podzielić okno na siatkę (plansza do gry w Go o rozmiarze 9 x 9 linii).

---

### Zadanie 9
Korzystając z poznanych narzędzi utwórz obraz zawierający obszar reprezentujący trawę (zielony prostokąt), niebo (niebieski prostokąt) i chmurkę (zestaw trzech elips).

---

### Zadanie 10. 
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


---

### Zadanie 11.
Korzystając z wbudowanych zmiennych mouseX, mouseY utworzyć elipsę, której pozycję i kolor będzie zależeć od położenia kursora myszy.

---

### Zadanie 12. 
Przemieszczająca się elipsa - utwórz program z dwiema zmiennymi, których wartość będzie kontrolować położenie elipsy na ekranie. Niech wraz z działaniem programu ich wartość się zwiększa i przemieszcza elipsę:
- od prawej do lewej,
- od lewej do prawej,
- z góry na dól,
- z dołu do góry.

Wypróbuj różne prędkości ich przemieszczania.

---

### Zadanie 13. 
Korzystając z operacji modulo wprowadź do programu z poprzedniego zadania (Przemieszczająca się elipsa) tzw. periodyczne warunki brzegowe:
- jeżeli elipsa dotrze do prawej krawędzi okna, zostanie przeniesiona na krawędź lewą,
- jeżeli elipsa dotrze do lewej krawędzi okna, zostanie przeniesiona na krawędź prawą,
- jeżeli elipsa dotrze do górnej krawędzi okna, zostanie przeniesiona na krawędź dolną,
- jeżeli elipsa dotrze do dolnej krawędzi okna, zostanie przeniesiona na krawędź górną.

---

### Zadanie 14.
Błądzenie chaotyczne - korzystając z funkcji random(), sin() i cos() utwórz program obrazujacy zagadnienie błądzenia chaotycznego - program startuje z niewielką elipsą w środku okna. W każdym kroku program losuje kąt o jaki ma się obrócić kierunek ruchu i przemieszca elipsę o zadany krok. Uwaga - w tym ćwiczeniu warto wyłączyć opcję odmalowywania tła w funkcji draw(). 

---

### Zadanie 15. 
Wykonaj animację ruchu planet wokół Słońca wraz z kilkoma księżycami. Skorzystaj z funkcji translate() i rotate().  

---

### Zadanie 16.
Symulacja wahadła - wykonaj symulację wahadła na sprężystej gumce. Punkt zaczepienia wahadła powinien być wskazywany przez współrzędne kursora myszy. 

---

### Zadanie 17. 
Korzystając z równań Lorenza spróbuj wykonać symulację atraktora Lorenza dla dwóch elips o nieznacznie różniących się pozycjach początkowych. Zachowaj ich trajektorie w liście (Array) i wyswietlaj na ekranie.

---

### Zadanie 18. 
Wróć co zadania "Przemieszczająca się elipsa" i uprość program korzystając z wektorów.

---

### Zadanie 19.
Wróć do zadania "Błądzenie chaotyczne" i uprość program korzystając z wektorów.

---

### Zadanie 20.
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

### Zadanie 21.
W oparciu o zadanie "Przemieszczająca się elipsa" i korzystając z instrukcji warunkowych, utwórz program, w którym będziesz sterować pozycją i szybkością elipsy za pomocą klawiatury:
- strzałka w prawo - rych w prawo
- strzałka w lewo - ruch w lewo
- strzałka w dół - ruch w dół
- strzałka w górę - ruch w górę
- klawisz 'q' - zwiększanie szybkości
- klasisz 'w' - zmniejszanie szybkości

---

### Zadanie 22.

Korzystając z funkcji random() oraz instrukcji warunkowych utworzyć program do szacowania wartości liczby pi (całkowanie Monte Carlo).

Korzystając z instrukcji warunkowych, utworzyć program sortujący 

Utworzyć program losujący (typu kostka do gry)

Utworzyć program do gry typu Pong

Utworzyć program typu Paint

Utworzyć program typu kolorowe kwadraty


---

### Zadanie


---

# IV. Pętle

---

# V. Funkcje własne

---

# VI. Podstawy programowania obiektowego

---
