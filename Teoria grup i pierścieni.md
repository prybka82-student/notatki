# Wykład 1 | 10.10.2020

Wykład odwołany.

# Wykład 2 | 24.10.2020

## Kolokwia

1. 6. zjazd
2. 10. zjazd

## Adres: rgigon@ath.bielsko.pl

## Oznaczenia zbiorów

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{N}"> -- liczby naturalne: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{N} = \{0, 1, 2... \}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Z_+}"> -- liczby całkowite dodatnie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Z} = \{1, 2, 3...\}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Z}"> -- liczby całkowite: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Z} = \{...-2, -1, 0, 1, 2...\}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Q}"> -- liczby (ułamki) wymierne: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Q} = \{ \frac{a}{b}: a \in \mathbb{Z}, b \in \mathbb{Z_+}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{IQ}"> -- niewymierne, np. <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\sqrt{2}"> 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{R}"> -- rzeczywiste: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{R} = \mathbb{Q} \cup \mathbb{IQ}"> 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{C}"> -- zespolone: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{C} = \{ a + ib; a, b \in \mathbb{R}; i^2 = -1 \}">

## Działania arytmetyczne na zbiorach 

| Zbiór |  <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=+"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\cdot"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=:"> |
|-|-|-|-|-|
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{N}"> | tak^[a] | nie | tak | nie | 
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Z_+}"> | tak | nie | tak | nie |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Z}"> | tak | tak | tak | nie |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Q}"> | tak | tak | tak | nie |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Q} \setminus \{0\}"> | nie | nie | tak | tak |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{IQ}"> | nie | nie | nie | nie |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{R}"> | tak | tak | tak | nie |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{C}"> | tak | tak | tak | nie |

[a]: Dla każdych 2 liczb można znaleźć sumę (różnicę, iloczyn, iloraz) z tego samego zbioru. 

## Liczby zespolone

* dodawanie i odejmowanie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\\(a+ib) + (c + id) := (a+c) + i(b+d)">
* mnożenie i dzielenie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\\(a+ib) \cdot (c+id) \\= ac + iad + ibc + i^2 bd \\= ac + i(ad + bc) - bd">

Przykład: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(2+3i)(-3-2i) \\= -6 - 6i^2 - 13i \\= -6 - 6(-1) - 13i \\=-6 + 6 - 13i \\= -13i">

## Definicja formalna działania dwuargumentowego

Niech <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A"> będzie niepustym zbiorem. Działaniem <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet"> (czyt. kropka) określonym na zbiorze <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A"> nazywamy (każdą) funkcję <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet"> (kropka) taką, że każdej parze elementów ze zbioru <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A">, czyli: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=A \times A = \{ (a,b) : a, b \in A \}">

(czyt. _A krzyż A_) tj. zbiorowi uporządkowanych par (iloczynowi kartezjańskiemu) -- funkcja <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet"> przyporządkowuje inny element również ze zbioru <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A">: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=A \times A \rightarrow A">

## Przykłady działań dwuargumentowych

* mnożenie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\cdot(a, b) := a \cdot b">, skrótowo:  <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=ab">

---

* działanie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\cdot"> w zbiorze <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A = \{1, 2\}"> zdefiniowane tabelką: 

| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet_1"> | 1 | 2 | 
|-|-|-|
| **1** | 1 | 1 | 
| **2** | 1 | 1 |

---

* działanie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet"> w zbiorze <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A = \{1, 2\}"> zdefiniowane tabelką: 

| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet_2"> | 1 | 2 |
|-|-|-|
| **1** | 2 | 2 |
| **2** | 2 | 2 |

# Ćwiczenia 2 | 24.10.2020

## Liczba możliwych działań dwuargumentowych

Dla zbioru <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A = \{a, b\}"> i działania <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet"> zdefiniowanego tabelką

| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet_A"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b"> |
|-|-|-|
| **<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a">** | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> lub <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> lub <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b"> |
| **<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b">** | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> lub <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> lub <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b"> |

-- liczba możliwych działań: 2 możliwe wartości w każdej kratce w 4 różnych kombinacjach, a więc <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2^4=2^{2^2}">

Dla zbioru <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=B = \{a, b, c\}"> i działania <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet"> zdefiniowanego tabelką

| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet_B"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c"> |
|-|-|-|-|
| **<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a">** | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a, b, c"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a, b, c"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a,b, c"> |
| **<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b">** | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a, b, c"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a, b, c"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a,b, c"> |
| **<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c">** | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a, b, c"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a, b, c"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a,b, c"> |

-- liczba możliwych działań: 3 możliwe wartości w każdej kratce w 9 różnych kombinacjach, a więc <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=3^9=3^{3^2}"> możliwych działań.

* działania w zbiorze 4-elementowym: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=4^{16} = 4^{4^2}"> możliwych działań 2-argumentowych; 

* działania w zbiorze 5-elementowym: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5^25=5^{5^2} = 25"> możliwych działań 2-argumentowych. 

Ogólnie w zbiorze <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n">-elementowym możliwe jest 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=n^{n^2}"> 

działań <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2">-elementowych. 

## Wzajemna odpowiedniość działań w zbiorach 

Przykład działań i zbiorów wzajemnie sobie odpowiadających: 

* zbiór <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A = \{1, 2, 3\}">
* działania: 

| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet"> | 1 | 2 | 3 |
|-|-|-|-|
| **1** | 2 | 1 | 1 |
| **2** | 3 | 3 | 2 |
| **3** | 2 | 1 | 1 |

* zbiór <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=B = \{a, b, c\}">
* działania: 

| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=*"> | a | b | c |
|-|-|-|-|
| **a** | b | a | a |
| **b** | c | c | b |
| **c** | b | a | a |

## Własności działań

Działanie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet"> w zbiorze <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A"> nazywamy: 

* __przemiennym__ jeśli dla każdej pary _a_, _b_ należących do zbioru _A_ zachodzi równość: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a\bullet b = b\bullet a">

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\forall_{a,b \in A} a \bullet b = b \bullet a">

* __łącznym__ jeśli dla każdej trójki _a_, _b_, _c_ należących do _A_ zachodzi równość: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(a \bullet b) \bullet c = a \bullet (b \bullet c)">

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\forall_{a, b, c \in A} (a \bullet b) \bullet c = a \bullet (b \bullet c)">

Przykłady działań niełącznych: 
* odejmowanie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(2 - 2) - 3 \neq 2 - (2 - 3)">. 
* dzielenie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(2 : 2) : 3 \neq 2 : (2 : 3)">. 

## Grupoid -- zbiór <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A"> z działaniem <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet">

Definicja: grupoid to zbiór <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A"> z określonym działaniem dwuargumentowym <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet">. 

Zapis: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(A, \bullet)">

Grupoid <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A"> jest **przemienny**, jeśli działanie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet"> w zbiorze <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A"> jest **przemienne**. 

## Półgrupa 

Definicja: grupoid <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(A, \bullet)"> to **półgrupa**, jeśli działanie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet"> w zbiorze <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A"> jest **łączne**. 

## Element neutralny w zbiorze <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A">

Definicja: element <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1"> należący do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A"> jest neutralny, jeśli dla każdego elementu tego zbioru zachodzi równość <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a\bullet 1 = 1 \bullet a = a"> (wykonanie działania na dowolnym elemencie zbioru i elemencie neutralnym nie zmienia wartośći): 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\forall_{a \in A} a \bullet 1 = 1 \bullet a = a">

Przykłady

| Zbiór i działanie | El. neutr. | Sprawdzenie |
|-|-|-|
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(\mathbb{R},+)"> <br/>-- liczby rzeczywiste i dodawanie | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\forall_{a \in \mathbb{R}} a+0 = 0+a = a"> |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(\mathbb{R},\cdot)"> <br/>-- liczby rzeczywiste i mnożenie | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\forall_{a \in \mathbb{R}} a\cdot 1 = 1\cdot 1 = a"> |

