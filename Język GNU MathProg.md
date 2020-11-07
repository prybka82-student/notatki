### Spis treści
* [Dokumentacja](#Dokumentacja)
* [Struktura zadań programowania liniowego](#Struktura-zadań-programowania-liniowego)

# Dokumentacja[^](#Spis-treści)

[http://gusek.sourceforge.net/gmpl.pdf](http://gusek.sourceforge.net/gmpl.pdf)

# Struktura zadań programowania liniowego[^](#Spis-treści)

Funkcja celu -- do zmaksymalizowania lub zminimalizowania:

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=z = c_1 x_1 + c_2 x_2 + ... c_n x_n + c_0">
 
Ograniczenia liniowe (s.t. -- subject to):

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=L_1 <= a_11 x_1 + a_12 x_2 + ... + a_1n x_n <= U_1">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=L_2 <= a_21 x_1 + a_22 x_2 + ... + a_2n x_n <= U_2">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=...">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=L_m <= a_m1 x_1 + a_m2 x_2 + ... + a_mn x_n <= U_m">  

Ograniczenia zmiennych:

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=l_1 <= x_1 <= u_1">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=l_2 <= x_2 <= u_2">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=...">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=l_n <= x_n <= u_n">

gdzie:
-   <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x_1, x_2, ..., x_n"> -- zmienne    
-   <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=z"> -- warto

# Dopuszczalne znaki w kodzie

- wielkie litery ASCII: ``A B C D E F G H I J K L M N O P Q R S T U V W X Y Z``;
- małe litery ASCII: ``a b c d e f g h i j k l m n o p q r s t u v w x y z``;
- cyfry: ``0 1 2 3 4 5 6 7 8 9 ``;
- znaki specjalne ASCII: ``~ ! # ^ & * ( ) _ + - = [ ] { } | ; : ' " , . / < >``.

# Identyfikatory (_symbolic names_)

Pierwszy znak: 

- mała litera, np. ``alpha123``;
- wielka litera, np. ``Alpha123``;
- podkreślnik, np. ``_alpha123``.

# Literały

## Literały napisowe

- Pojedynczy cudzysłów, np. ``'abc'``
- Podwójny cudzysłów, np. ``"abc"``
- Sekwencja ucieczki dla apostrofu, np. ``'that''s all'``
- Sekwencja ucieczki dla cudzysłowu, np. ``"he said ""hello"""``

## Literały liczbowe

- ``123``
- ``123.123``
- ``.123``
- ``123.E+123``
- ``123.123e-123``

# Słowa kluczowe

Zarezerwowane słowa kluczowe (nie mogą być identyfikatorami): 

``and   or   if   else   by   cross   diff   div   in   inter   less   mod   not   symdiff   then   union   within``

# Ograniczniki wyrażeń (_expression delimiters_)

``+   -  *   **   &   &&   =   ==   /   <   <=   <>   >>   <-   >   >=   !=   !   |   ||   ^   .   ..   ,   :   :   ;=   ~   (   )   [   ]   {   }``

Wieloznakowe ograniczniki nie mogą zawierać spacji.

Niektóre ograniczniki nie mają znaczenia: ułatwiają tylko czytanie kodu i można je pominąć. 

# Komentarze

- Jednowierszowe, np. ``# abc``
- Wielowierszowe, np. ``/* abc */``

# Wyrażenia

- Numeryczne (_numeric expressions_)
- Symboliczne (_symbolic expressions_)
- Indeksujące (_indexing expressions_)
- Zbiorowe (_set expressions_)
- Logiczne (_logical expressions_)
- Liniowe (_linear expressions_)

## Wyrażenia numeryczne

Formuła zwracająca wartość pojedynczej zmiennej typu zmiennoprzecinkowego. 

Szczególne przypadki: 

### Literały liczbowe

Np. ``123``, ``123.123``, ``.123``, ``123.123e-123``.

### Indeksy

Np. ``i`` w ``a[i]``.

### Parametry

Np. ``alpha``, ``time_start``, ``x``, ``a[i]``.

### Wyrażenia warunkowe (_conditional expressions_)

Kod: 

```if i in I then 2 * p else q[i + 1]```

Zapis w języku ``C#``:

```csharp
if (I.contains(i))
	return 2*p;
else
	return q[i+1];
```

---

Kod: 

```if i == 2 then 3```

-- jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=i \neq 2">, wyrażenie ma wartość <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0">.

### Wywołania funkcji (_function references_)

| Składnia | Funkcja |
| --- | --- | 
| ``abs(x)`` | wartość bezwzględna <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x"> |
| ``atan(x)`` | _arcus tangens_ z <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x"> |
| ``atan(x, y)`` | _arcus tangens_ z <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\frac{y}{x}"> |
| ``card(X)`` | moc zbioru (_cardinality_) -- liczba elementów zbioru <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=X"> |
| ``ceil(x)`` | sufit (_ceiling_), zaokrąglenie w górę do najbliższej całkowitej |
| ``cos(x)`` | _cosinus_ z <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x"> |
| ``exp(x)`` | eksponenta, funkcja <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=e^x"> |
| ``floor(x)`` | podłoga (_floor_), zaokrąglenie w dół do najbliższej całkowitej |
| ``gmtime()`` | liczba sekund od północy 1 stycznia 1970 do teraz |
| ``length(s)`` | długość napisu <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s"> (liczba znaków) |
| ``log(x)`` | logarytm naturalny z <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x"> |
| ``log10(x)`` | logarytm przy podstawie 10 z <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x"> |
| ``max(a_1,a_2,...,a_n)`` | maksymalna wartość z podanych |
| ``min(a_1,a_2,...,a_n)`` | minimalna wartość z podanych |
| ``round(x)`` | zaokrąglenie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x"> to najbliższej całkowitej |
| ``round(x, n)`` | zaokrąglenie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x"> do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n"> liczb po przecinku |
| ``sin(x)`` | _sinus_ z <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x"> |
| ``sqrt(x)`` | pierwiastek kwadratowy z <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x"> |
| ``str2time(s, f)`` | konwersja napisu <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s"> na datę w formacie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=f"> |
| ``tan(x)`` | _tangens_ z <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x"> |
| ``trunc(x)`` | odcięcie cyfr po przecinku (bez zaokrąglania) |
| ``trunc(x, n)`` | odcięcie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n"> cyfr po przecinku (bez zaokrąglania) |
| ``Irand224()`` | liczba pseudolosowa z przedziału <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=[0, 2^{24})"> |
| ``Uniform01()`` | liczba pseudolosowa z przedziału <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=[0, 1)"> |
| ``Uniform(a, b)`` | liczba pseudolosowa z przedziału <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=[a, b)"> |
| ``Normal01()`` | generate Gaussian pseudo-random variate with <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mu = 0"> and <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\sigma = 1"> |
| ``Normal(u, s)`` | generate Gaussian pseudo-random variate with given <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=u"> and <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s"> |



### Wyrażenia iterowane (_iterated expressions_)

Kod: 

```sum{i in S diff T} a[i] * b[i, j]```

Zapis matematyczny:

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\sum_{i \in S \setminus T} {a_i b_{ij} }">

---

Kod: 

```prod{i in I} f(i)``

Zapis matematyczny: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\prod_{i \in I} f(i)">

---

Kod: 

```min{i in I} f(i)```

Zapis matematyczny: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=min_{i_1, ..., i_n \in I} f(i)">

-- minimalna wartość funkcji <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=f"> obliczanej dla parametrów od <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=i_1"> do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=i_n"> ze zbioru <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=I">. 

---

Kod: 

```max{i in I} f(i)```

Zapis matematyczny: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=max_{i_1, ..., i_n \in I} f(i)">

## Parametr indeksowany (_subscripted parameter_)

Kod: 

```a[i, j]```

Zapis matematyczny: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a_{ij}">

---

Kod: 

```a['maj 2003', j + 1]```

Możliwe zapisy w języku ``C#``:

```csharp
a.Where(date = "maj 2003" && index = j+1);

a["maj 2008"][j+1]; //z przeciążeniem indeksatora
```

## Wyrażenia symboliczne 

Wyrażenia zwracające ciągi znaków. 

Przypadki szczególne: 

### Literały

Np. ``abc``, ``1 maja 2020``.

### Indeksy

Np. ``i`` w ``nazwy[i]``.

### Parametry

Np. ``x``, ``nazwy``, ``nazwy['a']``, ``nazwy[3]``.

### Wyrażenia warunkowe

Jak wyżej. 

### Wywołania funkcji

| Składnia | Funkcja |
| --- | --- | 
| ``substr(s, x)`` | Fragment napisu <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s"> zaczynający się od znaku <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x"> |
| ``substr(s, x, y)`` | Jw., ale o długości <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=y"> |
| ``time2str(t, f)`` | Konwersja czasu <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=t"> na napis w formacie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=f"> |

## Wyrażenia indeksujące (_indexing expressions_) i wskaźniki nieme (_dummy indices_)

Przeliczalne (enumerowalne) kolekcje elementów. 

| Składnia | Zawartość | 
| --- | --- |
| ``i in S`` | zbiór jednoelementowych krotek z indeksem niemym <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=i"> |
| ``(i_1, i_2, ..., i_n) in S`` | zbiór n-elementowych krotek z ideksami niemymi <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=i_1">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=i_2"> do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=i_n"> |
| ``S`` | zbiór o nazwie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=S"> |
| ``{ a, b, c }`` | zbiór bez nazwy |
| ``{ a, b, c : >= 0 }`` | zbiór bez nazwy z ograniczeniem |
| ``{ i in I, (i, j) in B}`` | zbiór składający się ze zbioru jednoelementowych krotek (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=I">) i zbioru dwuelementowych krotek (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=B">) |

### Indeksy nieme

Nie są stosowane do wskazania elementu kolekcji, ale tylko wskazują, że mamy do czynienia ze zbiorem. Można jednak stosować je jako zmienną w operacjach. 

| Operator niemy w GNU MathProg | operator niemy w językach programowania |
| --- | --- |
| ``i in I`` |``I.select(i => i); //C#`` |
| ``action{ i in A, (j, k) in B, l in C } x(i, j, k, l)`` | ``for i in A: #Python``<br/>&nbsp;&nbsp;&nbsp;``for (j, k) in B:``<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;``for l in C:``<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;``x = (i, j, k, l)``<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;``action(x)`` |

Widoczność indeksu niemego ogranicza się do wyrażenia, np. 

``i in I i ^^ 2; # OK``

``i in I; i ^^ 2; # błąd: i jest niezdefiniowane``

Przykłady: 

- Suma wyrażeń

Kod: 

``sum{i in A, (j, k) in B, l in C} p[i, j, k, l]``

Zapis matematyczny: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\sum_{i \in A, (j, k) \in B, l \in C} p_{ijkl}">

* Iloczyn kartezjański

Kod:

``{A, B, C}``

Zapis matematyczny: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=A \times B \times C = \{  (i, j, k, l) : i \in A, (j, k) \in B, l \in C \}">

Przykładowe wartości zbiorów: 

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A = { 1, 2 }">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=B = { (a, 1), (b, 2) }">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=C = { x, y, z }">

Wartości iloczynu <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A \times B \times C">: 

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={1, a, 1, x}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={1, a, 1, y}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={1, a, 1, z}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={1, a, 2, x}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={1, a, 2, y}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={1, a, 2, z}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={1, b, 1, x}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={1, b, 1, y}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={1, b, 1, z}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={1, b, 2, x}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={1, b, 2, y}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={1, b, 2, z}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={2, a, 1, x}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={2, a, 1, y}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={2, a, 1, z}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={2, a, 2, x}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={2, a, 2, y}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={2, a, 2, z}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={2, b, 1, x}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={2, b, 1, y}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={2, b, 1, z}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={2, b, 2, x}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={2, b, 2, y}">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math={2, b, 2, z}">

---

* Parametr zawierający zbiory

Kod: 

``param p{i in A, (j, k) in B, l in C};``

Analogiczny obiekt w języku ``C#``:

```csharp
var p = new
{
	A = new int[2],
	B = new (int, string)[2],
	C = new string[3]
};
```



# Operatory

## Operatory arytmetyczne (_arithmetic operators_)

| Składnia | Liczba argumentów | Funkcja |
| --- | --- | --- |
| ``+x`` | 1 | zmiana znaku |
| ``-x`` | 1 | zmiana znaku | 
| | | |
| ``x + y`` | 2 | dodawanie |
| ``x - y`` | 2 | odejmowanie | 
| ``x less y`` | 2 | odejmowanie dodatnie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0">, jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x - y < 0">, w przeciwnym razie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x - y">[^a] |
| ``x * y`` | 2 | mnożenie | 
| ``x / y`` | 2 | dzielenie rzeczywiste |
| ``x div y`` | 2 | dzielenie całkowite |
| ``x mod y`` | 2 | reszta z dzielenia |
| ``x ** y``, ``x ^ y`` | 2 | potęgowanie (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x^y">) |

[^a]: Przykłady:
``3 less 1`` <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math==2"> 
``3 less 2`` <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math==1">
``3 less 3`` <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math==0"> 
``3 less 4`` <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math==0">
``3 less 5`` <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math==0"> 

## Hierarchia operatorów arytmetycznych

1. Funkcje, np. ``abs``, ``ceil``.
2. Potęgowanie: ``x ** y``, ``x ^ y``.
3. Zmiana znaku: ``-x``, ``+x``.
4. Mnożenie, dzielenie, reszta z dzielenia: ``x * y``, ``x / y``, ``x div y``, ``x mod y``.
5. Operatory iteracyjne: ``sum``, ``prod``, ``min``, ``max``.
6. Dodawanie i odejmowanie: ``x + y``, ``x - y``, ``x less y``.
7. Wyrażenia warunkowe: ``if x then y``, ``if x then y else z``.

## Operatory symboliczne (znakowe)

| Składnia | Liczba argumentów | Funkcja |
| --- | --- | --- |
| ``a & b`` | 2 | Konkatenacja (złączenie) napisów <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> i <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b"> |

## Hierarchia operatorów symbolicznych

1. Funkcje. 
2. Konkatenacja. 
3. Wyrażenia warunkowe. 





> Written with [StackEdit](https://stackedit.io/).


