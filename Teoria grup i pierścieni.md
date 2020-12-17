# Wykład 1 | 10.10.2020

Wykład odwołany.

# Wykład 2 | 24.10.2020

## Kolokwia

1. 6. zjazd
2. 10. zjazd

## Adres: rgigon@ath.bielsko.pl

## Oznaczenia zbiorów

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{N}"> -- liczby naturalne: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{N} = \{0, 1, 2... \}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Z_+}"> -- liczby całkowite dodatnie
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Z}"> -- liczby całkowite: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Z} = \{...-2, -1, 0, 1, 2...\}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Q}"> -- liczby (ułamki) wymierne: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Q} = \{ \frac{a}{b}: a \in \mathbb{Z}, b \in \mathbb{Z_+}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{IQ}"> -- niewymierne, np. <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\sqrt{2}"> 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{R}"> -- rzeczywiste: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{R} = \mathbb{Q} \cup \mathbb{IQ} \}"> 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{C}"> -- zespolone: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{C} = \{ a + ib; a, b \in \mathbb{R}; i^2 = -1 \}">

## Działania arytmetyczne na zbiorach 

| Zbiór |  <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=+"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\cdot"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=:"> |
|-|-|-|-|-|
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{N}"> | tak^[a] | nie | tak | nie | 
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Z_+}"> | tak | nie | tak | nie |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Z}"> | tak | tak | tak | nie |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Q}"> | tak | tak | tak | nie |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Q} \setminus \{Q\}"> | nie | nie | tak | tak |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{IQ}"> | nie | nie | nie | nie |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{R}"> | tak | tak | tak | nie |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{C}"> | tak | tak | tak | nie |

[a]: Dla każdych 2 liczb można znaleźć sumę (różnicę, iloczyn, iloraz) z tego samego zbioru. 

## Liczby zespolone

* dodawanie i odejmowanie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\\(a+ib) + (c + id) := (a+c) + i(b+d)">
* mnożenie i dzielenie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\\(a+ib) \cdot (c+id) \\= ac + iad + ibc + i^2 bd \\= ac + i(ad + bc) - bd">

Przykład: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(2+3i)(-3-2i) = -6 - 6i^2 - 13i = -13i">

## Definicja formalna działania dwuargumentowego

Niech <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A"> będzie niepustym zbiorem. Działaniem <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet"> (czyt. kropka) określonym na zbiorze <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A"> nazywamy (każdą) funkcję <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet"> (kropka) taką, że: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=A \times A -> A">

(czyt. _A krzyż A_) tj. zbiór uporządkowanych par (iloczyn kartezjański), gdzie:  <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A \times A = \{ (a,b) : a, b \in A \}">

Przykłady

* mnożenie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\cdot(a, b) := a \cdot b, ab">

* działanie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\cdot"> w zbiorze <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A = \{1, 2\}"> zdefiniowanym jako: 

| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet_1"> | 1 | 2 | 
|-|-|-|
| **1** | 1 | 2 | 
| **2** | 1 | 1 |

* działanie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet"> w zbiorze <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A = \{1, 2\} zdefiniowanym jako: 

| ">\bullet_2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | 1 | 2 |
|-|-|-|
| **1** | 2 | 2 |
| **2** | 2 | 2 |

# Ćwiczenia 2 | 24.10.2020

* działanie w zbiorze 3-elementowym ">A = \{1, 2, 3\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= z działaniem 2-argumentowym ">\bullet<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- ">3^2=9<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= możliwych działań): 

| ">\bullet<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | 1 | 2 | 3 |
|-|-|-|-|
| **1** | 3 | 2 | 2 |
| **2** | 2 | 1 | 1 |
| **3** | 3 | 1 | 3 |

* działania w zbiorze 4-elementowym: ">4^2 = 16<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= możliwych działań 2-argumentowych; 

* działania w zbiorze 5-elementowym: ">5^2 = 25<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= możliwych działań 2-argumentowych. 

Ogólnie w zbiorze ">n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-elementowym możliwe jest ">n^m<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= działań ">m<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-elementowych. 

## Wzajemna odpowiedniość działań w zbiorach 

Przykład działań i zbiorów odpowiednich: 

* zbiór ">A = \{1, 2, 3\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* działania: 

| ">\bullet<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | 1 | 2 | 3 |
|-|-|-|-|
| **1** | 2 | 1 | 1 |
| **2** | 3 | 3 | 2 |
| **3** | 2 | 1 | 1 |

* zbiór ">B = \{a, b, c\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* działania: 

| ">*<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | a | b | c |
|-|-|-|-|
| **a** | b | a | a |
| **b** | c | c | b |
| **c** | b | a | a |

## Własności działań

Działanie ">\bullet<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= w zbiorze ">A<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= nazywamy: 

* __przemiennym__ jeśli dla każdej pary _a_, _b_ należących do zbioru _A_ zachodzi równość: ">a\bullet b = b\bullet a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\forall_{a,b \in A} a \bullet b = b \bullet a">

* __łącznym__ jeśli dla każdej trójki _a_, _b_, _c_ należących do _A_ zachodzi równość: ">(a \bullet b) \bullet c = a \bullet (b \bullet c)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\forall_{a, b \in A} (a \bullet b) \bullet c = a \bullet (b \bulletc)">

Przykłady działań niełącznych: 
* odejmowanie: ">(2 - 2) - 3 \neq 2 - (2 - 3)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=. 
* dzielenie. 

## Grupoid -- zbiór ">A<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= z działaniem ">\bullet<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Definicja: grupoid to zbiór ">A<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= z określonym działaniem ">\bullet<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=. 

Zapis: ">(A, \bullet)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Grupoid ">A<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest **przemienny**, jeśli działanie ">\bullet<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= w zbiorze ">A<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest **przemienne**. 

## Półgrupa 

Definicja: grupoid ">(A, \bullet)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= to **półgrupa**, jeśli działanie ">\bullet<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= w zbiorze ">A<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest **łączne**. 

## Element neutralny w zbiorze ">A<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Definicja: element ">1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= należący do ">A<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest neutralny, jeśli dla każdego elementu tego zbioru zachodzi równość ">a\bullet 1 = 1 \bullet a = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (wykonanie działania na dowolnym elemencie zbioru i elemencie neutralnym nie zmienia wartośći): 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\forall_{a \in A} a \bullet 1 = 1 \bullet a = a">

Przykłady

| Zbiór i działanie | El. neutr. | Sprawdzenie |
|-|-|-|
| ">(\mathbb{R},+)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= <br/>-- liczby rzeczywiste i dodawanie | ">0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">\forall_{a \in \mathbb{R}} a+0 = 0+a = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= |
| ">(\mathbb{R},\cdot)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= <br/>-- liczby rzeczywiste i mnożenie | ">1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">\forall_{a \in \mathbb{R}} a\cdot 1 = 1\cdot 1 = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= |

## Monoid

Definicja: monoid to półgrupa z
* jednością,
* działaniem łącznym 
* elementem neutralnym. 

## Inwers (element odwrotny)

Definicja: niech będzie grupoid ">A<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (dokładnie zbiór z działaniem: ">(A, \bullet)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=) z elementem neutralnym ">1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to element ">b \in A<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= nazywamy **odwrotnym**, jeśli dla każdego ">a \in A<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= zachodzi: ">a \bullet b = b \bullet a = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\forall_{a \in A} a\bullet b = b = \bullet a = 1">

Twierdzenie: w półgrupie (czyli grupie z działaniem łącznym) ">(A, \bullet)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= z elementem neutralnym ">1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= każdy element ma co najwyżej jeden element odwrotny lub nie ma go wcale. 

Dowód: niech 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a, b, c \in A"> 

oraz 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=1 = a \bullet b = b \bullet a = a \bullet c = c \bullet a"> 

(a więc ">b<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= i ">c<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= są odwrotne do ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=), wówczas można zapisać, że

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=b = b \bullet 1">

-- każdy element zbioru można zapisać jako działanie z elementem neutralnym, np. ">2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= można zapiać jako ">2 + 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= lub ">2 \cdot 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=.

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=b \bullet 1 = b \bullet (a \bullet c)">