## Monoid

Definicja: monoid to półgrupa z elementem neutralnym. 

## Element odwrotny (inwers)

Definicja: niech będzie grupoid <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A"> (dokładnie: zbiór z działaniem: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(A, \bullet)">) z elementem neutralnym <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1">, to element <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b \in A"> nazywamy **odwrotnym**, jeśli dla każdego <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \in A"> zachodzi: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \bullet b = b \bullet a = 1">: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\forall_{a \in A} a\bullet b = b \bullet a = 1">

Przykłady dla grupoidu <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(\mathbb{R}, \cdot)">

| liczba | inwers | 
|-|-|
|<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a=2"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b=\frac{1}{2}"> |
|<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a=-3"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b=-\frac{1}{3}"> |

Przykłady dla grupoidu <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(\mathbb{R}, +)">

| liczba | inwers | 
|-|-|
|<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a=2"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b=-2"> |
|<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a=-3"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b=3"> | 

Dla dodawania inwersy są liczbami przeciwnymi. 

Na ogół element odwrotny (jeśli istnieje) do danego elementu nie jest wyznaczony jednoznacznie. 

Przykład działania <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet"> w zbiorze <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\{1, a, b\}"> (gdzie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1"> jest elementem neutralnym) z inwersem niewyznaczonym jednoznacznie: 

| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet"> | 1| a | b |
|-|-|-|-|
| **1** | 1| 1| 1|
| **a** | 1| 1| 1|
| **b** | 1| 1| 1|

Elementy odwrotne do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1 = \{1, a, b\}"> 
Elementy odwrotne do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a = \{1, a, b\}"> 
Elementy odwrotne do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b = \{1, a, b\}">   

Przykład działania <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet"> w zbiorze <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\{1, a, b\}"> (gdzie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1"> jest elementem neutralnym) bez inwersów: 

| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet"> | 1| a | b |
|-|-|-|-|
| **1** | a| 1| a|
| **a** | b| a| 1|
| **b** | 1| a| a|

Tutaj brak elementów odwrotnych. <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b"> nie jest elementem odwrotnym <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a">, bo o ile <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \bullet b = 1">, to <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b \bullet a \neq 1">. 



## Twierdzenie o elementach odwrotnych (inwersach)

Twierdzenie: w półgrupie (czyli grupie z działaniem łącznym) <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(A, \bullet)"> z elementem neutralnym <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1"> każdy element ma co najwyżej jeden element odwrotny lub nie ma go wcale. 

Dowód: niech 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a, b, c \in A"> 

oraz 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=1 = a \bullet b = b \bullet a = a \bullet c = c \bullet a"> 

(a więc <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b"> i <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c"> są odwrotne do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a">), wówczas można zapisać, że

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=b = b \bullet 1">

-- każdy element zbioru można zapisać jako działanie z elementem neutralnym, np. <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2"> można zapiać jako <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2 + 0"> lub <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2 \cdot 1">.

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=b \bullet 1 = b \bullet (a \bullet c)">

-- skoro <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \bullet c = 1">.

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=b \bullet (a \bullet c) = (b \bullet a) \bullet c"> 

-- z prawa łączności. 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(b \bullet a) \bullet c = 1 \bullet c"> 

-- skoro <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b \bullet a = 1">.

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=1 \bullet c = 1">

-- co było do udowodnienia?

# Wykład 3 (14.11.2020)

Od następnego zjazdu wykład od godz. 8.20

## Grupa

Wyznaczniki grupy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A">:

* działanie grupy jest **łączne**;
* działanie posiada **element neutralny** <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1">, taki że <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\forall_{a \in A} a \bullet 1 = a"> (element neutralny działania <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\bullet"> nie zmienia wartośći);
*
wykład od 8.20 do 9.-5

# Grupa (przypomnienie)

Grupa jeśli 3 warunki spełnione: 
- działanie jest łączne
- istnieje element neutralny działania
- każdy element <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> grupy ma **inwers** (element odwrotny) <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x"> spełniający warunek:

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\forall_{a \in A} \exists_{x \in A} ax = xa = 1">

-- tzn. wykonanie działania na dowolnym elemencie grupy i inwersie daje w rezultacie element neutralny. Inwers możnamożemy inwers oznaczać jako <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a^{-1}"> 

## Przykłady grup

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(\mathbb{C}, +, 0)"> --Największy zbiór: liczby zespolone z dodawaniem i zerem 

Sprawdzenie przemienności: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(CC, +, 0)">

-(a + ib) = -a + i(-b)"><img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(a+ib) + (-a + i(-b)) = 0">

* L
Inny przykład: liczby rzeczywiste <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{R}">R z dodawaniem i zerem.

* LInny przykład: liczby wymierne <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Q}">Q z dodawaniem i zerem.

* LiczbyPrzykład: całkowite <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Z}">Z z dodawaniem i zerem. 

* Liczby zespolone <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{C}">

Przykład: zespolone bez zera z, mnożeniem i, jednością: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(\mathbb{C} \setminus en 

(C\{0\}, \cdot, 1)">

* L*, 1)

Przykład: liczby rzeczywiste bez zera z, mnożeniem i, jednością: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(\mathbb{R} \setminus en

(R\{0\}, \cdot, 1)">

* Liczby*, 1)

Przykład: wymierne bez zera z, mnożeniem i jednością: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(\mathbb{Q} \setminus \{0\}, \cdot, 1)">

* Bijekcja <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=B(X)">, gdzie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=X"> to dowolny zbiór: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=B(X) - \{f : X \rightarrow X\}">

-- funkcja jest różnowartościowa (różnym wartościom przypisuje różne wartości z tego samego zbioru) i ma zbiór <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=X">. 

Bijekcja posiada również funkcję odwrotną. 

* Permutacja

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=f = \Bigl(\begin{matrix} 1 & 2 & 3 \\ 2 & 1 & 3 \end{matrix}\Bigr)">

Odwrotność: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=f^{-1} = \Bigl (\begin{matrix} 1 & 2 & 3 \\ 2 & 1 & 3 \end{matrix}\Bigr)">

* Funkcja <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=f(x) = x^3, x \in \mathbb{R}">  

Funkcja jest różnowartościowa w zbiorze <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{R}">: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=f: \mathbb{R} \rightarrow \mathbb{R}">

Funkcja odwrotna: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=f^{-1} = \sqrt[3]{x}">

* Składanie funkcji: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(B(X), \circ, 1_x)">

Element neutralny -- funkcja identycznościowa <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1_x"> taka, że <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1_x(x) = x">

Dowód: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\forall_x (f \circ 1_x)(x) = f(1_x(x)) = f(x)">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=f \circ 1_x =f">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1_x \circ f = f">

* Permutacja 

Jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=X"> jest zbiorem wieloelementowym: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=X = \{1, 2, 3, ...., n \}"> i zamiast <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=B(X)"> będziemy pisać <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=P_n"> (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=B(X) := P_n">), to zbiór wszystkich permutcji (bijekcji) zbioru <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n">-elementowego. 

Niech <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n = 5">. 

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

* Pełna grupa liniowa z mnożeniem

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=GL(2)"> -- takie macierze należące do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=M_2">, że wyznacznik jest niezerowy: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=GL(2) = \{ A \in M_2 : \det{A} \neq 0\}">

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z_5"> -- wszystkie reszty z dzielenia liczby całkowitej przez <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5">

Możliwe liczby: 0, 1, 2, 3, 4 (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z_5 = \{0, 1, 2, 3, 4\}">.

Przyjmujemy oznaczenie: jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \in Z">, to <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(a)_5"> może być resztą z dzielenia <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> przez <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5">, np. 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(10)_5 = 0">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(13)_5 = 3">

Przyjmijmy działanie dodawanie modulo 5 <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=+_5">, np. 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2 +_5 1 = (2+1)_5 = 3_5 = 3">, bo <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=3 = 0 \cdot 5 + 3">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2 +_5 2 = 4">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=3 +_5 2 = (3+2)_5 = 0">

# Ćwiczenia 3 (14.11.2020)

## Przykłady grup c.d. 

* Dodawanie modulo 5 w zbiorze <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\{0,1,2,3,4\}">

Zbiór: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z_5 = \{0,1,2,3,4\}">

Działanie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a +_5 b = (a+b)_5">

Sposób obliczania: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a +_5 b = \begin{cases} a+b, & a+b<5 \\ a+b-5, & a+b >=5 \end{cases}">

Wyniki: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=+_5"> | 0 | 1 | 2 | 3 | 4
-|-|-|-|-|-
**0** |0|1|2|3|4
**1** |1|2|3|4|0
**2** |2|3|4|0|1
**3** |3|4|0|1|2
**4** |4|0|1|2|3

Elementy odwrotne (takie, które po zsumowaniu dadzą 5):

* dla 0 -- 0 (bo 5 nie należy do zbioru), 
* dla 1 -- 4 (zapis: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-_5 1 = 4">) 
* dla 2 -- 3, 
* dla 3 -- 2, 
* dla 4 -- 1

* Ogólnie dla zbioru <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z_n = \{0, 1, 2, ..., n-2, n-1\}, (n>1)"> (zbiorami typu <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z_1 = \{0\}"> nie będziemy się zajmować)

Działanie dodawanie modulo <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n">:: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a +_n b= (a_b)_n = \begin{cases} a+b, & a+b < n \\ a+b-n, & a+b >=n \end{cases} ">

Element neutralny działania <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=+_n">: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0">

Element przeciwny <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-_n">: 
 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-_n 0 = 0">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-_n k =  n-k, k > 0">

## Zadania 

1. Sprawdzić, czy dane działanie jest przemienne, łączne i czy posiada element neutralny, a jeśli tak, to znaleźć elementy odwrotne.  

* Zbiór: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{R}">
* Działanie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ b = a+b+3, a \in \mathbb{R}">

Wynik <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \circ b"> należy do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{R}<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=. ">1\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Działanie jest przemienne, bo dodawanie jest przemienne:">b \circ a = b + a + 3<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=Korzystamy z przemienności dodawania: ">b + a + 3 = a + b + 3 = a \circ b<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math= (q.e.d)">2\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Sprawdzenie łączności:">(a \circ b) \circ c = (a + b + 3) \circ c = a + b + c + 6<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math= 

Korzystamy z przemienności:">a \circ (b \circ c) = a \circ (b + c + 3) = a + b + c + 6 = (a \circ b) \circ c<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(q.e.d.)">3\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Sprawdzenie elementu neutralnego">a \circ x = a \Leftrightarrow x = -3<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=">x \circ b = b \Leftrightarrow x = -3##

Element neutralny: ">-3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">4\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Elementy przeciwne:

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a \circ x = -3">
<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a + x + 3 = -3 /-3">
<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a + x = -6 - a">
<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=x = -6 - a">

Ogólny wzór na element przeciwny do ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=: ">x = -6 - a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Sprawdzenie: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a \circ -6 -a = a + -6 -a +3 = -3">

A ">-3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= to element neutralny. 

Mamy więc do czynienia z grupą przemienną (tzw. abelową). 

---

2. Sprawdzić, czy dane działanie jest przemienne, łączne i czy posiada element neutralny, a jeśli tak, to znaleźć elementy odwrotne.  

Działanie: ">a \circ b = a + b + ab<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">1\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Działanie jest przemienne, bo dodawanie i mnożenie jest przemienne. 

Sprawdzenie">L = a \circ b = a + b + ab<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">P = b \circ a = b + a + ba<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Pytanie, czy ">L = P<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">P = b \circ a = b + a + ba = a + b + ab = a \circ b = L<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(q.e.d.)">2\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Sprawdzenie, czy działanie jest łączne: ">L = (a \circ b) \circ c<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">P = a \circ (b \circ c)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Pytanie, czy ">L = P<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">P = a \circ (b \circ c) \\= a \circ (b + c + bc)\\ = a + (b + c + bc) + a(b+c+bc)\\ = a + b + c + bc + ab + ac + abc\\ = a + b + c + ab + bc + ac + abc<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">L = (a \circ b) \circ c\\ = (a + b +ab) \circ c\\ = (a+b+ab) + c + c(a+b+ab) \\= a + b + ab + c + ca +cb + cab \\= a + b + c + ab + bc + ac + abc = P<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(q.e.d.)">3\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Element neutralny ">x<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=: 

Z definicji ">a \circ x<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= powinno się równać ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, a więc:">a \circ x = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a + x + ax = a / -a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">x + ax = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">x(1+a) = 0 / \frac{1}{1+a}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">x = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Element neutralny: ">0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Sprawdzenie: ">a \circ 0 = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a + 0 + 0\cdot a = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">4\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Element odwrotny ">x<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z definicji elementu odwrotnego, ">a \circ x<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= powinno dać element neutralny, czyli ">0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, a więc: ">a \circ x = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a + x +ax = 0 / -a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">x + ax = -a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">x(1+a) = -a / \frac{1}{1+a}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">x = \frac{-a}{1+a}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Element odwrotny do ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= to ">\frac{-a}{1+a}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Sprawdzenie: ">a \circ \frac{-a}{1+a} = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a + \frac{-a}{1+a} + a\cdot \frac{-a}{1+a} = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\frac{a(1+a) - a - a^2}{1+a} = 0 / \frac{1}{1+a}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a+a^2-a-a^2 = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a - a + a^2 - a^2 = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">0 = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(q.e.d.)

# Wykład 4 | 28.11.2020

## Zadania c.d.

3. Sprawdzić, czy dane działanie jest przemienne, łączne i czy posiada element neutralny, a jeśli tak, to znaleźć elementy odwrotne.  

Zbiór: ">\mathbb{R_+}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- liczby rzeczywiste większe do zera. 

Działanie: ">\circ<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= zdefiniowane jako: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a \circ b = (\sqrt[3]{a} + \sqrt[3]{b})^3">">1\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Sprawdzenie przemienności -- działanie jest przemienne, bo dodawanie jest przemienne. ">2\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Sprawdzenie łączności: ">L = (a \circ b) \circ c = (\sqrt[3]{a} + \sqrt[3]{b})^3 \circ c\\=(\sqrt[3]{(\sqrt[3]{a} + \sqrt[3]{b})^3} + \sqrt[3]{c})^3\\=(\sqrt[3]{a} + \sqrt[3]{b} + \sqrt[3]{c})^3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">P = a \circ (b \circ c) = a \circ (\sqrt[3]{b} + \sqrt[3]{c})^3\\=(\sqrt[3]{a} + \sqrt[3]{(\sqrt[3]{b} + \sqrt[3]{c})^3})^3\\=(\sqrt[3]{a}+\sqrt[3]{b}+\sqrt[3]{c})^3 = L<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(q.e.d.)

A więc działanie jest łączne. ">3\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Element neutralny ">x<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z definicji: ">a \circ x = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">(\sqrt[3]{a} + \sqrt[3]{x})^3 = a /\sqrt[3]{}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\sqrt[3]{a} + \sqrt[3]{x} = \sqrt[3]{a}  / -\sqrt[3]{a}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\sqrt[3]{x} = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">x = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Element neutralny: ">0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">4\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Element odwrotny do ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z definicji ">a \circ a^{-1} = e<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, gdzie ">e<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest elementem neutralnym. A więc: ">a \circ a^{-1} = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">(\sqrt[3]{a} + \sqrt[3]{a^{-1}})^3 = 0 / \sqrt[3]{}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\sqrt[3]{a} + \sqrt[3]{a^{-1}} = 0 / -\sqrt[3]{a}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= ">\sqrt[3]{a^{-1}} = -\sqrt[3]{a} /^3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a^{-1} = -a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A więc element odwrotny do ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= to ">-a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=. 

Sprawdzenie: ">a \circ -a = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">(\sqrt[3]{a} + \sqrt[3]{-a})^3 = 0 / \sqrt[3]{}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\sqrt[3]{a} - \sqrt[3]{a} = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">0 = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(q.e.d.)

---

4. Sprawdzić, czy dane działanie jest przemienne, łączne i czy posiada element neutralny, a jeśli tak, to znaleźć elementy odwrotne.  

Zbiór: ">\mathbb{R^+}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (dodatnie liczby rzeczywiste.

Działanie: ">a \diamond b = 5^{\log_5{a} \cdot \log_5{b}}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">1\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Sprawdzenie przemienności.

Z własności logarytmów możemy zapisać: ">=5^{ \log_5{b} \cdot \log_5{a} } = b \diamond a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 

A zatem działanie jest przemienne.">2\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Sprawdzenie łączności. ">L = (a \diamond b) \diamond c = (5^{\log_5{a} \cdot \log_5{b}}) \diamond c= 5^{\log_5{5^{\log_5{a} \cdot \log_5{b}}} \cdot \log_5{c}}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Korzystając z własności logarytmu: ">\log_n{x^\alpha} = \alpha \cdot \log_n{x}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=: ">L = 5^{{\log_5{a} \cdot \log_5{b} } \cdot \log_5{5} \cdot \log_5{c}}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 

Usuwamy ">\log_5{5} = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">L = 5^{\log_5{a} \cdot \log_5{b} \cdot \log_5{c}}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">P = a \diamond (b \diamond c) = a \diamond (5^{\log_5{b} \cdot \log_5{c}}) = 5^{\log_5{a} \cdot \log_5{5^{\log_5{b} \cdot \log_5{c}}}}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">P = 5^{\log_5{a} \cdot \log_5{5} \cdot \log_5{b} \cdot \log_5{c}}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Usuwamy ">\log_5{5} = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">P = 5^{\log_5{a} \cdot \log_5{b} \cdot \log_5{c}} = L<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(q.e.d.)

A więc działanie jest łączne. ">3\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Element neutralny ">a \diamond e = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">5^{\log_5{a} \cdot \log_5{e}} = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (logarytmujemy obustronnie)">\log_5{5^{\log_5{a} \cdot \log_5{e}}} = \log_5{a}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\log_5{a} \cdot \log_5{e} \cdot \log_5{5} = \log_5{a}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\log_5{a} \cdot \log_5{e} = \log_5{a} / \frac{1}{\log_5{a}}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">log_5{e} = 1 \Leftrightarrow 5^1=e<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">e = 5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Sprawdzenie: ">a \diamond 5 = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">5^{\log_5{a} \cdot \log_5{5}} = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">5^{(\log_5{a}) \cdot 1} = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z własności logarytmu: ">a^{\log_a{b}} = b<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(q.e.d.)">4\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Element odwrotny do ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z definicji elementu odwrotnego: ">a \diamond a^{-1} = e<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, gdzie ">e<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest elementem neutralnym. A więc: ">a \diamond a^{-1} = 5 = 5^1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">5^{\log_5{a} \cdot \log_5{a^{-1}}} = 5 = 5^1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\log_5{a} \cdot \log_5{a^{-1}} = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\log_5{a} \neq 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, a zatem ">a \neq 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\log_5{a} = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= oraz ">\log_5{a^{-1}} = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a = 5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= oraz ">a^{-1} = 5 = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a = a^{-1}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Działanie nie ma zatem elementu odwrotnego, a więc ">(\mathbb{R^+}, \diamond, 5)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= nie jest grupą. 

# Ćwiczenia 4 | 28.11.2020 

## Podgrupa 

Definicja: niepusty podzbiór ">H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= grupy ">G<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= nazywamy **podgrupą** grupy ">G<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, jeśli sam jest grupą, a więc musi spełniac warunki: 

* ">1 \in H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- musi mieć element neutralny,
* działanie w tym zbiorze musi być przemienne; 

a dodatkowo dla każdego elementu ">H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= musi istnieć jego inwers (element przeciwny): 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\forall_{a \in H} a^{-1} \in H">

## Przykłady podgrup

* ">G=Z_4<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= z dodawaniem modulo 4 ">(+_4)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=---

* ">(Q\{0\}, \circ, 1)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=---

* Liczby całkowite z mnożeniem nie są podgrupą, bo ">\frac{1}{\mathbb{Z}}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= nie należy od zbioru liczb całkowitych.

---

* Bijekcja ">B(X)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (">X<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= to dowolny zbiór), zdefiniowana jako funkcja przepisująca elementy zbioru w ten sam zbiór:  

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=B(X) \{f : X \rightarrow X: f\}">

Bijekcja ">B<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest różnowartościowa i ma zbiór ">X<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=. 

Przykład: 

zbiór ">X<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= ---  zbiór ">X<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 
1 ">\rightarrow<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 2
2 ">\rightarrow<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 1
3 ">\rightarrow<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 3

-- różnym wartościom przypisane są różne wartości; wszystkie elementy zbioru ">X<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= są wykorzystane. 

Funkcję ">f<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= można pokazać jako permutację: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=f = \Bigl( \begin{matrix} 1 & 2 & 3 \\ 2 & 1 & 3 \end{matrix} \Bigr)">

Odwrotność (funkcja odwrotna): 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=f^{-1} = \Bigl( \begin{matrix} 1 & 2 & 3 \\ 2 & 1 & 3 \end{matrix} \Bigr)">

---
 
* Funkcja ">f(x) = x^3, x \in \mathbb{R}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Funkcja jest różnowartościowa w zbiorze ">\mathbb{R}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=f: \mathbb{R} \rightarrow \mathbb{R}">

Wykres

<iframe src="https://www.desmos.com/calculator/3sdsbko0ew?embed" width="500px" height="500px" style="border: 1px solid #ccc" frameborder=0></iframe>

Funkcja odwrotna: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=f^{-1} = \sqrt[3]{x}">

---

* Składanie funkcji <img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(B(X), \circ, 1_x)">

Symbol działania: ">\circ<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Element neutralny -- funkcja identycznościowa ">1_x<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, gdzie ">1_x(x) = x<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Sprawdzenie: ">(f \circ 1_x)(x) = f( 1_x(x) ) = f(x)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=  dla każdego ">x<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">f \circ 1_x =f<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">1_x \circ f = f<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=---

* Permutacja (bijekcja)">X<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest zbiorem wieloelementowym (">X = \{1, 2, 3, ...., n \}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=)

Zamiast ">B(x)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= możemy pisać ">P_n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=: ">B(X) := P_n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Niech ">n = 5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Element neturalny ">1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=:

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

Sprawdzenie:">\Bigl[ \begin{matrix} 1 & 0 \\ 0 & 1 \end{matrix} \Bigr] \cdot \Bigl[ \begin{matrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{matrix} \Bigr] = \Bigl[ \begin{matrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{matrix} \Bigr]<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=---

* Pełna grupa liniowa z mnożeniem">GL(2)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- takie macierze należące do ">M_2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, że ich wyznacznik jest niezerowy: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=GL(2) = \{ A \in M_2 : \det{A} \neq 0 \}">

---

* ">Z_5, +_5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- wszystkie reszty z dzielenia liczby całkowitej przez ">5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Możliwe liczby: 0, 1, 2, 3, 4

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=Z_5 = \{0, 1, 2, 3, 4\}">

Przyjmujemy oznaczenie: jeśli ">a\in Z<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to ">(a)_5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= może być dowolną liczbą naturalną i resztą z dzielenia ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= przez ">5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, np. ">(10)_5 = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">(13)_5 = 3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Przyjmijmy działanie dodawanie modulo 5 ">+_5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= takie, że jeśli">a +_5 b = (a + b)_5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Przykłady">2 +_5 1 = (2+1)_5 = 3_5 = 3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (bo ">3 = 0 \cdot 5 + 3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=)">2 +_5 2 = 4<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">3 +_5 2 = (3+2)_5 = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=---

* Dodawanie modulo 5 (">+_5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=): ">a +_5 b = (a+b)_5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Zbiór: ">Z_5 = {0,1,2,3,4}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Sposób obliczania:">\begin{cases} a + b, & a + b < 5 \\ a + b - 5, &a + b \geq 5 \end{cases}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Działania">+_5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | 0 | 1 | 2 | 3 | 4
-|-|-|-|-|-
**0** |0|1|2|3|4
**1** |1|2|3|4|0
**2** |2|3|4|0|1
**3** |3|4|0|1|2
**4** |4|0|1|2|3

Elementy odwrotne: (takie, że suma da 5): ">-_5 0 = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (bo 5 nie należy do zbioru)">-_5 1 = 4<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">-_5 2 = 3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">-_5 3 = 2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">-_5 4 = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=----

* Ogólnie dodawanie modulo ">n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= w zbiorze ">Z_n = \{0, 1, 2, ..., n-2, n-1\}, (n>1)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Zbiorem ">Z_1 = {0}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= nie będziemy się zajmować

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a +_n b = (a+b)_n = \begin{cases} a + b, & a + b < n \\ a + b - n,& a+b \geq n \end{cases}">

Element neutralny działania ">+_n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=: ">0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Element przeciwny: ">-_n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= ">-_n 0 = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">-_n k =  n-k   , k > 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=----

## Zadania

1. Sprawdzić, czy dane działanie jest przemienne, łączne i czy posiada element neutralny, a jeśli tak, to znaleźć elementy odwrotne. 

Zbiór: ">\mathbb{R}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Działanie: ">a \circ b = a+b+3, a \in \mathbb{R}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, wynik ">a \circ b<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= należy do ">\mathbb{R}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">1\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Działanie jest przemienne, bo dodawanie jest przemienne:">b \circ a = b + a + 3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Korzystam z przemienności dodawania:">b + a + 3 = a + b + 3 = a \circ b<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(q.e.d)">2\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Sprawdzenie łączności:">(a \circ b) \circ c = (a + b + 3) \circ c = a + b + c + 6<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Korzystam z przemienności">a \circ (b \circ c) = a \circ (b + c + 3) = a + b + c + 6 = (a \circ b) \circ c<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 

(q.e.d.)">3\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Sprawdzenie elementu neutralnego:

Z definicji ">a \circ x = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a + x + 3 = a / -a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">x + 3 = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">x = -3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Element neutralny: ">-3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">4\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Elementy przeciwne:

Z definicji ">a \circ a^{-1} = e<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, gdzie ">e<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= to element neutralny.">a \circ a^{-1} = -3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a + a^{-1} + 3 = -3 / -3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a + a^{-1} = -6 /-a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a^{-1} = -6 - a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (ogólny wzór na element przeciwny) 

Sprawdzenie: ">a \circ -6 -a = a + -6 -a +3 = -3 = e<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Mamy zatem do czynienia z grupą przemienną (abelową).

## Zadanie domowe

Sprawdzić, czy dane działanie jest przemienne, łączne i czy posiada element neutralny, a jeśli tak, to znaleźć elementy odwrotne. 

Działanie: ">a \circ b = a + b + ab<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">1\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Sprawdzenie przemienności ">L = a \circ b = a + b + ab<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">P = b \circ a = b + a + ba<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Korzystam z przemienności dodawania i mnożenia: ">L = b + a + ba = P<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(q.e.d.)">2\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Sprawdzenie łączności">(a \circ b) \circ c \\= (a + b + ab) \circ c \\= (a + b + ab) + c + c(a + b + ab) \\=a + b + c + ab + ac + bc + abc<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a \circ (b \circ c) \\=a \circ (b + c + cb) \\= a + (b + c +cb) + a(b + c + bc) \\=a + b + c + ab + ac + bc + abc\\=(a \circ b) \circ c<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(q.e.d)">3\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Element neutralny ">e<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z definicji ">a \circ e = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a + e + ae = a /-a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">e + ae = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">e(1 + a) = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">e = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Sprawdzenie: ">a \circ 0 = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a + 0 + a\cdot 0 = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a + 0 = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(q.e.d.)">4\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Element odwrotny ">a^{-1}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 

Z definicji ">a \circ a^{-1} = e<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, gdzie ">e<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= to element neutralny.">a \circ a^{-1} = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a + a^{-1} + aa^{-1} = 0 / -a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a^{-1} + aa^{-1} = -a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a^{-1}(1 + a) = -a / \frac{1}{1+a}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a^{-1} = \frac{-a}{1+a}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Sprawdzenie">a \circ \frac{-a}{1+a} = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a + \frac{-a}{1+a} + a\frac{-a}{1+1} = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\frac{a(1+a) + ( -a) + ( -a^2)}{1+a} = 0/(1+a)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a+a^2-a-a^2 = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">0=0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(q.e.d.)

# ???Wykład 4 | 28.11.2020

## Zadania c.d.

1. Sprawdzić, czy dane działanie jest przemienne, łączne i czy posiada element neutralny, a jeśli tak, to znaleźć elementy odwrotne.

Zbiór: ">\mathbb{R}^+<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Działanie: ">\circ<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a \circ b = (\sqrt[3]{a} + \sqrt[3]{b})^3">">1\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Sprawdzenie przemienności -- działanie ">\circ<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest przemienne, bo dodawanie jest przemienne. ">2\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Sprawdzenie łączności">(a \circ b) \circ c \\= (\sqrt[3]{a} + \sqrt[3]{b})^3 \circ c \\= (\sqrt[3]{(\sqrt[3]{a} + \sqrt[3]{b})^3} + \sqrt[3]{c})^3 \\= (\sqrt[3]{a} + \sqrt[3]{b} + \sqrt[3]{c})^3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a \circ (b \circ c) \\=a \circ (\sqrt[3]{b} + \sqrt[3]{c})^3 \\=(\sqrt[3]{a} + \sqrt[3]{(\sqrt[3]{b} + \sqrt[3]{c})^3})^3 \\=(\sqrt[3]{a} + \sqrt[3]{b} + \sqrt[3]{c})^3 \\=(a \circ b) \circ c<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A więc działanie jest łączne.">3\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Element neutralny ">e<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z definicji ">a \circ e = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">(\sqrt[3]{a} + \sqrt[3]{e})^3 = a /\sqrt[3]{}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\sqrt[3]{a} + \sqrt[3]{e} = \sqrt[3]{a} /-\sqrt[3]{a}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\sqrt[3]{e} = 0 /^3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">e = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Element neutralny: ">0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Sprawdzenie: ">a \circ 0 = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">(\sqrt[3]{a} + \sqrt[3]{0})^3 = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">(\sqrt[3]{a} + 0)^3 = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">(\sqrt[3]{a})^3 = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(q.e.d.)

Mając element neutralny, możemy mówić o elemencie odwrotnym.">4\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Element odwrotny ">a^{-1}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z definicji ">a \circ a^{-1} = e<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, gdzie ">e<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest elementem neutralnym. ">a \circ a^{-1} = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">(\sqrt[3]{a} + \sqrt[3]{a^{-1}})^3 = 0 /\sqrt[3]{}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\sqrt[3]{a} + \sqrt[3]{a^{-1}}=0 /-\sqrt[3]{a}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\sqrt[3]{a^{-1}} = -\sqrt[3]{a} /^3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a^{-1} = -a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (ogólny wzór na element odwrotny)

Sprawdzenie: ">a \circ -a = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">(\sqrt[3]{a} + \sqrt[3]{-a})^3 = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">(\sqrt[3]{a} - \sqrt[3]{a})^3 = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">(0)^3 = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(q.e.d.)

-------

2. Sprawdzić, czy dane działanie jest przemienne, łączne i czy posiada element neutralny, a jeśli tak, to znaleźć elementy odwrotne.

Zbiór: ">\mathbb{R}^+<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Działanie: ">\circ<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a \circ b = 5^{log_5{a} \cdot log_5{b}}">">1\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Sprawdzenie przemienności 

Mnożenie jest przemienne, a więc: ">a \circ b\\=5^{\log_5{a} \cdot \log_5{b}} \\=5^{\log_5{b} \cdot \log_5{a}} \\=b \circ a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=jest przemienne.">2\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Sprawdzenie łączności ">(a \circ b) \circ c \\= (5^{\log_5{a} \cdot \log_5{b}}) \circ c \\= 5^{\log_5(5^\log_5{a} \cdot \log_5{b}) \cdot \log_5{c}}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z własności logarytmu wiemy, że: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\log_5{x^\alpha} = \alpha \cdot \log_5{x}">

Z zatem">5^{\log_5{a} \cdot \log_5{b} \cdot \log_5{5} \cdot \log_5{c}} \\= 5^{log_5{a} \cdot \log_5{b} \cdot \log_5{c}}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">3\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Element neutralny ">e<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z definicji elementu neutralnego: ">a \circ e = a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">5^{\log_5{a} \cdot log_5{e}} = a /\log_5{}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\log_5{5^{\log_5{a} \cdot \log_5{e}}} = \log_5{a}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z definicji logarytmu ">\log_a{x} = y \leftrightarrow a^y=x<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">5^{\log_5{a}} = 5^{\log_5{a} \cdot \log_5{e}}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A więc: ">\log_5{a} = \log_5{a} \cdot \log_5{e} /\frac{1}{\log_5{a}}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\log_5{e} = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">5^1 = e = 5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Sprawdzenie: ">5^{\log_5{a} \cdot \log_5{5}} = a/\log_5{}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\log_5{5^{\log_5{a} \cdot \log_5{5}}} = \log_5{a}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">5^{\log_5{a}} = 5^{\log_5{a} \cdot \log_5{5}}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\log_5{a} = \log_5{a} \cdot \log_5{5} /\frac{1}{\log_5{a}}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">1 = \log_5{5}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">5^1 = 5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(q.e.d)">4\degree<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= Element przeciwny ">a^{-1}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z definicji ">a \circ a^{-1} = e<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, gdzie ">e<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= to element neutralny. ">5^{\log_5{a} \cdot \log_5{a^{-1}}} = 5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z własności potęgowania ">(a^x)^y = a^{x\cdot y}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">(5^{\log_5{a}})^{\log_5{a^{-1}}} = 5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z własności logarytmów: ">a^{\log_a{b}} = b<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a^{\log_5{a^{-1}}} = 5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z własności logarytmów: ">a^{\log_c{b}} = b^{\log_c{a}}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">(a^{-1})^{\log_5{a}} = 5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">a^{-1} = 5^{\frac{1}{\log_5{a}}}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Sprawdzenie: ">5^{\log_5{a} \cdot \log_5{5^{\frac{1}{\log_5{a}}}}} = 5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">5^{\log_5{a} \cdot \log_5{5^{\frac{1}{\log_5{a}}}}} = 5^1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\log_5{a} \cdot \log_5{5^{\frac{1}{\log_5{a}}}} = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z własności logarytmów: ">\log_a{x^y} = y\log_a{x}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\log_5{a} \cdot \frac{1}{\log_5{a} } \log_5{5} = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">1 \cdot 1 = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(q.e.d.)

-------------------

# ???Ćwiczenia 4 | 28.11.2020 

## Podgrupa 

Definicja: niepusty podzbiór ">H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= grupy ">G<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= nazywamy **podgrupą** grupy ">G<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, jeśli sam jest grupą.

## Przykłady podgrup

* ">G=Z_4<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= z dodawaniem modulo 4 ">(+_4)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Na ogół podzbiórami są elementy z 1 elementem i równe innej grupie. 

## Twierdzenie Lagrange'a

Niech ">H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= będzie podgrupą grupy skończonej ">G<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (tzn. ">G<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= ma skończoną liczbę elementów), wówczas liczba elementów (tzw. rząd) grupy ">H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= dzieli liczbę elementów grupy ">G<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=.

Np. jeśli grupa ">G<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= ma 12 elementów, to wówczas podgrupa ">H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= grupy ">G<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= ma 12, 1, 6, 2, 3, 4 elementów.

## Warstwy lewo- i prawostronne grup

Oznaczenia: 

* ">G<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= to grupa, 
* ">H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- podgrupa grupy ">G<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, 
* ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- element należący do ">G<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (">a \in G<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=), 
* ">aH<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- zbiór elementów ">a\cdot h<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= takich, że ">h<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= przebiega przez ">H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=:
 
<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=aH = \{ a \cdot h : h \in H\}">

Np. ">H = \{0,2\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=to ">0 +_4 H = \{0, 2\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">1 +_4 H = \{1, 3\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">2 +_4 H = \{2, 0\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= ">3 +_4 H = \{3, 1\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 

Taki zbiór nazywamy **warstwą lewostronną** (bo ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest po lewej) grupy ">G<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= wyznaczoną przez element ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= i podgrupę ">H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=. 

A taki zbiór:

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=Ha= \{h \cdot a : h \in H\}">

-- nazywamy **warstwą prawostronną** grupy ">G<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= wyznaczoną przez element ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= i podgrupę ">H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Dla ">a = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to ">a \cdot H = 1 \cdot H = H \cdot 1 = H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 

Warstwy mają tyle samo elementów co grupa

## Przykłady

* Niech będzie grupa ">G<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, ">H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Weźmy funkcję 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=L_a: H \rightarrow aH">

gdzie ">L_a (h) = a \cdot h, h \in H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 

Zauważamy, że ">L_a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest różnowartościowa, bo jeśli ">L_a(h) = L_a(h')<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to wówczas ">ah = ah' |a^-1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, a zatem ">a{^-1} a h = a^{-1} a h'<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, czyli ">h = h'<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=. A więc ">L_4<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest na zbiór ">aH<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=. 

Mamy tu bijekcję, tzn. wzajemne dopasowanie elementów grupy ">H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= i zbioru ">aH<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=. 

W przypadku zbiorów skończonych wszystkie warstwy mają tyle samo elementów co odpowiadająca im grupa. 

Np. ">aH<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= ma tyle samo elementów co ">H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= i tyle samo co ">Ha<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=. 

---

* ">Z_4, H = \{0,2\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Warstwy: 

* ">0 +_4 H = \{0, 2\} = 2 +_4 H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* ">1 +_4 H = \{1, 3\} = 3 +_4 H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Mamy zatem 2 warstwy 

0	| 	1
2	| 	3

Warstwy te są rozłączne, co wynika z innego twierdzenia:

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=aH \cap bH \neq \emptyset \rightarrow aH = bH">

bo nie może być tak, żeby jakiś element był częścią wspólną 

## Dowód rozłączności warstw

Założenie: ">x \in aH \cap bH<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">(?) aH \neq bH<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">x \in aH \cap bH<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, a stąd wynika, że ">( \exists h_1, h_2 \in H)(x ah_1 = ab_2)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Dowód ">aH \neq bH<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">y = aH \rightarrow (\exists h \in H)(y = ah)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Podstawiamy ">a = bh_2 h_1^{-1}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Więc ">y = bh_1 h_1^{-1} h \in bH<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">bh_1 h_1^{-1} h \in H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A więc, gdy mamy grupę. 

---

## Przykłady warstw podgrup c.d.">G<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, podrupa ">H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Warstwy

|H||||
|-|-|-|-|
| a|d|g|j|
| b|e|h|k|
|c|f|i|l|

A więc warstwa jest wielokrotnością wielokrotność elementów grupy. 

Wnioski z twierdzenia

1) Ilość elementów grupy ">G<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (">|G|<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=):

Jeśli ">|G| = p<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (liczba pierwsza), to ">G<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= ma tylko 2 podgrupy: 

* ">H_1 = G<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, 
* ">H_2 = \{1\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (element neutralny) ">Z_2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, ">Z_5<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, ">Z_3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, ">Z_7<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, ">Z_11<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= itd. -- wszystkie one nie mają wlaściwych (definicyjnych) podgrup. 

2) Niech będzie grupa ">Z_12<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to mamy podgrupy o liczbach elementów: 1, 12, 2, 6, 3, 4. 

Pytanie, czy ">Z<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= ma podgrupę 2 elementową -- dzielimy ">Z<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= na 2 i mamy 6, a 6 jest w zbiorze, więc ">12:6 = 2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, a więc mamy ">[0,2]<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=. 

Wniosek: w grupie ">Z_e<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= dla każdego dzielnika istnieje dokładnie 1 podgrupa 

# Ćwiczenia 5 | 05.12.2020

## Kolokwium za 2 tyg., godz. 8.00

## Zadania

1. Znaleźć wszystkie podgrupy (właściwe, tzn. nietrywialne) grup: 

a) ">(Z_{24}, +_{24}, 0)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= różne od całego ">Z_{24}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= oraz ">\{0\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b) ">(Z_{36}, +_{36}, 0)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= różne od całego ">Z_{36}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= oraz ">\{0\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=---

Ad a

Podgrupa ma tyle elementów, ile jest dzielników właściwych liczby elementów. 

A więc dzielniki 24: 1, 24 (te nas nie interesują), 2, 12, 3, 8, 4, 6. 

* 2-elementowa podgrupa: dzielimy ">24 / 2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, mamy 12, podgrupa ">H_2 = \{0, 12}\<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* 12-elementowa podgrupa: ">24 / 12 = 2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- ">H_{12} = \{0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (co 2).

* 3-elementowa podgrupa: ">24 / 3 = 8<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- ">H_3 = \{0, 8, 16\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* 8-elementowa podgrupa: ">24 / 8 = 3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- ">H_8 = \{0, 3, 6, 9, 12, 15, 18, 21\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* 4-elementowa podgrupa: ">24 / 4 = 6<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- ">H_4 = \{0, 6, 12, 18\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* 6-elementowa podgrupa: ">24 / 6 = 4<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- ">H_6 = \{0, 4, 8, 12, 16, 20\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=---

Ad b

Liczba elementów grupy: 36 

Dzielniki: 1, 36 (te nas nie interesują), 2, 18, 3, 12, 4, 9, 6,

Istnieje zatem 7 właściwych podgrup:

* 2-elementowa: ">36/2 = 18<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- ">H_2 = \{0, 18\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* 18-elementowa: ">36/18 = 2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- ">H_{18} = \{0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* 3-elementowa: ">36/3 = 12<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- ">H_3 = \{0, 12, 24\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* 12-elementowa: ">36/12 = 3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- ">H_{12} = \{0, 3, 6, 9, 12, 15, 18, 21, 24, 27, 30, 33\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* 4-elementowa: ">36/4 = 9<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- ">H_4 = \{0, 9, 18, 27\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* 9-elementowa: ">36/9 = 4<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- ">H_9 = \{0, 4, 8, 12, 16, 20, 24, 26, 32\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* 6-elementowa: ">36/6 = 6<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- ">H_6 = \{0, 6, 12, 18, 24, 30\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 

## Generatory podgrup

2. Znaleźć wszystkie podgrupy ">(\mathbb{Z}, +, 0)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (całkowite, z dodawaniem i elementem neutralnym) 

2 podgrupy są trywialne: 
* ">\{0\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- tylko zero (dodawanie 0 do 0 zawsze da 0, więc nie wyjdziemy poza zbiór, 0 też jest elementem neutralnym dodawania), 
* ">\mathbb{Z}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- wszystkie liczby całkowite.

Jeśli do podgrupy weźmiemy ">1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to automatycznie musimy też dodać ">0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (element neutralny) oraz ">-1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (inwers), a dalej cały zbiór liczb całkowitych (dwie jedynki dają ">2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, trzy jedynki -- ">3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= itd.). 

Jeśli do podgrupy weźmiemy ">2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to musi się w niej znaleźć także ">0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= i ">-2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, a także ">4<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= i ">-4<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, ">6<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= i ">-6<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= itd.">1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, ">2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= w powyższych przykładach to **generatory** podgrup: 

* "><1> = <-1> = \mathbb{Z}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* "><2> = <-2> = \{0, 2, -2, 4, -4, ...\} = 2 \cdot \mathbb{Z}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* trójka generuje: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=<3> = \{0, 3, -3, 6, -6...\} = 3 \cdot \mathbb{Z}">

Ogólnie: ">n \cdot \mathbb{Z}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= to zbiór wielokrotności ">n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, (bo ">n = 0, 1, 2...<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=). 

Każdy zbiór wielokrotności jakiejś liczby to jest podgrupa dla każdej liczby naturalnej. 

Podgrupa zerowa to ">\{0\} = 0 \cdot \mathbb{Z}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Podgrupa równa grupie: ">\mathbb{Z} = 1 \cdot \mathbb{Z}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=## Dowód, że nie ma innych podgrup ">\mathbb{Z}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= niż te złożone z wielokrotności poszczególnych liczb całkowitych

Jeśli wezmę grupę ">H \notin \{0\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to w tym zbiorze 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(\exists k \in \mathbb{Z}, k \neq 0) (k \in H)">

-- jeśli jakaś liczba należy do grupy, to z tego wynika, że moduł ">k<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= należy do ">H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, a moduł z ">k<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= to liczba naturalna (">|k| \in H, |k| \in \mathbb{N}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=)

A skoro tak, to taki zbiór liczb naturalnych ma element najmniejszy. Oznaczmy go jako ">n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- najmniejsza liczba naturalna należąca do ">H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=. 

A powiedzieliśmy wcześniej, że ">n \dot \mathbb{Z} \in H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Dowód na to, że innych podgrup liczb całkowitych nie ma: 

Jeśli wezmę jakieś ">m \in H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to mogę podzielić zbiór ">H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= tak, że ">m = qn + r, 0 \leq r < n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">r = m - qn, (m, q \in H)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Ale ">n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= miało być najmniejszą liczbą naturalną, a skoro ">r \in H<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= i ">r < n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to ">r = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Więc ">m = qn \in n\mathbb{Z}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Pokazaliśmy zatem, że ">H \in n\mathbb{Z}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, a więc ">H = n\mathbb{Z}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=. 

A więc innych podgrup liczb całkowitych niż wielokrotności ">n\mathbb{Z}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= nie ma. 

## Przykłady podgrup c.d.

* Liczby zespolone z mnożeniem i jedynką:">(\mathbb{C} \setminus \{0\}, \cdot, 1)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Udowodnić, że następujące zbiory są podgrupami tej grupy

a) ">\mathbb{C}_1 = \{z \in \mathbb{C} : |z| = 1 \}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Liczby ">\mathbb{C}_1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= to takie liczby zespolone, że ich odległość (moduł) jest równy 1, a więc wszystkie leżą na okręgu jednostkowym. 

A zatem 
* ">1 \in \mathbb{C}_1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* jeśli ">z_1, z_2 \in \mathbb{C}_1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to iloczyn ">|z_1 z_2|<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= też powiniem należeć do ">\mathbb{C}_1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=|z_1 z_2| = |z_1||z_2| = 1 \cdot 1 = 1 \rightarrow z_1 \cdot z_2 \in \mathbb{C}_1"> ">z = a + ib<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">|z| = \sqrt{a^2 + b^2}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Liczbę odwrotną do zespolonej: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\frac{1}{a+ib}">

obliczymy przez sprzężenie - przemnożenie przez mianownik: ">\frac{1}{a+ib} \cdot \frac{a-ib}{a-ib}=\frac{a-ib}{a^2-iab+iab+b^2}=\frac{a-ib}{a^2+b^2}=\frac{a}{a^2+b^2} - i\frac{b}{a^2+b^2}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Jeśli ">z \in \mathbb{C}_1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to także ">a^2 + b^2 = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, a więc: ">\frac{a}{a^2+b^2} - i\frac{b}{a^2+b^2}=a+i(-b)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">z^{-1} = a+(-b)i<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">|z^{-1}| = \sqrt{a^2 + (-b)^2} = \sqrt{a^2 + b^2} = \sqrt{1} = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Liczba odwrotna też należy do okręgu jednostkowego,
mamy więc podgrupę:

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=z \in \mathbb{C}_1 \rightarrow z^{-1} \in \mathbb{C}_1">

Dla ">n = 2, 3, 4, ... \mu_n = \{z \in \mathbb{C}: z^n = 1 \}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- zbiór wszystkich pierwiatków ">n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-tego stopnia z jedynki; 
takich pierwiastków jest ">n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=. ">\sqrt[2]{1} = \{1, -1\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\sqrt[4]{1} = \{1, i, -1, -i\} = <i><img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (generowana przez ">i<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=)

A więc 

* ">1 \in \mu_4<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, bo ">1^n = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* jeśli 2 liczby ">z_1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, ">z_2 \in \mu_4<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to ">(z_1 \cdot z_2)^n = z_1 z_2 z_1 z_2... = 
z_1^n \cdot z_2^n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, a już wiemy, że ">z_1^n = 1, z_2^n = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, więc ">1 \cdot 1 = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* skoro ">z \in \mu_n \rightarrow (z^-{1)}^n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to czy element odwrotny też należy? 

Wiemy, że ">z \cdot z \cdot ...\cdot z \cdot z = 1 /\cdot z^{-1}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Jedno ">z<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= się skróci, zostanie ">z \cdot z \cdot... \cdot z \cdot z = 1 \cdot z^{-1}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">z \cdot z \cdot ... \cdot z \cdot z = z^{-1} \rightarrow (z^1)^n = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Co jest analogiczne do generowania przez 1.

---

Jeszcze większą grupą od dotychczasowych jest
 
<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\mu_2 \cup \mu_3 \cup \mu_4">

-- dodajemy wszystkie zbiory. 

A zatem 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\mu_\infty = \mu_2 \cup \mu_3 \cup \mu_4..."> 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\bigcup_n=2^\infty \mu_n">

Z mnożeniem, jeśli ">z_1^n = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to ">z_2^m = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=(z_1 z_2)^nm = z_1^nm \cdot z_2^nm = (z_1^n)^m \cdot (z_2^m)^n
= 1^m \cdot 1^n = 1">

# Wyklad 6 | 12.12.2020

## 1. kolokwium -- 19.12.2020, 8.00-9.30

Zrobić zdjęcie pracy i wysłać na maila

Nie ma zajęć o 13

## Przykłady grup c.d.

Rozważmy grupę -- trójkąt równoboczny o wierzchołkach 1, 2, 3

Grupa izometrii będzie przekształcała ten trójkąt w inne trójkąty: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=GI_\triangle = \{ 1_\triangle, 0_{120\degree}, 0_{250\degree}, s_1 \}">

* ">1_\triangle<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- brak przekształcenia

* ">0_{120\degree}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- obrót o 120 stopni: uzyskamy ">\{2, 3, 1\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* ">0_|240\degree}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- obrót o 240 stopni -- ">\{ 3, 1, 2\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* ">s_1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- symetria osiowa względem osi przechodzącej przez wierzchołek ">1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- ">\{ 1, 3, 2\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* ">s_2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- symetria osiowa względem osi przechodzącej przez wierzchołek ">2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- ">\{ 3, 2, 1\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* ">s_3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- symetria osiowa względem osi przechodzącej przez wierzchołek ">3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- ">\{ 2, 1, 3\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=|0| ">1_\triangle<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">0_{120\degree}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">0_{240\degree}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">s_1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">s_2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">s_3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | 
|-|-|-|-|-|-|-|
| ">1_\triangle<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">1_\triangle<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">0_{120\degree}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">0_{240\degree}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">s_1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= |  ">s_2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= |  ">s_3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= |
| ">0_{120\degree}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">0_{120\degree}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">0_{240\degree}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">1_\triangle<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">s_3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">s_1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">s_2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= |
| ">0_{240\degree}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">0_{240\degree}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">1_\triangle<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">0_{120\degree}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">s_2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">s_3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">s_1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= |
| ">s_1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">s_1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">s_3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">s_2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">1_\triangle<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">0_{120\degree}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">0_{240\degree}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= |
| ">s_2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">s_2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">s_1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">s_3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">0_{240\degree}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">1_\triangle<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">0_{120\degree}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= |
| ">s_3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">s_3<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">s_2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">s_1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">0_{120\degree}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">0_{240\degree}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= | ">1_\triangle<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= |

Identyczność ">1_\triangle<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest elementem neutralnym -- nic nie zmienia.

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
* uzupełnianie tabelki z wynikami, np. półgrupy ">Z_4, \cdot_4<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (mnożenie modulo 4)
* znajdowanie wszystkich podgrup jakiejś grupy, np. ">Z_{12}, +_2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (dodawanie modulo 2)
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

Zapis skrótowy cyklu: ">(1, 3, 4, 5)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=---

Permutacja: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\alpha = \Bigl( \begin{matrix} 1&2&3&4&5&6&7&8&9&10 \\ 4&5&2&6&3&8&2&1&9&10 \end{matrix} \Bigr)">

-- posiada 2 cykle: 
* ">(1, 4, 6, 8)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (to skrótowy zapis z identycznościami w miejscu tych liczb, które nie mają znaczenia:
1 2 3 4 5 6 7 8 9 10
4 2 3 6 5 8 7 1 9 10 

* ">(2, 5, 3)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 
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

Funkcją ">f : A \rightarrow B<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (odwzorowującą ">A<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= w ">B<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, gdzie ">A<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, ">B<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= to grupy), nazywamy **homomorfizmem**, gdy dla dowolnych ">x<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, ">y<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= należących do ">A<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= zachodzi, że jeśli wymnożymy ">x<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= i ">y<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= i prześlemy do ">f<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to uzyskamy to samo co w wyniku mnożenia wyników przesłania osobno ">x<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= do ">f<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= i ">y<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= do ">f<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=: 

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

Np. dla ">x = 1000<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">1000 \dot 10000<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">\lg{1000} + \lg{10000} = 3 + 4 = 7<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Wracamy: ">10^7 = 1000000$













 
























> Written with [StackEdit](https://stackedit.io/).