-- skoro ">a \bullet c = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=.

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=b \bullet (a \bullet c) = (b \bullet a) \bullet c"> 

-- z prawa łączności. 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(b \bullet a) \bullet c = 1 \bullet c"> 

-- skoro ">b \bullet a = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=.

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=1 \bullet c = 1">

-- co było do udowodnienia?

# Wykład 3 (14.11.2020)

Od następnego zjazdu wykład od godz. 8.20

## Grupa

Wyznaczniki grupy ">A<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=:

* działanie grupy jest **łączne**;
* działanie posiada **element neutralny** ">1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, taki że ">\forall_{a \in A} a \bullet 1 = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (element neutralny działania ">\bullet<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= nie zmienia wartośći);
*
wykład od 8.20 do 9.-5

# Grupa (przypomnienie)

Grupa jeśli 3 warunki spełnione: 
- działanie jest łączne
- istnieje element neutralny działania
- każdy element ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= grupy ma **inwers** (element odwrotny) ">x<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= spełniający warunek:

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\forall_{a \in A} \exists_{x \in A} ax = xa = 1">

-- tzn. wykonanie działania na dowolnym elemencie grupy i inwersie daje w rezultacie element neutralny. Inwers możnamożemy inwers oznaczać jako ">a^{-1}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 

## Przykłady grup

* ">(\mathbb{C}, +, 0)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= --Największy zbiór: liczby zespolone z dodawaniem i zerem 

Sprawdzenie przemienności: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=">(CC, +, 0)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-(a + ib) = -a + i(-b)"><img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(a+ib) + (-a + i(-b)) = 0">

* L
Inny przykład: liczby rzeczywiste ">\mathbb{R}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=R z dodawaniem i zerem.

* LInny przykład: liczby wymierne ">\mathbb{Q}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Q z dodawaniem i zerem.

* LiczbyPrzykład: całkowite ">\mathbb{Z}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z z dodawaniem i zerem. 

* Liczby zespolone ">\mathbb{C}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Przykład: zespolone bez zera z, mnożeniem i, jednością: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(\mathbb{C} \setminus en 

(C\{0\}, \cdot, 1)">

* L*, 1)

Przykład: liczby rzeczywiste bez zera z, mnożeniem i, jednością: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(\mathbb{R} \setminus en

(R\{0\}, \cdot, 1)">

* Liczby*, 1)

Przykład: wymierne bez zera z, mnożeniem i jednością: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(\mathbb{Q} \setminus \{0\}, \cdot, 1)">

* Bijekcja ">B(X)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, gdzie ">X<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= to dowolny zbiór: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=B(X) - \{f : X \rightarrow X\}">

-- funkcja jest różnowartościowa (różnym wartościom przypisuje różne wartości z tego samego zbioru) i ma zbiór ">X<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=. 

Bijekcja posiada również funkcję odwrotną. 

* Permutacja

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=f = \Bigl(\begin{matrix} 1 & 2 & 3 \\ 2 & 1 & 3 \end{matrix}\Bigr)">

Odwrotność: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=f^{-1} = \Bigl (\begin{matrix} 1 & 2 & 3 \\ 2 & 1 & 3 \end{matrix}\Bigr)">

* Funkcja ">f(x) = x^3, x \in \mathbb{R}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=  

Funkcja jest różnowartościowa w zbiorze ">\mathbb{R}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=: ">f: \mathbb{R} \rightarrow \mathbb{R}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Funkcja odwrotna: ">f^{-1} = \sqrt[3]{x}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* Składanie funkcji: ">(B(X), \circ, 1_x)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Element neutralny -- funkcja identycznościowa ">1_x<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= taka, że ">1_x(x) = x<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Dowód: ">\forall_x (f \circ 1_x)(x) = f(1_x(x)) = f(x)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">f \circ 1_x =f<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">1_x \circ f = f<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* Permutacja 

Jeśli ">X<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest zbiorem wieloelementowym: ">X = \{1, 2, 3, ...., n \}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= i zamiast ">B(X)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= będziemy pisać ">P_n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (">B(X) := P_n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=), to zbiór wszystkich permutcji (bijekcji) zbioru ">n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-elementowego. 

Niech ">n = 5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=. 

Element neutralny: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=1 = \Bigl( \begin{matrix} 1 & 2 & 3 \\ 1 & 2 & 3 \end{matrix} \Bigr)">

Element odwrotny: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\alpha = \Bigl( \begin{matrix} 1 & 2 & 3 & 4 & 5 \\ 3 & 4 & 1 & 2 & 5 \end{matrix} \Bigr)">

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\alpha^{-1} = \Bigl( \begin{matrix} 1 & 2 & 3 & 4 & 5 \\ 3 & 4 & 1 & 2 & 5 \end{matrix} \Bigr)">

* Macierz kwadratowa stopnia 2

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=M_2 = \{ \Bigl[ \begin{matrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{matrix} \Bigr]: a_{11}, a_{12}, a_{21}, a_{22} \in \mathbb{R}(\mathbb{C} \}, *) ">

Element neutralny -- macierz jednostkowa: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=1 = \Bigl[ \begin{matrix} 1 & 0 \\ 0 & 1 \end{matrix} \Bigr] ">

Sprawdzenie:

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math= \Bigl[ \begin{matrix} 1 & 0 \\ 0 & 1 \end{matrix} \Bigr] \cdot \Bigl[ \begin{matrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{matrix} \Bigr] = \Bigl[ \begin{matrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{matrix} \Bigr]">

* Pełna grupa liniowa z mnożeniem">GL(2)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- takie macierze należące do ">M_2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, że wyznacznik jest niezerowy: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=GL(2) = \{ A \in M_2 : \det{A} \neq 0\}">

* ">Z_5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- wszystkie reszty z dzielenia liczby całkowitej przez ">5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Możliwe liczby: 0, 1, 2, 3, 4 (">Z_5 = \{0, 1, 2, 3, 4\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=.

Przyjmujemy oznaczenie: jeśli ">a \in Z<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to ">(a)_5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= może być resztą z dzielenia ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= przez ">5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, np. ">(10)_5 = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">(13)_5 = 3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Przyjmijmy działanie dodawanie modulo 5 ">+_5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, np. ">2 +_5 1 = (2+1)_5 = 3_5 = 3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, bo ">3 = 0 \cdot 5 + 3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">2 +_5 2 = 4<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">3 +_5 2 = (3+2)_5 = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=# Ćwiczenia 3 (14.11.2020)

## Przykłady grup c.d. 

* Dodawanie modulo 5 w zbiorze ">\{0,1,2,3,4\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Zbiór: ">Z_5 = \{0,1,2,3,4\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Działanie: ">a +_5 b = (a+b)_5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Sposób obliczania: ">a +_5 b = \begin{cases} a+b, & a+b<5 \\ a+b-5, & a+b >=5 \end{cases}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Wyniki: ">+_5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | 0 | 1 | 2 | 3 | 4
-|-|-|-|-|-
**0** |0|1|2|3|4
**1** |1|2|3|4|0
**2** |2|3|4|0|1
**3** |3|4|0|1|2
**4** |4|0|1|2|3

Elementy odwrotne (takie, które po zsumowaniu dadzą 5):

* dla 0 -- 0 (bo 5 nie należy do zbioru), 
* dla 1 -- 4 (zapis: ">-_5 1 = 4<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=) 
* dla 2 -- 3, 
* dla 3 -- 2, 
* dla 4 -- 1

* Ogólnie dla zbioru ">Z_n = \{0, 1, 2, ..., n-2, n-1\}, (n>1)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (zbiorami typu ">Z_1 = \{0\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= nie będziemy się zajmować)

Działanie dodawanie modulo ">n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=:: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a +_n b= (a_b)_n = \begin{cases} a+b, & a+b < n \\ a+b-n, & a+b >=n \end{cases} ">

Element neutralny działania ">+_n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=: ">0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Element przeciwny ">-_n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=: 
 
* ">-_n 0 = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* ">-_n k =  n-k, k > 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=## Zadania 

1. Sprawdzić, czy dane działanie jest przemienne, łączne i czy posiada element neutralny, a jeśli tak, to znaleźć elementy odwrotne.  

* Zbiór: ">\mathbb{R}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* Działanie: ">a \circ b = a+b+3, a \in \mathbb{R}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Wynik ">a \circ b<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= należy do ">\mathbb{R}<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=. 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1\degree"> Działanie jest przemienne, bo dodawanie jest przemienne:">b \circ a = b + a + 3<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=Korzystamy z przemienności dodawania: ">b + a + 3 = a + b + 3 = a \circ b<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math= (q.e.d)

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2\degree"> Sprawdzenie łączności:">(a \circ b) \circ c = (a + b + 3) \circ c = a + b + c + 6<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math= 

Korzystamy z przemienności:">a \circ (b \circ c) = a \circ (b + c + 3) = a + b + c + 6 = (a \circ b) \circ c<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(q.e.d.)

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=3\degree"> Sprawdzenie elementu neutralnego">a \circ x = a \Leftrightarrow x = -3<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=">x \circ b = b \Leftrightarrow x = -3##

Element neutralny: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-3">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=4\degree"> Elementy przeciwne:

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a \circ x = -3">
<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a + x + 3 = -3 /-3">
<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a + x = -6 - a">
<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=x = -6 - a">

Ogólny wzór na element przeciwny do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a">: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x = -6 - a">

Sprawdzenie: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a \circ -6 -a = a + -6 -a +3 = -3">

A <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-3"> to element neutralny. 

Mamy więc do czynienia z grupą przemienną (tzw. abelową). 

---

2. Sprawdzić, czy dane działanie jest przemienne, łączne i czy posiada element neutralny, a jeśli tak, to znaleźć elementy odwrotne.  

Działanie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ b = a + b + ab">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1\degree"> Działanie jest przemienne, bo dodawanie i mnożenie jest przemienne. 

Sprawdzenie

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=L = a \circ b = a + b + ab">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=P = b \circ a = b + a + ba">

Pytanie, czy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=L = P">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=P = b \circ a = b + a + ba = a + b + ab = a \circ b = L">

(q.e.d.)

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2\degree"> Sprawdzenie, czy działanie jest łączne: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=L = (a \circ b) \circ c">
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=P = a \circ (b \circ c)">

Pytanie, czy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=L = P">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=P = a \circ (b \circ c) \\= a \circ (b + c + bc)\\ = a + (b + c + bc) + a(b+c+bc)\\ = a + b + c + bc + ab + ac + abc\\ = a + b + c + ab + bc + ac + abc">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=L = (a \circ b) \circ c\\ = (a + b +ab) \circ c\\ = (a+b+ab) + c + c(a+b+ab) \\= a + b + ab + c + ca +cb + cab \\= a + b + c + ab + bc + ac + abc = P">

(q.e.d.)

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=3\degree"> Element neutralny <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x">: 

Z definicji <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ x"> powinno się równać <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a">, a więc:

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ x = a">
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a + x + ax = a / -a">
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x + ax = 0">
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x(1+a) = 0 / \frac{1}{1+a}">
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x = 0">

Element neutralny: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0">

Sprawdzenie: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ 0 = a">
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a + 0 + 0\cdot a = a">
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a = a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=4\degree"> Element odwrotny <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x">

Z definicji elementu odwrotnego, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ x"> powinno dać element neutralny, czyli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0">, a więc: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ x = 0">
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a + x +ax = 0 / -a">
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x + ax = -a">
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x(1+a) = -a / \frac{1}{1+a}">
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x = \frac{-a}{1+a}">

Element odwrotny do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> to <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\frac{-a}{1+a}">

Sprawdzenie: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ \frac{-a}{1+a} = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a + \frac{-a}{1+a} + a\cdot \frac{-a}{1+a} = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\frac{a(1+a) - a - a^2}{1+a} = 0 / \frac{1}{1+a}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a+a^2-a-a^2 = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a - a + a^2 - a^2 = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0 = 0">

(q.e.d.)

# Wykład 4 | 28.11.2020

## Zadania c.d.

3. Sprawdzić, czy dane działanie jest przemienne, łączne i czy posiada element neutralny, a jeśli tak, to znaleźć elementy odwrotne.  

Zbiór: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{R_+}"> -- liczby rzeczywiste większe do zera. 

Działanie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\circ"> zdefiniowane jako: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a \circ b = (\sqrt[3]{a} + \sqrt[3]{b})^3">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1\degree"> Sprawdzenie przemienności -- działanie jest przemienne, bo dodawanie jest przemienne. 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2\degree"> Sprawdzenie łączności: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=L = (a \circ b) \circ c = (\sqrt[3]{a} + \sqrt[3]{b})^3 \circ c\\=(\sqrt[3]{(\sqrt[3]{a} + \sqrt[3]{b})^3} + \sqrt[3]{c})^3\\=(\sqrt[3]{a} + \sqrt[3]{b} + \sqrt[3]{c})^3">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=P = a \circ (b \circ c) = a \circ (\sqrt[3]{b} + \sqrt[3]{c})^3\\=(\sqrt[3]{a} + \sqrt[3]{(\sqrt[3]{b} + \sqrt[3]{c})^3})^3\\=(\sqrt[3]{a}+\sqrt[3]{b}+\sqrt[3]{c})^3 = L">

(q.e.d.)

A więc działanie jest łączne. 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=3\degree"> Element neutralny <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x">

Z definicji: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ x = a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(\sqrt[3]{a} + \sqrt[3]{x})^3 = a /\sqrt[3]{}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\sqrt[3]{a} + \sqrt[3]{x} = \sqrt[3]{a}  / -\sqrt[3]{a}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\sqrt[3]{x} = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x = 0">

Element neutralny: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=4\degree"> Element odwrotny do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a">

Z definicji <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ a^{-1} = e">, gdzie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=e"> jest elementem neutralnym. A więc: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ a^{-1} = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(\sqrt[3]{a} + \sqrt[3]{a^{-1}})^3 = 0 / \sqrt[3]{}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\sqrt[3]{a} + \sqrt[3]{a^{-1}} = 0 / -\sqrt[3]{a}"> 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\sqrt[3]{a^{-1}} = -\sqrt[3]{a} /^3">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a^{-1} = -a">

A więc element odwrotny do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> to <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-a">. 

Sprawdzenie: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ -a = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(\sqrt[3]{a} + \sqrt[3]{-a})^3 = 0 / \sqrt[3]{}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\sqrt[3]{a} - \sqrt[3]{a} = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0 = 0">

(q.e.d.)

---

4. Sprawdzić, czy dane działanie jest przemienne, łączne i czy posiada element neutralny, a jeśli tak, to znaleźć elementy odwrotne.  

Zbiór: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{R^+}"> (dodatnie liczby rzeczywiste.

Działanie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \diamond b = 5^{\log_5{a} \cdot \log_5{b}}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1\degree"> Sprawdzenie przemienności.

Z własności logarytmów możemy zapisać: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math==5^{ \log_5{b} \cdot \log_5{a} } = b \diamond a"> 

A zatem działanie jest przemienne.

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2\degree"> Sprawdzenie łączności. 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=L = (a \diamond b) \diamond c = (5^{\log_5{a} \cdot \log_5{b}}) \diamond c= 5^{\log_5{5^{\log_5{a} \cdot \log_5{b}}} \cdot \log_5{c}}">

Korzystając z własności logarytmu: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\log_n{x^\alpha} = \alpha \cdot \log_n{x}">: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=L = 5^{{\log_5{a} \cdot \log_5{b} } \cdot \log_5{5} \cdot \log_5{c}}"> 

Usuwamy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\log_5{5} = 1">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=L = 5^{\log_5{a} \cdot \log_5{b} \cdot \log_5{c}}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=P = a \diamond (b \diamond c) = a \diamond (5^{\log_5{b} \cdot \log_5{c}}) = 5^{\log_5{a} \cdot \log_5{5^{\log_5{b} \cdot \log_5{c}}}}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=P = 5^{\log_5{a} \cdot \log_5{5} \cdot \log_5{b} \cdot \log_5{c}}">

Usuwamy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\log_5{5} = 1">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=P = 5^{\log_5{a} \cdot \log_5{b} \cdot \log_5{c}} = L">

(q.e.d.)

A więc działanie jest łączne. 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=3\degree"> Element neutralny 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \diamond e = a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5^{\log_5{a} \cdot \log_5{e}} = a"> (logarytmujemy obustronnie)

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\log_5{5^{\log_5{a} \cdot \log_5{e}}} = \log_5{a}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\log_5{a} \cdot \log_5{e} \cdot \log_5{5} = \log_5{a}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\log_5{a} \cdot \log_5{e} = \log_5{a} / \frac{1}{\log_5{a}}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=log_5{e} = 1 \Leftrightarrow 5^1=e">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=e = 5">

Sprawdzenie: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \diamond 5 = a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5^{\log_5{a} \cdot \log_5{5}} = a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5^{(\log_5{a}) \cdot 1} = a">

Z własności logarytmu: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a^{\log_a{b}} = b">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a = a">

(q.e.d.)

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=4\degree"> Element odwrotny do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a">

Z definicji elementu odwrotnego: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \diamond a^{-1} = e">, gdzie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=e"> jest elementem neutralnym. A więc: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \diamond a^{-1} = 5 = 5^1">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5^{\log_5{a} \cdot \log_5{a^{-1}}} = 5 = 5^1">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\log_5{a} \cdot \log_5{a^{-1}} = 1">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\log_5{a} \neq 0">, a zatem <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \neq 1">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\log_5{a} = 1"> oraz <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\log_5{a^{-1}} = 1">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a = 5"> oraz <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a^{-1} = 5 = a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a = a^{-1}">

Działanie nie ma zatem elementu odwrotnego, a więc <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(\mathbb{R^+}, \diamond, 5)"> nie jest grupą. 

# Ćwiczenia 4 | 28.11.2020 

## Podgrupa 

Definicja: niepusty podzbiór <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H"> grupy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G"> nazywamy **podgrupą** grupy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G">, jeśli sam jest grupą, a więc musi spełniac warunki: 

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1 \in H"> -- musi mieć element neutralny,
* działanie w tym zbiorze musi być przemienne; 

a dodatkowo dla każdego elementu <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H"> musi istnieć jego inwers (element przeciwny): 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\forall_{a \in H} a^{-1} \in H">

## Przykłady podgrup

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G=Z_4"> z dodawaniem modulo 4 <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(+_4)">

---

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(Q\{0\}, \circ, 1)">

---

* Liczby całkowite z mnożeniem nie są podgrupą, bo <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\frac{1}{\mathbb{Z}}"> nie należy od zbioru liczb całkowitych.

---

* Bijekcja <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=B(X)"> (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=X"> to dowolny zbiór), zdefiniowana jako funkcja przepisująca elementy zbioru w ten sam zbiór:  

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=B(X) \{f : X \rightarrow X: f\}">

Bijekcja <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=B"> jest różnowartościowa i ma zbiór <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=X">. 

Przykład: 

zbiór <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=X"> ---  zbiór <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=X"> 
1 <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\rightarrow"> 2
2 <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\rightarrow"> 1
3 <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\rightarrow"> 3

-- różnym wartościom przypisane są różne wartości; wszystkie elementy zbioru <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=X"> są wykorzystane. 

Funkcję <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=f"> można pokazać jako permutację: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=f = \Bigl( \begin{matrix} 1 & 2 & 3 \\ 2 & 1 & 3 \end{matrix} \Bigr)">

Odwrotność (funkcja odwrotna): 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=f^{-1} = \Bigl( \begin{matrix} 1 & 2 & 3 \\ 2 & 1 & 3 \end{matrix} \Bigr)">

---
 
* Funkcja <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=f(x) = x^3, x \in \mathbb{R}">

Funkcja jest różnowartościowa w zbiorze <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{R}">: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=f: \mathbb{R} \rightarrow \mathbb{R}">

Wykres

<iframe src="https://www.desmos.com/calculator/3sdsbko0ew?embed" width="500px" height="500px" style="border: 1px solid #ccc" frameborder=0></iframe>

Funkcja odwrotna: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=f^{-1} = \sqrt[3]{x}">

---

* Składanie funkcji <img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(B(X), \circ, 1_x)">

Symbol działania: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\circ">

Element neutralny -- funkcja identycznościowa <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1_x">, gdzie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1_x(x) = x">

Sprawdzenie: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(f \circ 1_x)(x) = f( 1_x(x) ) = f(x)">  dla każdego <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=f \circ 1_x =f">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1_x \circ f = f">

---

* Permutacja (bijekcja)

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=X"> jest zbiorem wieloelementowym (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=X = \{1, 2, 3, ...., n \}">)

Zamiast <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=B(x)"> możemy pisać <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=P_n">: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=B(X) := P_n">

Niech <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n = 5">

Element neturalny <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1">:

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=1 = \Bigl( \begin{matrix} 1 & 2 & 3 & 4 & 5 \\ 1 & 2 & 3 & 4 & 5 \end{matrix} \Bigr)">

Zbiór wszystkich permutacji (bijekcji) zbioru n-elementowego

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\alpha = \Bigl( \begin{matrix} 1 & 2 & 3 & 4 & 5 \\ 3 & 4 & 1 & 2 & 5 \end{matrix} \Bigr)">

Element odwrotny: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\alpha^{-1} = \Bigl( \begin{matrix} 1 & 2 & 3 & 4 & 5 \\ 3 & 4 & 1 & 2 & 5 \end{matrix} \Bigr)">

---

* Macierz kwadratowa stopnia 2.

Zbiór wszystkich macierzy: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=M_2 = \{ [ a_{11} a_{12} a_{21} a_{22}] : a_{11}, a_{12}, s_{21}, s_{22} \in \mathbb{R}(\mathbb{C}), *)">

Element neutralny -- macierz jednostkowa

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=1 = \Bigl[ \begin{matrix} 1 & 0 \\ 0 & 1 \end{matrix} \Bigr]">

Sprawdzenie:

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\Bigl[ \begin{matrix} 1 & 0 \\ 0 & 1 \end{matrix} \Bigr] \cdot \Bigl[ \begin{matrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{matrix} \Bigr] = \Bigl[ \begin{matrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{matrix} \Bigr]">

---

* Pełna grupa liniowa z mnożeniem

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=GL(2)"> -- takie macierze należące do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=M_2">, że ich wyznacznik jest niezerowy: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=GL(2) = \{ A \in M_2 : \det{A} \neq 0 \}">

---

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z_5, +_5"> -- wszystkie reszty z dzielenia liczby całkowitej przez <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5">

Możliwe liczby: 0, 1, 2, 3, 4

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=Z_5 = \{0, 1, 2, 3, 4\}">

Przyjmujemy oznaczenie: jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a\in Z">, to <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(a)_5"> może być dowolną liczbą naturalną i resztą z dzielenia <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> przez <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5">, np. 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(10)_5 = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(13)_5 = 3">

Przyjmijmy działanie dodawanie modulo 5 <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=+_5"> takie, że jeśli
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a +_5 b = (a + b)_5">

Przykłady

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2 +_5 1 = (2+1)_5 = 3_5 = 3"> (bo <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=3 = 0 \cdot 5 + 3">)

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2 +_5 2 = 4">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=3 +_5 2 = (3+2)_5 = 0">

---

* Dodawanie modulo 5 (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=+_5">): <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a +_5 b = (a+b)_5">

Zbiór: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z_5 = {0,1,2,3,4}">

Sposób obliczania:

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\begin{cases} a + b, & a + b < 5 \\ a + b - 5, &a + b \geq 5 \end{cases}">

Działania

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=+_5"> | 0 | 1 | 2 | 3 | 4
-|-|-|-|-|-
**0** |0|1|2|3|4
**1** |1|2|3|4|0
**2** |2|3|4|0|1
**3** |3|4|0|1|2
**4** |4|0|1|2|3

Elementy odwrotne: (takie, że suma da 5): 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-_5 0 = 0"> (bo 5 nie należy do zbioru)
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-_5 1 = 4">
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-_5 2 = 3">
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-_5 3 = 2">
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-_5 4 = 1">

----

* Ogólnie dodawanie modulo <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n"> w zbiorze <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z_n = \{0, 1, 2, ..., n-2, n-1\}, (n>1)">

Zbiorem <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z_1 = {0}"> nie będziemy się zajmować

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a +_n b = (a+b)_n = \begin{cases} a + b, & a + b < n \\ a + b - n,& a+b \geq n \end{cases}">

Element neutralny działania <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=+_n">: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0">

Element przeciwny: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-_n"> 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-_n 0 = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-_n k =  n-k   , k > 0">

----

## Zadania

1. Sprawdzić, czy dane działanie jest przemienne, łączne i czy posiada element neutralny, a jeśli tak, to znaleźć elementy odwrotne. 

Zbiór: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{R}">

Działanie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ b = a+b+3, a \in \mathbb{R}">, wynik <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ b"> należy do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{R}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1\degree"> Działanie jest przemienne, bo dodawanie jest przemienne:

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b \circ a = b + a + 3">

Korzystam z przemienności dodawania:

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b + a + 3 = a + b + 3 = a \circ b">

(q.e.d)

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2\degree"> Sprawdzenie łączności:

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(a \circ b) \circ c = (a + b + 3) \circ c = a + b + c + 6">

Korzystam z przemienności

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ (b \circ c) = a \circ (b + c + 3) = a + b + c + 6 = (a \circ b) \circ c"> 

(q.e.d.)

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=3\degree"> Sprawdzenie elementu neutralnego:

Z definicji <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ x = a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a + x + 3 = a / -a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x + 3 = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x = -3">

Element neutralny: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-3">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=4\degree"> Elementy przeciwne:

Z definicji <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ a^{-1} = e">, gdzie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=e"> to element neutralny.

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ a^{-1} = -3">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a + a^{-1} + 3 = -3 / -3">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a + a^{-1} = -6 /-a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a^{-1} = -6 - a"> (ogólny wzór na element przeciwny) 

Sprawdzenie: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ -6 -a = a + -6 -a +3 = -3 = e">

Mamy zatem do czynienia z grupą przemienną (abelową).

## Zadanie domowe

Sprawdzić, czy dane działanie jest przemienne, łączne i czy posiada element neutralny, a jeśli tak, to znaleźć elementy odwrotne. 

Działanie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ b = a + b + ab">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1\degree"> Sprawdzenie przemienności 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=L = a \circ b = a + b + ab">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=P = b \circ a = b + a + ba">

Korzystam z przemienności dodawania i mnożenia: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=L = b + a + ba = P">

(q.e.d.)

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2\degree"> Sprawdzenie łączności

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(a \circ b) \circ c \\= (a + b + ab) \circ c \\= (a + b + ab) + c + c(a + b + ab) \\=a + b + c + ab + ac + bc + abc">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ (b \circ c) \\=a \circ (b + c + cb) \\= a + (b + c +cb) + a(b + c + bc) \\=a + b + c + ab + ac + bc + abc\\=(a \circ b) \circ c">

(q.e.d)

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=3\degree"> Element neutralny <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=e">

Z definicji <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ e = a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a + e + ae = a /-a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=e + ae = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=e(1 + a) = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=e = 0">

Sprawdzenie: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ 0 = a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a + 0 + a\cdot 0 = a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a + 0 = a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a = a">

(q.e.d.)

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=4\degree"> Element odwrotny <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a^{-1}"> 

Z definicji <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ a^{-1} = e">, gdzie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=e"> to element neutralny.

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ a^{-1} = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a + a^{-1} + aa^{-1} = 0 / -a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a^{-1} + aa^{-1} = -a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a^{-1}(1 + a) = -a / \frac{1}{1+a}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a^{-1} = \frac{-a}{1+a}">

Sprawdzenie

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ \frac{-a}{1+a} = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a + \frac{-a}{1+a} + a\frac{-a}{1+1} = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\frac{a(1+a) + ( -a) + ( -a^2)}{1+a} = 0/(1+a)">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a+a^2-a-a^2 = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0=0">

(q.e.d.)

# ???Wykład 4 | 28.11.2020

## Zadania c.d.

1. Sprawdzić, czy dane działanie jest przemienne, łączne i czy posiada element neutralny, a jeśli tak, to znaleźć elementy odwrotne.

Zbiór: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{R}^+">

Działanie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\circ">

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a \circ b = (\sqrt[3]{a} + \sqrt[3]{b})^3">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1\degree"> Sprawdzenie przemienności -- działanie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\circ"> jest przemienne, bo dodawanie jest przemienne. 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2\degree"> Sprawdzenie łączności

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(a \circ b) \circ c \\= (\sqrt[3]{a} + \sqrt[3]{b})^3 \circ c \\= (\sqrt[3]{(\sqrt[3]{a} + \sqrt[3]{b})^3} + \sqrt[3]{c})^3 \\= (\sqrt[3]{a} + \sqrt[3]{b} + \sqrt[3]{c})^3">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ (b \circ c) \\=a \circ (\sqrt[3]{b} + \sqrt[3]{c})^3 \\=(\sqrt[3]{a} + \sqrt[3]{(\sqrt[3]{b} + \sqrt[3]{c})^3})^3 \\=(\sqrt[3]{a} + \sqrt[3]{b} + \sqrt[3]{c})^3 \\=(a \circ b) \circ c">

A więc działanie jest łączne.

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=3\degree"> Element neutralny <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=e">

Z definicji <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ e = a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(\sqrt[3]{a} + \sqrt[3]{e})^3 = a /\sqrt[3]{}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\sqrt[3]{a} + \sqrt[3]{e} = \sqrt[3]{a} /-\sqrt[3]{a}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\sqrt[3]{e} = 0 /^3">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=e = 0">

Element neutralny: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0">

Sprawdzenie: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ 0 = a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(\sqrt[3]{a} + \sqrt[3]{0})^3 = a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(\sqrt[3]{a} + 0)^3 = a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(\sqrt[3]{a})^3 = a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a = a">

(q.e.d.)

Mając element neutralny, możemy mówić o elemencie odwrotnym.

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=4\degree"> Element odwrotny <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a^{-1}">

Z definicji <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ a^{-1} = e">, gdzie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=e"> jest elementem neutralnym. 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ a^{-1} = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(\sqrt[3]{a} + \sqrt[3]{a^{-1}})^3 = 0 /\sqrt[3]{}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\sqrt[3]{a} + \sqrt[3]{a^{-1}}=0 /-\sqrt[3]{a}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\sqrt[3]{a^{-1}} = -\sqrt[3]{a} /^3">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a^{-1} = -a"> (ogólny wzór na element odwrotny)

Sprawdzenie: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ -a = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(\sqrt[3]{a} + \sqrt[3]{-a})^3 = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(\sqrt[3]{a} - \sqrt[3]{a})^3 = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(0)^3 = 0">

(q.e.d.)

-------

2. Sprawdzić, czy dane działanie jest przemienne, łączne i czy posiada element neutralny, a jeśli tak, to znaleźć elementy odwrotne.

Zbiór: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{R}^+">

Działanie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\circ">

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a \circ b = 5^{log_5{a} \cdot log_5{b}}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1\degree"> Sprawdzenie przemienności 

Mnożenie jest przemienne, a więc: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ b\\=5^{\log_5{a} \cdot \log_5{b}} \\=5^{\log_5{b} \cdot \log_5{a}} \\=b \circ a">

jest przemienne.

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2\degree"> Sprawdzenie łączności 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(a \circ b) \circ c \\= (5^{\log_5{a} \cdot \log_5{b}}) \circ c \\= 5^{\log_5(5^\log_5{a} \cdot \log_5{b}) \cdot \log_5{c}}">

Z własności logarytmu wiemy, że: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\log_5{x^\alpha} = \alpha \cdot \log_5{x}">

Z zatem

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5^{\log_5{a} \cdot \log_5{b} \cdot \log_5{5} \cdot \log_5{c}} \\= 5^{log_5{a} \cdot \log_5{b} \cdot \log_5{c}}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=3\degree"> Element neutralny <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=e">

Z definicji elementu neutralnego: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ e = a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5^{\log_5{a} \cdot log_5{e}} = a /\log_5{}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\log_5{5^{\log_5{a} \cdot \log_5{e}}} = \log_5{a}">

Z definicji logarytmu <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\log_a{x} = y \leftrightarrow a^y=x">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5^{\log_5{a}} = 5^{\log_5{a} \cdot \log_5{e}}">

A więc: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\log_5{a} = \log_5{a} \cdot \log_5{e} /\frac{1}{\log_5{a}}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\log_5{e} = 1">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5^1 = e = 5">

Sprawdzenie: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5^{\log_5{a} \cdot \log_5{5}} = a/\log_5{}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\log_5{5^{\log_5{a} \cdot \log_5{5}}} = \log_5{a}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5^{\log_5{a}} = 5^{\log_5{a} \cdot \log_5{5}}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\log_5{a} = \log_5{a} \cdot \log_5{5} /\frac{1}{\log_5{a}}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1 = \log_5{5}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5^1 = 5">

(q.e.d)

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=4\degree"> Element przeciwny <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a^{-1}">

Z definicji <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ a^{-1} = e">, gdzie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=e"> to element neutralny. 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5^{\log_5{a} \cdot \log_5{a^{-1}}} = 5">

Z własności potęgowania <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(a^x)^y = a^{x\cdot y}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(5^{\log_5{a}})^{\log_5{a^{-1}}} = 5">

Z własności logarytmów: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a^{\log_a{b}} = b">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a^{\log_5{a^{-1}}} = 5">

Z własności logarytmów: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a^{\log_c{b}} = b^{\log_c{a}}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(a^{-1})^{\log_5{a}} = 5">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a^{-1} = 5^{\frac{1}{\log_5{a}}}">

Sprawdzenie: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5^{\log_5{a} \cdot \log_5{5^{\frac{1}{\log_5{a}}}}} = 5">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5^{\log_5{a} \cdot \log_5{5^{\frac{1}{\log_5{a}}}}} = 5^1">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\log_5{a} \cdot \log_5{5^{\frac{1}{\log_5{a}}}} = 1">

Z własności logarytmów: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\log_a{x^y} = y\log_a{x}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\log_5{a} \cdot \frac{1}{\log_5{a} } \log_5{5} = 1">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1 \cdot 1 = 1">

(q.e.d.)

-------------------

# ???Ćwiczenia 4 | 28.11.2020 

## Podgrupa 

Definicja: niepusty podzbiór <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H"> grupy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G"> nazywamy **podgrupą** grupy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G">, jeśli sam jest grupą.

## Przykłady podgrup

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G=Z_4"> z dodawaniem modulo 4 <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(+_4)">

Na ogół podzbiórami są elementy z 1 elementem i równe innej grupie. 

## Twierdzenie Lagrange'a

Niech <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H"> będzie podgrupą grupy skończonej <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G"> (tzn. <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G"> ma skończoną liczbę elementów), wówczas liczba elementów (tzw. rząd) grupy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H"> dzieli liczbę elementów grupy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G">.

Np. jeśli grupa <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G"> ma 12 elementów, to wówczas podgrupa <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H"> grupy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G"> ma 12, 1, 6, 2, 3, 4 elementów.

## Warstwy lewo- i prawostronne grup

Oznaczenia: 

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G"> to grupa, 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H"> -- podgrupa grupy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G">, 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> -- element należący do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G"> (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \in G">), 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=aH"> -- zbiór elementów <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a\cdot h"> takich, że <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=h"> przebiega przez <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H">:
 
<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=aH = \{ a \cdot h : h \in H\}">

Np. <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H = \{0,2\}">
to <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0 +_4 H = \{0, 2\}">
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1 +_4 H = \{1, 3\}">
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2 +_4 H = \{2, 0\}"> 
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=3 +_4 H = \{3, 1\}"> 

Taki zbiór nazywamy **warstwą lewostronną** (bo <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> jest po lewej) grupy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G"> wyznaczoną przez element <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> i podgrupę <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H">. 

A taki zbiór:

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=Ha= \{h \cdot a : h \in H\}">

-- nazywamy **warstwą prawostronną** grupy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G"> wyznaczoną przez element <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> i podgrupę <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H">

Dla <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a = 1">, to <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \cdot H = 1 \cdot H = H \cdot 1 = H"> 

Warstwy mają tyle samo elementów co grupa

## Przykłady

* Niech będzie grupa <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a">

Weźmy funkcję 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=L_a: H \rightarrow aH">

gdzie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=L_a (h) = a \cdot h, h \in H"> 

Zauważamy, że <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=L_a"> jest różnowartościowa, bo jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=L_a(h) = L_a(h')">, to wówczas <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=ah = ah' |a^-1">, a zatem <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a{^-1} a h = a^{-1} a h'">, czyli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=h = h'">. A więc <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=L_4"> jest na zbiór <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=aH">. 

Mamy tu bijekcję, tzn. wzajemne dopasowanie elementów grupy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H"> i zbioru <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=aH">. 

W przypadku zbiorów skończonych wszystkie warstwy mają tyle samo elementów co odpowiadająca im grupa. 

Np. <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=aH"> ma tyle samo elementów co <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H"> i tyle samo co <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Ha">. 

---

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z_4, H = \{0,2\}">

Warstwy: 

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0 +_4 H = \{0, 2\} = 2 +_4 H">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1 +_4 H = \{1, 3\} = 3 +_4 H">

Mamy zatem 2 warstwy 

0	| 	1
2	| 	3

Warstwy te są rozłączne, co wynika z innego twierdzenia:

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=aH \cap bH \neq \emptyset \rightarrow aH = bH">

bo nie może być tak, żeby jakiś element był częścią wspólną 

## Dowód rozłączności warstw

Założenie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x \in aH \cap bH">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(?) aH \neq bH">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x \in aH \cap bH">, a stąd wynika, że <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=( \exists h_1, h_2 \in H)(x ah_1 = ab_2)">

Dowód <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=aH \neq bH">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=y = aH \rightarrow (\exists h \in H)(y = ah)">

Podstawiamy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a = bh_2 h_1^{-1}">

Więc <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=y = bh_1 h_1^{-1} h \in bH">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=bh_1 h_1^{-1} h \in H">

A więc, gdy mamy grupę. 

---

## Przykłady warstw podgrup c.d.

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G">, podrupa <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H">

Warstwy

|H||||
|-|-|-|-|
| a|d|g|j|
| b|e|h|k|
|c|f|i|l|

A więc warstwa jest wielokrotnością wielokrotność elementów grupy. 

Wnioski z twierdzenia

1) Ilość elementów grupy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G"> (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=|G|">):

Jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=|G| = p"> (liczba pierwsza), to <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G"> ma tylko 2 podgrupy: 

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H_1 = G">, 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H_2 = \{1\}"> (element neutralny) 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z_2">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z_5">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z_3">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z_7">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z_11"> itd. -- wszystkie one nie mają wlaściwych (definicyjnych) podgrup. 

2) Niech będzie grupa <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z_12">, to mamy podgrupy o liczbach elementów: 1, 12, 2, 6, 3, 4. 

Pytanie, czy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z"> ma podgrupę 2 elementową -- dzielimy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z"> na 2 i mamy 6, a 6 jest w zbiorze, więc <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=12:6 = 2">, a więc mamy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=[0,2]">. 

Wniosek: w grupie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z_e"> dla każdego dzielnika istnieje dokładnie 1 podgrupa 

# Ćwiczenia 5 | 05.12.2020

## Kolokwium za 2 tyg., godz. 8.00

## Zadania

1. Znaleźć wszystkie podgrupy (właściwe, tzn. nietrywialne) grup: 

a) <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(Z_{24}, +_{24}, 0)"> różne od całego <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z_{24}"> oraz <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\{0\}">

b) <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(Z_{36}, +_{36}, 0)"> różne od całego <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z_{36}"> oraz <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\{0\}">

---

Ad a

Podgrupa ma tyle elementów, ile jest dzielników właściwych liczby elementów. 

A więc dzielniki 24: 1, 24 (te nas nie interesują), 2, 12, 3, 8, 4, 6. 

* 2-elementowa podgrupa: dzielimy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=24 / 2">, mamy 12, podgrupa <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H_2 = \{0, 12}\">

* 12-elementowa podgrupa: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=24 / 12 = 2"> -- <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H_{12} = \{0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22\}"> (co 2).

* 3-elementowa podgrupa: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=24 / 3 = 8"> -- <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H_3 = \{0, 8, 16\}">

* 8-elementowa podgrupa: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=24 / 8 = 3"> -- <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H_8 = \{0, 3, 6, 9, 12, 15, 18, 21\}">

* 4-elementowa podgrupa: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=24 / 4 = 6"> -- <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H_4 = \{0, 6, 12, 18\}">

* 6-elementowa podgrupa: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=24 / 6 = 4"> -- <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H_6 = \{0, 4, 8, 12, 16, 20\}">

---

Ad b

Liczba elementów grupy: 36 

Dzielniki: 1, 36 (te nas nie interesują), 2, 18, 3, 12, 4, 9, 6,

Istnieje zatem 7 właściwych podgrup:

* 2-elementowa: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=36/2 = 18"> -- <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H_2 = \{0, 18\}">
* 18-elementowa: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=36/18 = 2"> -- <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H_{18} = \{0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34\}">
* 3-elementowa: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=36/3 = 12"> -- <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H_3 = \{0, 12, 24\}">
* 12-elementowa: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=36/12 = 3"> -- <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H_{12} = \{0, 3, 6, 9, 12, 15, 18, 21, 24, 27, 30, 33\}">
* 4-elementowa: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=36/4 = 9"> -- <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H_4 = \{0, 9, 18, 27\}">
* 9-elementowa: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=36/9 = 4"> -- <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H_9 = \{0, 4, 8, 12, 16, 20, 24, 26, 32\}">
* 6-elementowa: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=36/6 = 6"> -- <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H_6 = \{0, 6, 12, 18, 24, 30\}"> 

## Generatory podgrup

2. Znaleźć wszystkie podgrupy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(\mathbb{Z}, +, 0)"> (całkowite, z dodawaniem i elementem neutralnym) 

2 podgrupy są trywialne: 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\{0\}"> -- tylko zero (dodawanie 0 do 0 zawsze da 0, więc nie wyjdziemy poza zbiór, 0 też jest elementem neutralnym dodawania), 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Z}"> -- wszystkie liczby całkowite.

Jeśli do podgrupy weźmiemy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1">, to automatycznie musimy też dodać <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0"> (element neutralny) oraz <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-1"> (inwers), a dalej cały zbiór liczb całkowitych (dwie jedynki dają <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2">, trzy jedynki -- <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=3"> itd.). 

Jeśli do podgrupy weźmiemy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2">, to musi się w niej znaleźć także <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0"> i <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-2">, a także <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=4"> i <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-4">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=6"> i <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-6"> itd.

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2"> w powyższych przykładach to **generatory** podgrup: 

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=<1> = <-1> = \mathbb{Z}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=<2> = <-2> = \{0, 2, -2, 4, -4, ...\} = 2 \cdot \mathbb{Z}">
* trójka generuje: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=<3> = \{0, 3, -3, 6, -6...\} = 3 \cdot \mathbb{Z}">

Ogólnie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n \cdot \mathbb{Z}"> to zbiór wielokrotności <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n">, (bo <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n = 0, 1, 2...">). 

Każdy zbiór wielokrotności jakiejś liczby to jest podgrupa dla każdej liczby naturalnej. 

Podgrupa zerowa to <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\{0\} = 0 \cdot \mathbb{Z}">

Podgrupa równa grupie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Z} = 1 \cdot \mathbb{Z}">

## Dowód, że nie ma innych podgrup <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Z}"> niż te złożone z wielokrotności poszczególnych liczb całkowitych

Jeśli wezmę grupę <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H \notin \{0\}">, to w tym zbiorze 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(\exists k \in \mathbb{Z}, k \neq 0) (k \in H)">

-- jeśli jakaś liczba należy do grupy, to z tego wynika, że moduł <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=k"> należy do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H">, a moduł z <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=k"> to liczba naturalna (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=|k| \in H, |k| \in \mathbb{N}">)

A skoro tak, to taki zbiór liczb naturalnych ma element najmniejszy. Oznaczmy go jako <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n"> -- najmniejsza liczba naturalna należąca do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H">. 

A powiedzieliśmy wcześniej, że <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n \dot \mathbb{Z} \in H">

Dowód na to, że innych podgrup liczb całkowitych nie ma: 

Jeśli wezmę jakieś <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=m \in H">, to mogę podzielić zbiór <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H"> tak, że 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=m = qn + r, 0 \leq r < n">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=r = m - qn, (m, q \in H)">

Ale <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n"> miało być najmniejszą liczbą naturalną, a skoro <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=r \in H"> i <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=r < n">, to <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=r = 0">

Więc <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=m = qn \in n\mathbb{Z}">

Pokazaliśmy zatem, że <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H \in n\mathbb{Z}">, a więc <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=H = n\mathbb{Z}">. 

A więc innych podgrup liczb całkowitych niż wielokrotności <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n\mathbb{Z}"> nie ma. 

## Przykłady podgrup c.d.

* Liczby zespolone z mnożeniem i jedynką:

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(\mathbb{C} \setminus \{0\}, \cdot, 1)">

Udowodnić, że następujące zbiory są podgrupami tej grupy

a) <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{C}_1 = \{z \in \mathbb{C} : |z| = 1 \}">

Liczby <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{C}_1"> to takie liczby zespolone, że ich odległość (moduł) jest równy 1, a więc wszystkie leżą na okręgu jednostkowym. 

A zatem 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1 \in \mathbb{C}_1">
* jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=z_1, z_2 \in \mathbb{C}_1">, to iloczyn <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=|z_1 z_2|"> też powiniem należeć do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{C}_1">: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=|z_1 z_2| = |z_1||z_2| = 1 \cdot 1 = 1 \rightarrow z_1 \cdot z_2 \in \mathbb{C}_1"> 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=z = a + ib">
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=|z| = \sqrt{a^2 + b^2}">

Liczbę odwrotną do zespolonej: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\frac{1}{a+ib}">

obliczymy przez sprzężenie - przemnożenie przez mianownik: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\frac{1}{a+ib} \cdot \frac{a-ib}{a-ib}=\frac{a-ib}{a^2-iab+iab+b^2}=\frac{a-ib}{a^2+b^2}=\frac{a}{a^2+b^2} - i\frac{b}{a^2+b^2}">

Jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=z \in \mathbb{C}_1">, to także <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a^2 + b^2 = 1">, a więc: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\frac{a}{a^2+b^2} - i\frac{b}{a^2+b^2}=a+i(-b)">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=z^{-1} = a+(-b)i">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=|z^{-1}| = \sqrt{a^2 + (-b)^2} = \sqrt{a^2 + b^2} = \sqrt{1} = 1">

Liczba odwrotna też należy do okręgu jednostkowego,
mamy więc podgrupę:

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=z \in \mathbb{C}_1 \rightarrow z^{-1} \in \mathbb{C}_1">

Dla <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n = 2, 3, 4, ... \mu_n = \{z \in \mathbb{C}: z^n = 1 \}"> -- zbiór wszystkich pierwiatków <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n">-tego stopnia z jedynki; 
takich pierwiastków jest <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n">. 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\sqrt[2]{1} = \{1, -1\}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\sqrt[4]{1} = \{1, i, -1, -i\} = <i>"> (generowana przez <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=i">)

A więc 

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1 \in \mu_4">, bo <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1^n = 1">

* jeśli 2 liczby <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=z_1">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=z_2 \in \mu_4">, to <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(z_1 \cdot z_2)^n = z_1 z_2 z_1 z_2... = 
z_1^n \cdot z_2^n">, a już wiemy, że <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=z_1^n = 1, z_2^n = 1">, więc <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1 \cdot 1 = 1">

* skoro <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=z \in \mu_n \rightarrow (z^-{1)}^n">, to czy element odwrotny też należy? 

Wiemy, że 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=z \cdot z \cdot ...\cdot z \cdot z = 1 /\cdot z^{-1}">

Jedno <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=z"> się skróci, zostanie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=z \cdot z \cdot... \cdot z \cdot z = 1 \cdot z^{-1}">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=z \cdot z \cdot ... \cdot z \cdot z = z^{-1} \rightarrow (z^1)^n = 1">

Co jest analogiczne do generowania przez 1.

---

Jeszcze większą grupą od dotychczasowych jest
 
<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\mu_2 \cup \mu_3 \cup \mu_4">

-- dodajemy wszystkie zbiory. 

A zatem 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\mu_\infty = \mu_2 \cup \mu_3 \cup \mu_4..."> 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\bigcup_n=2^\infty \mu_n">

Z mnożeniem, jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=z_1^n = 1">, to <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=z_2^m = 1">

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(z_1 z_2)^nm = z_1^nm \cdot z_2^nm = (z_1^n)^m \cdot (z_2^m)^n
= 1^m \cdot 1^n = 1">

# Wyklad 6 | 12.12.2020

## 1. kolokwium -- 19.12.2020, 8.00-9.30

Zrobić zdjęcie pracy i wysłać na maila

Nie ma zajęć o 13

## Przykłady grup c.d.

Rozważmy grupę -- trójkąt równoboczny o wierzchołkach 1, 2, 3

Grupa izometrii będzie przekształcała ten trójkąt w inne trójkąty: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=GI_\triangle = \{ 1_\triangle, 0_{120\degree}, 0_{250\degree}, s_1 \}">

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1_\triangle"> -- brak przekształcenia

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0_{120\degree}"> -- obrót o 120 stopni: uzyskamy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\{2, 3, 1\}">

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0_|240\degree}"> -- obrót o 240 stopni -- <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\{ 3, 1, 2\}">

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_1"> -- symetria osiowa względem osi przechodzącej przez wierzchołek <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1"> -- <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\{ 1, 3, 2\}">

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_2"> -- symetria osiowa względem osi przechodzącej przez wierzchołek <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2"> -- <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\{ 3, 2, 1\}">

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_3"> -- symetria osiowa względem osi przechodzącej przez wierzchołek <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=3"> -- <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\{ 2, 1, 3\}">

|0| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1_\triangle"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0_{120\degree}"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0_{240\degree}"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_1"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_2"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_3"> | 
|-|-|-|-|-|-|-|
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1_\triangle"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1_\triangle"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0_{120\degree}"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0_{240\degree}"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_1"> |  <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_2"> |  <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_3"> |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0_{120\degree}"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0_{120\degree}"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0_{240\degree}"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1_\triangle"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_3"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_1"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_2"> |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0_{240\degree}"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0_{240\degree}"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1_\triangle"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0_{120\degree}"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_2"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_3"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_1"> |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_1"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_1"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_3"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_2"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1_\triangle"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0_{120\degree}"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0_{240\degree}"> |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_2"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_2"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_1"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_3"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0_{240\degree}"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1_\triangle"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0_{120\degree}"> |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_3"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_3"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_2"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_1"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0_{120\degree}"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0_{240\degree}"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1_\triangle"> |

Identyczność <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1_\triangle"> jest elementem neutralnym -- nic nie zmienia.

Mamy grupę nieprzemienną (tabela nie jest symetryczna). 

Podgrupami będą grupy z identycznością i elementem odwrotnym. 

# Ćwiczenia 6 | 12.12.2020

## 1 kolokwium: 19.12.2020, godz. 8.00-9.30

Zeskanowane prace wysłać na: rgigon@ath.bielsko.pl

Nie będzie zajęć ćwiczeniowych o 13.00

Zadania

* definicja grupy + przykłady grup
* sprawdzanie własności działań -- czy przemienne, łączne, mają element neutralny, element odwrotny (inwers)
* znajdowanie permutacji odwrotnej do danej 
* uzupełnianie tabelki z wynikami, np. półgrupy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z_4, \cdot_4"> (mnożenie modulo 4)
* znajdowanie wszystkich podgrup jakiejś grupy, np. <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z_{12}, +_2"> (dodawanie modulo 2)
* rozkład permutacji na cykle 

## Permutacja odwrotna do danej

Mamy np. permutację

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a = \Bigl( \begin{matrix} 1&2&3&4&5&6&7&8 \\ 2&8&7&4&6&1&5&3 \end{matrix} \Bigr)">

Permutacja odwrotna:

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a = \Bigl( \begin{matrix} 1&2&3&4&5&6&7&8 \\ 6&1&8&4&7&5&3&2 \end{matrix} \Bigr)">

## Rozkład permutacji na cykle 

Tylko jedności się nie da rozłożyć -- w niej każdy element przechodzi sam w siebie. 

Np. w permutacji: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a = \Bigl( \begin{matrix} 1&2&3&4&5&6 \\ 3&2&4&5&1&6 \end{matrix} \Bigr)">

1 przechodzi w 3, 3 w 4, 4 w 5, 5 w 1

Zapis skrótowy cyklu: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(1, 3, 4, 5)">

---

Permutacja: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\alpha = \Bigl( \begin{matrix} 1&2&3&4&5&6&7&8&9&10 \\ 4&5&2&6&3&8&2&1&9&10 \end{matrix} \Bigr)">

-- posiada 2 cykle: 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(1, 4, 6, 8)"> (to skrótowy zapis z identycznościami w miejscu tych liczb, które nie mają znaczenia:
1 2 3 4 5 6 7 8 9 10
4 2 3 6 5 8 7 1 9 10 

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(2, 5, 3)">
 
Cykle są rozłączne jako zbiory.

---

Cykle 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\alpha = (1, 4, 6, 8) \circ (2, 5, 3)">

Zapis z identycznościami: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\Bigl( \begin{matrix} 1&2&3&4&5&6&7&8&9&10 \\ 4&2&3&6&5&8&7&1&9&10 \end{matrix} \Bigr) \\\circ \\\Bigl( \begin{matrix} 1&2&3&4&5&6&7&8&9&10 \\ 1&5&2&4&3&6&7&8&9&10 \end{matrix} \Bigr)">

Złożenie: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\Bigl( \begin{matrix} 1&2&3&4&5&6&7&8&9&10 \\ 4&5&2&6&3&8&7&1&9&10 \end{matrix} \Bigr)">

-- mamy zatem wyjściową permutację.

## Transpozycja cyklu

Cykl 2-wyrazowy, np. 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(1, 2)">

Jego transpozycja: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\Bigl( \begin{matrix} 1&2 \\ 2&1 \end{matrix} \Bigr)">

## Rozkładanie iloczynu transpozycji 

Przykład 1: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(1, 4, 6, 8) = (1, 4) \circ (1, 6) \circ (1, 8)"> 

---

Przykład 2:

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(2, 5, 3) = (2, 5) \circ (2, 3) ">

## Definicja homomorfizmu grup 

Definicja: 

Funkcją <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=f : A \rightarrow B"> (odwzorowującą <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A"> w <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=B">, gdzie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=B"> to grupy), nazywamy **homomorfizmem**, gdy dla dowolnych <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=y"> należących do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A"> zachodzi, że jeśli wymnożymy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x"> i <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=y"> i prześlemy do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=f">, to uzyskamy to samo co w wyniku mnożenia wyników przesłania osobno <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x"> do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=f"> i <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=y"> do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=f">: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\forall x, y \in A: f(xy) = f(x) \cdot f(y)">

Przykład homomorfizmu trywialnego

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=f(x) = 1 \in B">

czyli 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math= \forall x \in A, f(xy) = 1, f(x)f(y) = 1 \cdot 1">

----

Weźmy liczbę grup rzeczywistych dodatnich:

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(\mathbb{R}_+, \cdot, 1)">

i drugą grupę liczb rzeczywistych z dodawaniem:

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(\mathbb{R}_+, +, 0)">

Możemy mnożenie zastąpić dodawaniem.

---

Inny przykład: funkcja 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=f(x) = \ln{x}">

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=f(xy) = \ln{xy} = \ln{x} + \ln{y} = f(x) + f(y)">

a więc logarytmowanie jest izomorficzne.  

Np. dla <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x = 1000">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1000 \dot 10000">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\lg{1000} + \lg{10000} = 3 + 4 = 7">

Wracamy: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=10^7 = 1000000">













 
























> Written with [StackEdit](https://stackedit.io/).


