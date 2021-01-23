
# Wykład 1 + Laboratorium 1 | 11.10.2020 | Podstawowe definicje i pojęcia

## Kontakt 

- Teams -- czat, dzwonić, jeśli p. prof. jest dostępny, okno dialogowe przy zgłaszaniu zadania. 
- Mail uczelniany: [wwieczorek@ath.bielsko.pl](mailto:wwieczorek@ath.bielsko.pl)
- Dostęp w czasie zajęć

## Semestralny plan wykładu

1. Wstęp i podstawowe pojęcia
2. Programowanie liniowe, całkowitoliczbowe i zero-jedynkowe
3. Algorytm podziału i ograniczeń
4. Programowanie dynamiczne
5. Metody heurystyczne (VNS, GA)
6. Zaokrąglanie randomizowane
7. Answer set programming (ASP)
8. Satisfiability modulo theories (SMT)
9. Algorytmy zachłanne 

---

Z3 -- biblioteka Microsoftu do modelowania matematycznego.

Algorytmy zachłanne -- zachłanność: jeśli w kolejnym kroku algorytmu mamy kilka możliwości, to wybieramy taką, która jest najlepsza z pewnych względów. 
    
Metody heurystyczne -- dają wynik przybliżony, nie idealny (można znaleźć lepszy wynik), ale są szybkie. 

----------

## Zaliczenie

Po omówieniu zagadnienia (co 2 tygodnie) do zrobienia program komp. rozwiązujący zadanie związane z tym zagadnieniem. 

Do oddania po ogłoszeniu zadania tydzień + 1 dzień (do drugiego poniedziałku po zjeździe włącznie). 

Ocena dwukryterialna
* czas działania -- nie dłużej niż wymagany minimalny czas; 
* jakość rozwiązania.
 
Ocena z ćwiczeń -- średnia z wszystkich programów.

Ocena z wykładu -- test 1-krotnego wyboru na moodle. 

Możliwe, że ocena co najmniej dobra zwalnia z zaliczenia z wykładu.

Jeśli jakieś zadanie nieoddane, to liczone jako 0 (obniża średnią). 

Aspekty techniczne rozwiązań

-   dowolny język programowania
-   zadanie w 1 paczce, np. zip, 7z, rar z plikiem wykonywalnym, kodem wykonywalnym, ew. inne pliki związane z projektem -- przesłane na platformie Ms Teams
-   dane wejściowe odczytywane z pliku (nazwa pliku przekazywana jako parametr do wykonania programu)
-   można też przesłać kod źródłowy do skompilowania
-   program ma być konsolowy, wynik wypisywany w konsoli
-   liczy się sposób rozwiązania, nie język -- np. C++ będzie szybszy niż Python
-   C# prof. Wieczorek nie zna, więc nie pomoże, ale zna C++, Java, Go...
-   ==wywołanie w konsoli, np. program.exe nazwa_pliku_z_danymi.txt (tak to docelowo powinno działać)==
    
## Kategorie problemów optymalizacyjnych

Problemy optymalizacyjne można podzielić na:

* **ciągłe** -- badana dziedzina jest ciągła (to dane ciągłe), np. liczby rzeczywiste
* **dyskretne** -- badane obiekty są przestrzenie dyskretne, np. zbiory, podzbiory, liczby całkowite. 

==Na zajęciach tylko problemy dyskretne.==

Jeśli dziedzina ciągła -- **optymalizacja ciągła**. 

Jeśli dziedzina dyskretna -- **optymalizacja dyskretna**.

---

Przykłady

1. Problem ciągły.

Dla jakiego <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x \in \mathbb{R}^2"> funkcja: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=f(x) = 100(x_2 - x_1^2) + (1-x_1)^2">

przyjmuje najmniejszą wartość. 

2. Problem dyskretny.

Problem plecakowy -- plecak ma pojemność 15 kg. Jak dobrać rzeczy do plecaka, by zabrać najwięcej (każdy obiekt ma etykietę walutową do oznaczenia jego wartości). 

## Definicja problemu optymalizacyjnego

Problem optymalizacyjny możemy zdefiniować jako parę <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(F, c)">, gdzie

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=F"> -- (ang. *feasible* 'dopuszczalny') dowolny zbiór dopuszczalnych rozwiązań, 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c"> -- (ang. *cost*)  funkcja kosztu, która każdemu elementowi z <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=F"> przyporządkowuje pewien koszt rzeczywisty: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=c: F \rightarrow \mathbb{R}^1">

Rozwiązanie problemu, to element <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=f \in F">, dla którego zachodzi:

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=c(f) \leq c(y), y \in F">

-- koszt <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=f"> jest mniejsz lub równy od kosztu każdego innego rozwiązania. 

Rozwiązanie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=f"> nazywamy ==**optimum globalnym**== lub ==**optymalnym rozwiązaniem**==. 

Jeśli cel określony jest relację <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c(f) \geq c(y)">, to wówczas <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c"> jest funkcją zysku, a zadanie polega na maksymalizacji wyniku. 

### Przykład: problem ciągły (ad 1) 

* Dziedzina dopuszczalnych rozwiązań: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=F = \mathbb{R}^2">
* Funkcja kosztu: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c = f(x)"> 

### Przykład: problem plecakowy (ad 2) 

* Dziedzina dopuszczalnych rozwiązań: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=F = \ {U' \in 2^U: \sum_{u\in U'} r_u \leq B\}">

-- każdy podzbiór <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=U'"> zbioru przedmiotów <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=U">, dla którego suma rozmiarów <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=r_u"> tych przedmiotów nie przekracza wielkości plecaka <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=B">. 

---

### Przykład:  problem komiwojażera (TSP)

Mamy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n > 0"> miast oraz odległości między miastami zadane macierzą <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n \times n: [d_{ij}]">, gdzie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=d_{ij} \in \mathbb{Z}^+">.

Miasta tworzą wierzchołki grafu pełnego, którego krawędzie mają długość <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=d_ij">. 

Cel: znaleźć cykl Hamiltona o najmniejszej długości. 

* zbiór dopuszczalnych rozwiazań: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=F = \{ \text{permutacje jednocyklowe}\ \pi n\ \text{miast}\}">

-- <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\pi"> to bijekcja -- funkcja przyporządkowująca każdego elementowi inny element, np. <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\pi(2)=4"> oznacza przejście z miasta 2. do 4.

* funkcja celu: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=c = \sum_{j=1}^n d_{j\pi(j)}">

### Permutacje jednocyklowe

-- pojedyncze cykle pojawiające się w permutacjach wierzchołków bez powtórzeń. 

Np. dla kliki składającej się z wierzchołków <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\{1, 2, 3\}"> mamy 6 permutacji, w których pojedyncze cykle występują 2 razy. 

|Permutacje|Przejścia|Cykle|Permutacja 1-cyklowa|
|-|-|-|-|-|-|
|123| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\leftarrow"> początek przejść |||
|123|z 1 do 1, 2 do 2, 3 do 3 -- niemożliwe w problemie TSP[^nie]|3|nie|
|132|z 1 do 1, z 2 do 3, z 3 do 2 -- jw. | 2 |nie|
|213|z 1 do 2, z 2 do 1, z 3 do 3 -- jw. | 2 |nie|
|231|z 1 do 2, z 2 do 3, z 3 do 1 -- OK | ==1== | tak |
|312|z 1 do 3, z 3 do 2, z 2 do 1 -- OK | ==1== | tak |
|321|z 1 do 3, z 3 do 1, z 2 do 2 -- niemożliwe w TSP | 2 |nie|

[^nie]: Komiwojażer musi odwiedzić wszystkie miasta, a nie iść z jednego do tego samego. 
  
### Minimalne drzewo rozpinające (MST)

Mamy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n"> punktów i odległości <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=[d_{ij}], d_{ij} \in \mathbb{Z}^+"> między nimi. 

Zadanie: znaleźć takie drzewo zawierające wszystkie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n"> punktów, aby suma długości jego krawędzi (odległości między punktami) była najmniejsza. 

* Dopuszczalne rozwiązania: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=F = \{ \text{ drzewa rozpinające}\ (V, E) \}">

* Funkcja celu: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=c = \sum_{\{v_i, v_j \} \in E} d_{ij},\ \text{gdzie}\ V = \{v_1, \dots, v_n \}">

## Definicja sąsiedztwa

Mając problem optymalizacyjny <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(F, c)">, ==**sąsiedztwo** <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=N(f)">== jest odwzorowaniem: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=N: F \rightarrow 2^F">

-- czyli sąsiedztwo to dowolna funkcja przyporządkowująca rozwiązaniom <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=F"> pewien podzbiór <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2^F"> tych rozwiązań. 

### Przykłady

* Dopuszczalne rozwiązania: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=F = \mathbb{Z}"> -- wszystkie liczby całkowite
* Sąsiedztwo: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=N = \mathbb{Z} \rightarrow 2^\mathbb{Z}, N(x) = \{x-1, x+2\}"> -- funkcja określająca podzbiór <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2^\mathbb{Z}"> zbioru liczb całkowitych <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Z}"> składający się z par wierzchołków sąsiadujących -- poprzedniego i następnego

## Definicja optimum lokalnego 

Mając 

* problem optymalizacyjny <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(F, c)">
* sąsiedztwo <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=N">

-- dopuszczalne rozwiązanie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=f \in F"> jest ==**optimum lokalnym**== (względem <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=N">), gdy

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=c(f) \leq c(g) \ \text{dla wszystkich}\ g \in N(f)">

-- koszt tego rozwiązania _f_ (optimum lokalnego) jest mniejsze lub równe od kosztu dowolnego jego sąsiada. 

### Przykład: max cut

Problem: 
* znaleźć podzbiór <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=C"> wierzchołków grafu <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G = (V,E)">, 
* liczba krawędzi podzbioru <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=C"> takich, że jeden ich koniec jest w <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=C">, a drugi w <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G">, ma być największa
  
## Terminy z algebry

| Oznaczenia | Wartość | 
|-|-|
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{R}"> lub <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{R}^1"> | zbiór liczb rzeczywistych |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{R}^n"> | uporządkowane <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n">-tki (krotki -- iloczyny kartezjańskie) liczb rzeczywistych |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{R}^+"> | nieujemne liczby rzeczywiste |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Z}"> | liczby całkowite |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Z}^+"> | nieujemne liczby całkowite |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\mathbb{Z}^n"> | uporządkowane <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n">-tki liczb całkowitych |

## Definiowanie zbiorów

| Oznaczenie | Wartość |
|-|-|
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=S = \{ s_1, s_2, \dots \}"> | zbiór składający się z elementów <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=s_i"> |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=S = \{x : P(x)\}"> | zbiór wszystkich elementów <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x"> spełniających warunek <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=P"> |
| \|S\| | liczba elementów zbioru <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=S"> (jego liczność |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2^S"> | zbiór wszystkich podzbiorów <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=S"> | 

## Macierze 

| Oznaczenie | Wartość |
|-|-|
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=[a_{ij}]"> | macierz o wymiarach <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=m \times n"> (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=m"> wierszy i <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n"> kolumn) |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a_{ij}"> | element macierzy w wierszu <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=i"> i kolumnie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=j"> |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A^T"> | macierz transponowana | 

Przykład macierzy transponowanej: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=  A = \left [ \begin{array}{ccc} a&b&c \\ d&e&f \end{array} \right ], A^T = \left [ \begin{array}{cc} a&d \\ b&e \\ c&f \end{array} \right ] ">

## Mnożenie macierzy

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=A = \left [ \begin{array}{cc} a&b \\c&d \\ e&f \end{array} \right ], B = \left [ \begin{array}{ccc} i&j&k \\ l&m&n \end{array} \right ] ">

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=A \cdot B = \left [ \begin{array}{ccc} 
ai+bl & aj+bm & ak+bn \\ 
ci+dl & cj+dm & ck+dn & \\ 
ei+fl & ej+fm & ek+fn 
\end{array} \right ]">

## Układ równać w postaci macierzy 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\begin{matrix}
a_{11}x_1 + a_{12}x_2 + \dots + a_{1n}x_n = b_1 \\
a_{21}x_1 + a_{22}x_2 + \dots + a_{2n}x_n = b_2 \\
\dots \\
a_{m1}x_1 + a_{m2}x_2 + \dots + a_{mn}x_n = b_m \\ \end{matrix}">

Skrótowy zapis: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=Ax = b">

## Terminologia grafów

**Graf (nieskierowany)** <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G"> -- para <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(V, E)">, gdzie 

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=V"> -- skończony zbiór wierzchołków, 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=E"> -- zbiór krawędzi -- dwuelementowych (niuporządkowanych) podzbiorów <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=V">

Reprezentacja, np. 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=G = (\{a, b, c, d\}, \{\{a, b\}, \{a, c\}, \{b, c\}, \{b, d\}\})">

**Graf skierowany** -- graf, którego krawędzie mają określony kierunek. Dokładniej: skierowany graf <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=D"> jest parą <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(V, E)">, gdzie 

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=V"> -- skończony zbiór wierzchołków, 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=E"> -- zbiór uporządkowanych par wierzchołków (tzw. łuków).

Reprezentacja, np. 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=D = (\{a, b, c, d\}, \{(a, b), (a, c), (b, c), (b, d)\})">

**Stopień wierzchołka** <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=v \in V"> w grafie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G = (V, E)"> to liczba krawędzi, których końcem jest wierzchołek <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=v">. 

**Droga** -- zbiór wierzchołków połączonych ze sobą krawędziami w taki sposób, że można przejść od pierwszego do ostatniego z tych wierzchołków, przechodząc przez każdy z wierzchołków tego podzbioru. 

**Długość drogi** -- liczba wierzchołków wchodzących w jej skład pomniejszona o 1. 

**Droga zamnięta** <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=w = (v_1, v_2, \dots, v_k)"> (gdzie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=k > 1">) to taka droga, w której <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=v_1 = v_k">. 

**Cykl** -- droga zamknięta, w której poza pierwszym i ostatnim wierzchołkiem żaden inny wierzchołek się nie powtarza. 

**Cykl Hamiltona**  -- cykl przechodzi przez wszystkie wierzchołki tylko 1 raz. 

**Graf spójny** -- graf  w 1 kawałku, ściślej: graf, w którym dowolne 2 wierzchołki można połączyć drogą. 

**Graf niespójny** -- w kilku kawałkach (nie wszystkie 2 dowolne wierzchołki można połączyć drogą). 

**Graf dwudzielny** -- graf <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G">, którego wierzchołki tworzą dwa rozdzielne podzbiory <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=U"> i <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=V"> nie połączonych ze sobą wierzchołków -- nie ma krawędzi łączącej dowolne dwa wierzchołki ze zbioru <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=U"> oraz <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=V">; krawędzie łączą jedynie wierzchołki należące do różnych podzbiorów wierzchołków. 

Oznaczenie: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=B = (U, V, E)">

**Izomorfizm grafów** -- identyczność grafów (mimo że tego nie widać -- graf może być inaczej narysowany); ściślej: dwa grafy są izomorficzne, jeśli istnieje wzajemnie jednoznaczna odpowiedniość między wierzchołkami obu grafów taka, że liczba krawędzi łączących dopasowane do siebie wierzchołki jest taka sama w obu grafach. 

**Graf pełny** -- zawiera maksymalną liczba krawędzi -- każdy wierzchołek jest połączony z wszystkimi pozostałymi. 

**Klika** -- (największy) podzbiór wierzchołków, w którym każdy wierzchołek połączony jest wszystkimi pozostałymi wierzchołkami tego grafu (są one wzajemnie sąsiednie -- każdy sąsiaduje z każdym). 

**Klika maksymalna** -- klika nie będąca podzbiorem większej kliki. 

**Drzewo** -- graf spójny bez cykli. 

Twierdzenie o grafach i drzewach: jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G = (V, E)"> jest grafem, wówczas

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G"> jest drzewem wtedy, gdy
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G"> jest spójny i ma <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=|V|-1"> krawędzi, wtedy, gdy 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=G"> nie ma cykli, ale po dodaniu 1 krawędzi powstaje cykl.

## Literatura

![](https://www.evernote.com/shard/s443/res/747baff4-aab9-8ac2-aa4f-29c76aa94179)
  
# Wykład 2 | 24.10.2020 | Programowanie liniowe -- aspekty praktyczne

## Definicja problemu optymalizacyjnego

To para <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=F">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c">, gdzie: 

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=F"> -- zbiór dopuszczalnych rozwiązań
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c"> -- funkcja kosztu

Dopuszczalne rozwiązania to wszystkie iksy, które: 

* są liczbami rzeczywistymi (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\forall_{i \in [1, n]} x_i \in \mathbb{R}">)
* spełniają warunek <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\forall_{i \in [1, m], j \in [1, n]} a_{ij}x_j = b_i">
* i są nieujemne (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\forall_{i \in [1, n]} x_i \geq 0">)

Co można zapisać jako: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=F = {x: x \in \mathbb{R^n}, Ax = b, x \geq 0}">

A funkcja kosztu przypisuje każdym iksom wartość <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c^Tx">: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math= c: x \rightarrow c^Tx ">

co jest skrótowym zapisem sumy iloczynów: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=c_1x_1 + c_2x_2 + c_3x_3 + \dots + c_nx_n"> 

Przyjmujemy, że współczynniki <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a_{ij}">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b_i"> i <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c_i"> są liczbami całkowitymi:

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a_{ij} \in \mathbb{Z}, b_i \in \mathbb{Z}, c_i \in \mathbb{Z}">

Macierz <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=A"> ma wymiary <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=m \times n">. 

Wektor <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b"> ma wymiar <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=m">. 

Wektor <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c"> ma wymiar <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n">.

Wektor zmiennych <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x"> ma wymiar <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n">. 

Możemy zatem zapisać problem programowania liniowego jako zbiór równań: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\begin{array}{l l l l l |} 
a_{11}x_1 & + a_{12}x_2 & + \dots & + a_{1n}x_n & = b_1 \\
a_{21}x_1 & + a_{22}x_2 & + \dots & + a_{2n}x_n & = b_2 \\
a_{m1}x_1 & + a_{m2}x_2 & + \dots & + a_{mn}x_n & = b_m
\end{array} \ \min{c_1x_1 + c_2x_2 + \dots + c_nx_n}">

Liczba kolumn wynosi <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n">, co odpowiada liczbie zmiennych

Liczba wierzy wynosi <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=m">, co odpowiada liczbie ograniczeń

## Standardowa postać problemu programowania liniowego

Tradycyjnie problem programowania liniowego zapisuje się jako: 

==<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\min c^Tx"> lub <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\max c^Tx">==
==<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Ax = b">==
==<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x \geq 0">==

tzn. 
* celem zadania jest zminimalizowanie (zmaksymalizowanie) wyrażenia <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c^Tx">
* zachowując jednocześnie warunków:
	* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Ax=b">
	* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x \geq 0">

Zmienna <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x"> jest zasadniczo rzeczywista (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x_i \in \mathbb{R}">). 

Jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x"> jest całkowite, mówimy o **programowaniu całkowitoliczbowym**.

Jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x \in [0, 1]">, to mówimy o **programowaniu zero-jedynkowym**.  

## Inne postaci problemu programowania liniowego

**Postać kanoniczna** -- zamiast równań w psotaci standardowej pojawiają się nierówności. 

**Postać ogólna** -- połączenie obu powyższych: nie wszystkie ograniczenia są równaniami i nie wszystkie zmienne muszą być nieujemne.

| Postać standardowa | Postać kanoniczna | Postać ogólna |
|-|-|-|
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\begin{array}{l} \min{c^Tx}\\Ax = b\\  \\x \geq 0\\ \ \end{array}"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\begin{array}{l} \min{c^Tx}\\Ax \geq b\\ \\x \geq 0 \\ \ \end{array}"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\begin{array}{l l} \min{c^T x} & \\ a^T_i x = b_i & i \in M \\ a^T_i x \geq b_i & i \in \bar{M} \\ x_j \geq 0 & j \in N \\ -\infty < x_j < +\infty & j \in \bar{N} \end{array}"> |

## Użyteczne przekształcenia równań

| Postać wyjściowa | Postacie równoważne | Uwagi |
|-|-|-|
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\sum_{j=1}^n a_{ij}b_j = b_i"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\begin{array}{lrlr} \sum_{j=1}^n & a_{ij}x_j & \geq & b_i \\ \sum_{j=1}^n & -a_{ij}x_j & \geq & -b_i \end{array}"> | [a^]
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-\infty < x_j < +\infty"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\begin{array}{ll} x_j = x_j^+ - x_j^- & x_j^+, x_j^- \geq 0 \end{array}"> | [^b]
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\sum^n_{j=1} a_{ij}x_j \geq b_i"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\begin{array}{ll} \sum^n_{j=1} a_{ij}x_j - s_i = b_i & s_i \geq 0\end{array}"> | [^c]
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\sum^n_{j=1} a_{ij}x_j \leq b_i"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\begin{array}{ll} \sum^n_{j=1} a_{ij}x_j + s_i = b_i & s_i \geq 0\end{array}"> | [^d]
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x \neq y"> | [^e]

[^a]: W uproszczeniu: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a=b \leftrightarrow a \geq b \wedge a \leq b /-1">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a=b \leftrightarrow a \geq b \wedge -a \geq -b">

[^b]: Zmienną nieograniczoną <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x"> zastępujemy dwiema, których różnica musi dać szukaną zmienną. 

Np. jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x=3">, to można tę wartość zapisać np. jako <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x=3=10-7">. 

Oznaczenia w górnym indeksie są konwencjonalne -- równie dobrze można by zapisać: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x_j = \hat{x}_j - \dot{x}_j; \hat{x}_j, \hat{x}_j \geq 0">

[^c]: Nierówność można zamienić na równość przez dodanie dodatkowej zmiennej, np. 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5 \geq 3">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5-2 = 3">

[^d]: Jw., np. 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2 \leq 10">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=2 + 8 = 10">

[^e]: Przekształcenia: 

Jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x \neq y"> to:
* albo <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x < y">
* albo <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x > y">

W solwerach nie da się zwykle łączyć warunków spójnikiem <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\vee"> ('lub'), dostępne są jedynie spójniki <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\wedge"> ('oraz'), trzeba zatem powyższą alternatywę zastąpić koniunkcją.

Jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=y"> są całkowite  i leżą w przedziale <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=[0, k]">, to wówczas: 
* różnica <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x-y=+1">, jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x > y"> i są to kolejne liczby całkowite, np. <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5-4=+1">
* różnica <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x-y=-1">, jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x < y"> i są to kolejne liczby całkowite, np. <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=7-8=-1">
* różnica <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x-y=+k">, jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x > y"> i są to skrajne wartości przedziału: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=k-0=+k">
* różnica <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x-y=-k">, jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x < y"> i są to skrajne wartości przedziału: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0-k=-k">

Innymi słowy: 
* dla <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x > y"> wartość różnicy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x-y"> będzie w przedziale <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=[+1, +k]">
* dla <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x < y"> wartość różnicy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x-y"> będzie w przedziale <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=[-k, -1]">

Co możemy to zapisać jako:
 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=+1 \leq x-y \leq +k">
lub
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-k \leq x-y \leq -1">

Albo z użyciem spójnika <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\wedge"> 'oraz': 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\begin{array}{l}
x-y \geq +1 & \wedge &  x-y \leq +k, & x>y \\
\vee \\
x-y \leq -1 & \wedge & x-y \geq -k, & x<y
\end{array}">

Wprowadzając zmienną pomocniczą <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=z"> przyjmującą dwie wartości: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0"> ***lub*** <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1"> możemy zredukować alternatywę (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\vee"> 'lub') do koniunkcji (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\wedge"> 'oraz'): 

* dla <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=z=0"> mają być spełnione nierówności: 
	* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x-y \geq +1 \wedge x-y \leq +k">
* dla <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=z=1"> mają być spełnione nierówności: 
	* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x-y \leq -1 \wedge x-y \geq -k">

Co można sformułować następująco: 

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x-y \geq +1 - z(k+1)">, co jest równoznaczne z: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=y-x\leq z(k+1)-1">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x-y \leq +k - z(k+1)">

Ostatecznie:

| Postać wyjściowa | Postacie równoważne |
|-|-|
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x \neq y; x, y \in \mathbb{Z} \wedge x, y \in [0, k]"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=y-x \leq z(k+1) - 1\\ \wedge \\x-y \leq k - z(k+1)">

## Zamiana warunków logicznych na równania lub nierówności 

Zakładamy, że <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a, b, c \in [0, 1]">

| Warunek | Równanie lub nierówność | Uwagi |
|-|-|-|
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \wedge b"> (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> i <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b">) | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a = b = 1"> | [^tablica_prawdy] |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \vee b"> (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> lub <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b">) | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a + b \geq 1"> | [^tablica_prawdy] |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \Rightarrow b"> (jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a">, to <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b">) | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b - a \geq 0"> | [^tablica_prawdy] |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \Leftrightarrow b"> (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> wtedy, gdy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b">) | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a - b = 0"> | [^tablica_prawdy] |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \nLeftrightarrow b"> (albo <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a">, albo <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b">) | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a + b = 1"> | [^tablica_prawdy] |
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=ab = c"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=(1-c)+a \geq 1\\(1-c)+b \geq 1\\c+(1-a)+(1-b) \geq 1"> | [^niewlp]


[^tablica_prawdy]: Porównaj tablice prawdy i ich przekształcenia: 
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b"> || <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a\wedge b"> (AND) | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \vee b"> (OR) | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \Rightarrow b"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \Leftrightarrow b"> (IFF) | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \nLeftrightarrow b"> (XOR) |
|-|-|-|-|-|-|-|-|
|||||||||
| 0 | 0 || 0 | 0 | 1 (==<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b-a\geq0">==) | 1 (==<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a-b=0">==) | 0 |
| 0 | 1 || 0 | ==<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1\geq a+b">== | 1 (==<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b-a\geq0">==) | 0 | 1 (==<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a+b=1">==) | 
| 1 | 0 || 0 | ==<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1\geq a+b">== | 0 | 0 | 1 (==<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a+b=1">==) | 
| 1 | 1 || ==<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1=a=b">== | ==<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1\geq a+b">== | 1 (==<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b-a\geq0">==) | 1 (==<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a-b=0">==) | 0 | 

[^niewlp]: Mnożenie zmiennych jest niedopuszczalne w programowaniu liniowym, gdzie możliwe jest jedynie mnożenie stałej przez zmienną i ewentualne sumowanie z inną zmienną lub iloczynu zmiennej i stałej. Por. tablice prawdy dla wartości <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\neg a">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\neg b">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\neg c">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=ab"> i <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=ab=c">:
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\neg a = 1-a"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\neg b = 1-b"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=ab"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\neg c = 1-c"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=ab=c"> | War. |
|-|-|-|-|-|-|-|-|-|
| 0 | 1 | 0 | 1 | 0 | 0 | 1 | ==1== | 1,2,3
| 0 | 1 | 1 | 0 | 0 | 0 | 1 | ==1== | 1,2,3
| 1 | 0 | 0 | 1 | 0 | 0 | 1 | ==1== | 1,2,3
| 1 | 0 | 1 | 0 | 1 | 0 | 1 | 0 | 1,2,x
| 0 | 1 | 0 | 1 | 0 | 1 | 0 | 0 | x,x,3
| 0 | 1 | 1 | 0 | 0 | 1 | 0 | 0 | x,2,3
| 1 | 0 | 0 | 1 | 0 | 1 | 0 | 0 | 1,x,3
| 1 | 0 | 1 | 0 | 1 | 1 | 0 | ==1== | 1,2,3
-- jak widać, wszystkie trzy warunki podane w nierównościach są łącznie spełnione w wówczas, gdy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=ab=c"> ma wartość <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1">. 

## Popularne solwery liniowe

* GLPK (język MathProg)
* COIN-OR (język C++)

## Przykłady

### Problem kliki 

**Kilka** -- podzbiór wierzchołków jakiegoś grafu, w którym to podzbiorze każdy wierzchołek połączony jest z każdym innym wierzchołkiem. 

Znaleźć możliwie największy taki podziór. 

Np. dla grafu danego macierzą sąsiedztwa: 

||1|2|3|4|5|6|
|-|-|-|-|-|-|-|-|
|1|0|1|1|0|0|0|
|2|1|0|1|1|1|0|
|3|1|1|0|0|1|1|
|4|0|1|0|0|1|0|
|5|0|1|1|1|0|0|
|6|0|0|1|0|0|0|

Za zmienne <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x_1, x_2, ... x_n, n=6"> przyjmujemy wierzchołki. Wartość <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x_i = 1"> oznacza, że <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=i">-ty wierzchołek został wzięty do rozwiązania. 

Ograniczenia możemy zdefiniować jako sytuacje, w których dane wierzchołki do rozwiązania jednocześnie wejść nie mogą, bo nie są połączone krawędzią. Połączenie krawędziami możemy modelować jako sumę zmiennych <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x_i">. Np. połączenie wierzchołka 1. i 2.: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x_1 = 1">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x_2 = 1">. Jeśli wierzchołki mają być nie połączone, ich suma nie może przekroczyć 1, a więc <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=x_1 + x_2 + \dots x_n \leq 1">. 

Oto macierz tak zdefiniowanych warunków: 

| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=w_1"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=w_2"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=w_3"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=w_4"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=w_5"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=w_6"> | Objaśnienie |
|-|-|-|-|-|-|-|
|1|0|0|1|0|0|Wierzchołek 1. nie łączy się z 4.|
|1|0|0|0|1|0|Wierzchołek 1. nie łączy się z 5.|
|1|0|0|0|0|1|Wierzchołek 1. nie łączy się z 6.|
|0|1|0|0|0|1|Wierzchołek 2. nie łączy się z 6.|
|0|0|1|1|0|0|Wierzchołek 3. nie łączy się z 4.|
|0|0|0|1|0|1|Wierzchołek 4. nie łączy się z 6.[^w4]|
|0|0|0|0|1|1|Wierzchołek 5. nie łączy się z 6.[^w5]|

[^w4]: Brak połączenia z w. 1. i 3. został już zamodelowany. 

[^w5]: Brak połączenia z w. 1. został już zamodelowany. 

A zatem macierz ograniczeń: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=A = \left [ \begin{matrix}
1&0&0&1&0&0 \\ 1&0&0&0&1&0 \\ 1&0&0&0&0&1 \\ 0&1&0&0&0&1 \\ 0&0&1&1&0&0 \\ 0&0&0&1&0&1 \\ 0&0&0&0&1&1 \end{matrix} \right ] 
b = \left [ \begin{matrix} 1\\1\\1\\1\\1\\1\\1 \end{matrix} \right ]">

Co można zapisać skrótowo: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=Ax \leq b">

Rozwiązanie w języku ``MathProg``: 

Plik ``.mod``

```mathprog
param n, integer, >= 1; # deklaracja liczby wierzcholkow
var x{1..n}, binary; 	# deklaracja wektora zmiennych o n elementach
param k{i in 1..(n-1), j in (i+1)..n}, binary # deklaracja tablicy ograniczen

# cel
maximize size: sum{i in 1..n} x[i];

# ograniczenie
s.t. r{i in 1..(n-1), j in (i+1)..n: k[i,j] == 0}: x[i] + x[j] <= 1;
# suma wierzcholkow, ktore chcielibysmy łączyć nie moze przekroczyc 1 

solve;
display size, x;
end;
```

Plik ``.dat``

```mathprog
param n := 6;
param k := 1 2 1 1 3 1 1 4 0 1 5 0
           1 6 0 2 3 1 2 4 1 2 5 1
           2 6 0 3 4 0 3 5 1 3 6 1
           4 5 1 4 6 0 5 6 0; 
           # zapis: indeks i, indeks j, wartosc 0 lub 1 
           # czy wierzholki i oraz j nie sa/sa polaczone
end;
```

---

### Problem diety 

Mamy 3 produkty spożywcze i podane koszty 1 porcji każdego z nich oraz zawartość witamin i kalorii: 

Produkt | Koszt 1 porcji | Witaminy A w 1 porcji | Kalorii w 1 porcji |
|-|-|-|-|
| Kukurydza | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0,18 | 107 | 72 |
| Mleko 2% | ">0,23 | 500 | 121 |
| Chleb pszenny | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0,05 | 0 | 65 |

Ograniczenia: 

* maksymalna ilość porcji każdego produktu: 10
* suma kalorii: między 2 000 a 2 250
* ilość witaminy: między 5 000 a 50 000

Cel: znaleźć dietę (dobór liczby porcji każdego produktu) o minimalnym koszcie. 

Plik ``.mod``

```mathprog
set Produkty; 				# deklaracja zbioru produktow
param koszt{Produkty};		# deklaracja wektora kosztow kazdego produktu
param witamina{Produkty};	# dekalracja wektora liczby witamin w produkcie
var x{Produkty} >= 0;		# deklaracja zmiennej: ilosc porcji produktu

# cel
minimize cena: sum{p in Produkty} koszt[p] * x[p];

# ograniczenia
s.t. porcje{p in Produkty}: x[p] <= 10;
s.t. iloscWitamin: 5000 <= sum{p in Produkty} witamina[p] * x[p] <= 50000;
s.t. iloscKalorii: 2000 <= sum{p in Produkty} kalorie[p] * x[p] <= 2250;

solve;
display cena, x;
end;
```

Plik ``.dat``
```mathprog
set Produkty := kukurydza mleko chleb; 	# deklaracja zbioru produktow

param:        koszt   witamina   kalorie :=
  kukurydza   0.18    107        72
  mleko       0.23    500        121
  chleb       0.05    0          65;
```

---

### Problem ``MAX CUT``

Problem: podzielić wierzchołki grafu na 2 rozłączne zbiory tak, aby liczba krawędzi łączących wierzchołki obu zbiorów była największa. 

Model: 

* graf ">G = (V, E)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* wierzchołki: ">V = {v_1, v_2, \dots, v_n}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 
* zmienna binarna: ">x_i \in \{0, 1\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=	* ">x_i = 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, gdy wierzchołek ">i<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest wybrany do rozwiązania
	* ">x_i = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, gdy wierzchołek ">i<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= nie jest wybrany do rozwiązania
* cel: zmaksymalizować sumę: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\sum_{\{v_i, v_j\} \in E} x_i\ \text{xor}\ x_j">

Przekształcenie funkcji ``xor``: 

* niech ">x+y = 2c_1 + c_0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, gdzie ">c \in \{0, 1\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= i ">c_0 = x\ \text{xor}\ y<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 
* wówczas ">0 \leq x+y-2c \leq 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Plik ``.mod``

```mathprog
param n, integer, >= 2; 		# liczba wierzcholkow (min. 2)
set V := 1..n; 					# zbior wierzcholkow ideksowanych od 1 do n
set E, within V cross V;		# zbior krawedzie - iloczyn kartez. V
var x{V}, binary; 				# wektor rozwiazan - ktore wierzcholki
var c{E}, binary; 			    # wektor krawedzi 

# cel - jak najwiecej xorow = 1
maximize z: sum{(i,j) in E} (x[i] + x[j] - 2*c[i,j]);   

# ograniczenie - xor w przedziale 0 do 1
s.t. ogr{(i,j) in E}: 0 <= x[i] * x[j] - 2*c[i,j] <= 1;

solve;
display z, x;
end;
```

Plik ``.dat``

```mathprog
param n := 20; 					# liczba wierzcholkow
set E :=
  (1,2) (1,5) (1,10) (1,11) (2,3)
  (3,6) (3,7) (3,10) (4,8) (4,14)
  (4,17) (5,11) (5,13) (5,19) (6,7)
  (6,18) (7,8) (7,10) (8,10) (9,15)
  (12,13) (13,16) (13,19) (14,18)
  (15,18) (16,17) (16,19) (16,20)
  (17,19) (17,20);
end;
```

# Laboratorium 2...

# Wykład 3 | 14.11.2020 | Algorytm podziału i ograniczeń

Z ang. *branch and bound algorithm*. 

Podział -- rozgałęzienie algorytmu (grafu), podział przestrzeni wszystkich rozwiązań na mniejsze podprzestrzenie. 

Ograniczenie -- element wskazujący najlepsze rozwiązanie w danej podprzestrzeni. 
 
## Algorytm

1) Za koszt najlepszego (rozwiązania) przyjmujęmy początkowo nieskończoność

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\text{koszt\_najlepszego} = \infty">

2) Zbiór podprzestrzeni (puntków) -- zwykle stos lub kolejka priorytetowa (z ograniczeniem jako priorytetem), początkowo: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=Z = \{ \text{punkt\_poczatkowy} \}">

3) Wybierz element ">w<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= ze zbioru ">Z<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= i usuń go ze zbioru ">Z<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=4) Oblicz wartość ograniczenia (ang. *bounding*) dla elementu ">w<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=o(w)">

5) Jeśli ">o(w) \geq \text{koszt\_najlepszego}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, idź dalej i nie rozpatruj ">w<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=6) Jeśli ">o(w) < \text{koszt\_najlepszego}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to wówczas: 

	1. Wygeneruj potomki wierzchołka ">w<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=	2. Sprawdź, czy osiągnięto kompletne rozwiązanie. 
	3. Dodaj obiecujące potomki do zbioru ">Z<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 

7) Jeśli ">Z<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= nie jest puste, idź do pktu 3. 

8) Zwróć ">\text{najlepsze\_rozwiazanie}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 

## Przykłady

### Problem komiwojażera

Mamy odległości między miastami: 

||1|2|3|4|5|
|-|-|-|-|-|-|
|1|0|28|25|19|14|
|2|26|0|27|26|25|
|3|15|27|0|14|21|
|4|12|14|13|0|28|
|5|20|23|10|22|0|

(wersja niesymetryczna -- droga z miasta 1 do 2 nie jest równa drodze z 2 do 1).

Zadanie: startując od wskazanego miasta, musimy odwiedzić wszystkie miasta, pokonując jak najkrótszą drogę. 

* Załóżmy, że startujemy z 1. 
* Obliczamy funkcję ograniczenia jako sumę minimalnych odleglości (minimalnych wartości w każdym wierszu): 

	* ">o(1) = 14+25+14+12+10 = 75<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* Usuwamy wierzchołek 1 ze zbioru Z, bo jego ograniczenie jest mniejsze od kosztu, które początkowo jest nieskończone. 

* Znajdujemy potomki wierzchołka 1 i obliczamy dla nich ograniczenie: 
	* 1-2: ">o(2) = 28 + (25+14+12+10) = 28 + 61 = 89<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=	* 1-3: ">o(3) = 25 + (25+14+12+10) = 25 + 61 = 86<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=	* 1-4: ">o(4) = 19 + (25+14+12+10) = 19 + 61 = 80<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=	* 1-5: ">o(5) = 14 + (25+14+12+10) = 14 + 61 = 75<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* 5 jest najbardziej obiecująca (jego ograniczenie = 75), dodaję go do ">Z<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* Wybieram 5. z Z i szukam jego potomków i liczę ich ograniczenia: 
	* 1-5-2: ">o(2) = 14+23 + (25+14+12) = 37 + 51 = 88<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=	* 1-5-3: ">o(3) = 14+10 + (25+14+12) = 24 + 51 = 75<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=	* 1-5-4: ">o(3) = 14+22 + (25+14+12) = 36 + 51 = 87<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* Najbardziej obiecujący jest wierzchołek 3., więc go wybieram i szukam jego potomków: 
	* 1-5-3-2: ">o(2): 14+10+27 + (25+12) = 51 + 37 = 88<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 
	* 1-5-3-4: ">o(2): 14+10+14 + (25+12) = 38 + 37 = 75<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* Najbardziej obiecujący jest wierzchołek 4., więc go wybieram i szukam jego potomków: 
	* 1-5-3-4-2-1: ">\\c(1,5,3,4,2,1)=14+10+14+14 + (26) = 52 + 26 = 78<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* Koszt drogi 1-5-3-4-2-1 wynosi 78, ale w zbiorze Z są jeszcze rozwiązania: 
	* o(1,2) = 89
	* o(1,3) = 86
	* o(1,5) = 80
	* o(1,5,2) = 88
	* o(1,5,4) = 87
	* o(1,5,3,2) = 88

* Żadne z rozwiązań w zbiorze Z nie ma ograniczenia lepszego niż najmniejszy uzyskany koszt, zatem rozwiązaniem jest: 1-5-3-4-2-1

### Problem najkrótszej drogi

Mamy graf skierowany z wyszczególnionym wierzchołkiem początkowym _s_ i końcowym _t_ oraz następującymi wagami krawędzi: 

* s->a: 22
* s->b: 10
* a->c: 23
* b->c: 20
* b->d: 5
* c->t: 12
* d->t 28

Jako funkcję ograniczenia przyjmujemy długość przebytej drogi. 

Algorytm: 

* Rozpoczynamy od wiechołka _s_, dla którego ">o(s) = 0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (drogi wynosi 0).
* Usuwam _s_ z _Z_ 
* Szukamy potomków wierzchołka _s_, dodajemy je do _Z_ i obliczamy ograniczenie: 
	* s-a: ">o(s,a) = 22<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=	* s-b: ">o(s,b) = 10<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* Najbardziej obiecujący jest wierzchołek _b_, usuwam go z _Z_ i szukam jego potomków: 
	* s-b-c: ">o(s,b,c) = 10+20 = 30<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=	* s-b-d: ">o(s,b,d) = 10+5 = 15<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* Najbardziej obiecujący jest wierzchołek _d_, usuwam go z _Z_ i szukam jego potomków: 
	* s-b-d-t -- rozwiązanie jest kompletne, obliczam koszt: 
	* ">c(s,b,d,t) = 10+5+28 = 43<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* W _Z_ są jeszcze: 
	* s-a: ">o(s,a) = 22<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=	* s-b-c: ">o(s,b,c) = 30<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* Rozwiązanie s-a ma mniejsze ograniczenie niż najmniejszy uzyskany koszt, usuwam go z _Z_ i szukam jego potomków: 
	* s-a-c: ">o(s,a,c) = 22+23 = 45<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* Odrzucam to rozwiążanie, bo ma ograniczenie większe od najmniejszego uzyskanego kosztu (43), a więc nie warto go rozwijać. 

* Biorę kolejne rozwiązanie z _Z_, usuwam z _Z_ i szukam jego potomnków: 
	* s-b-c-t: ">o(s,b,c) = 10 + 20 + 12= 42<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* Znaleziono mniejsze rozwiązanie: 42

* Stop: zbiór _Z_ jest pusty. Rozwiązanie: s-b-c-t.

### Problem plecakowy

Problem: mamy zbiór przedmiotów _P_. Każdy z nich opisany jest wartością i rozmiarem. Musimy wybrać tyle przedmiotów, by suma ich rozmiarów nie przekroczyła rozmiaru plecaka, i aby ich wartość była największa. 

Obierzmy zbiór przedmiotów ">P = \{ (\text{wartosc}, \text{rozmiar}), A(3,7), B(2,5), c(1, 1), D(5,2) \}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=. 

Rozmiar plecaka: ">L = 8<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Definiujemy ograniczenie ">o(A+) = \frac{3}{7}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- wartość:  3, zajęte miejsce: 7 

...



# Laboratorium 3

przykłady zadań w języku gnu math prog

zad 1

partition

na wejściu zbiór liczb Z sumujący się do parzystej, np. 

Z = {2, 4, 5, 1, 6}

zadanie: czy z tego zbioru wybrać liczby sumującej się do k">\sum_{i = 1}^n z_i = 2k<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=niech k = 9

1 krok - ustalić zmienne

pytanie dot. podzbioru liczb - tworzymy drugi zbiór x_i taki, że x_i \in {0,1}
0 oznacza, że liczba z_i należy do rozwiązania

suma wybranych = k
suma niewybranych też = k, skoro suma wybranych = 2k

wybieranie liczb można przedstawić tak: 

suma wybranych ma się równać sumie niewybranych):
2x_1 + 4x_2 + 5x_3 + 1x_4 + 6x_5 = 
2(1-x_1) + 4(1-x_2) + 5(1-x_3) + 1(1-x_4) + 6(1-x_5)

i model gotowy (programowanie zero-jedynkowe)

kod:

plik: plecak.mod;

param n >=1, integer; //ile liczb
param wartosci {1..n} >= 0, integer; 
var x {1..n}, binary; //szukane

s.t. ogr1: sum{i in 1..n} wart[i] * x[i] == sum{i in 1..n} wart[i] * (1-x[i]); //tylko zmienna * stała

//cel nie potrzebny, bo pytamy, cyz jest podzbiór
solve;
display x;
end;

plik: plecak.dat

param n := 5;
param wart := 1 2 2 4 3 5 4 1 5 6;
end;



------
zad 1 
graf skierowany o n wierzchołkach

0 > 1
1 > 4
0 > 2
3 > 0
2 > 3

największy podzbiór wierzchołków takich, że
- nie są połączone
- i jeśli wybierzemy jakiś, to musi się łączyć z innym niewybranym

z wierzchołkami kojarzymy zmienne
xi = {0, 1} (1 wybrane, 0 niewybrane)

x_0 - wierzchołek 0
x_1 - wierzchołek 1
itd.

generalnie mam n wierzchołków od 0 do n-1

ogr. żadna para wierzchołków nie może być polączony krawędzią

krawędź
x_0 + x_1 <= 1

krawędź
x_1 + x_4 <= 1
x_0 + x_2 <= 1
x_0 + x_3 <= 1
x_2 + x_3 <= 1

drugie ograniczenie
jeśli nie wybiorę wierzchołku, to musi się on łączyć z jakimś wybranym
dla x_0: x_1 + x_2 >= (1 - x_0)
jeśli x_0 nie został wybrany, to musi istnieć przynajmniej 1 krawędź z rozwiązania
dla x_1: x4 >= (1-x_1)
dla x_2: x_3 >= (1-x_2)
dla x_3: x_0 >= (1-x_3)

ogr trzecie: 
x_4 = 1 // wszystkie wierzchołki izolowane wchodzą do rozwiązania

kod:
param n, integer, >= 1; liczba grafów
set V := 0..(n-1); //zbiór wierzchołków
set E within V cross V; //zbiór krawędzi to iloczyn kartezjański
param outdegree {i in V} := sum{(j,k) in E: i == j} 1;//krawędzie wychodzące z danego wierzchołka; i==j - to daje krawędzie wychodzące z wierzchołka i

//zmienne
var x {V}, binary; //wierzchołki

//ograniczenia 
//no connection
s.t. no_connection{(i,j) in E}: x[i] + x[j] <= 1;

//has connection
s.t. has_connection{i in V: outdegree[i] >= 1}: sum{(j,k) in E: i == j} x[k] >= 1 - x[i]; //outdegree[i] >= 1 bo mają być nieizolowane

//isolated - musimy ustalić, czy ilozowany wchodzi do rozwiazania
s.t. isolated{i in V: outdegree[i] == 0} x[i] == 1;

//jeśli chcemy, żeby liczba wierzchołków była największa:
maximize size: sum{i in V} x[i];

solve;
display x;
end;

plik z danymi: 
param n:= 20;
set E := (1,2) (1,5) (1,10); //wierzchołek początkowy, końcowy 
end;

ibm cplex
gurodi
- te solvery mogłoby szybciej znaleźć rozwiązanie

cbc
- ten solver jest gorszy
- 

-----

# Wykład 4 | 28.11.2020 | Programowanie dynamiczne

Stosowane w przypadku problemów klasy _p_ -- rozwiązywanych w czasie wielomianowym. 

## Ogólny algorytm programowania dynamicznego

Nie ma precyzyjnego algorytmu jak w innych metoda: programowanie dynamiczne jest raczej ogólną ideą. 

1. Sformułuj zadanie jako równanie rekurencyjne zależne od zadań mniejszych (jednego lub kilku). 

-- Żeby rozwiązać problem, rozwiązujemy zwykle zadania dla mniejszych danych i scalamy wyniki czastkowe. 

-- Istotne jest zauważenie możliwości podziału zadania na mniejsze elementy i zależności między nimi. Idealnie, gdy te zależnośc można zapisać w postaci równania rekurencyjnego. 

2. Zaimplementuj wymyśloną funkcję tak, by nie powtarzać obliczeń dla tych samych parametrów. 

-- W tym celu stosuje się zwykle tablice przechowujące wyniki dla cząstkowe i żeby nie ponawiać raz wykonanych obliczeń. 

3. Odczytaj rozwiązanie w właściwej komórki tablicy lub odpowiednio je wylicz. 

## Przykład 1: maksymalna suma spójnego podciągu

Na wejściu tablica liczb całkowitych: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a = [1, 2, -2, -2, 4, -1, 5, 2, -3]">

Cel: znaleźć maksymalną sumę elementów spójnego (bez przerw) podciągu. 

Rozwiązanie: 10 (suma liczb od 4. do 7.; liczby w tablicy indeksowane od 0)

Uwaga: nie bierzemy pod uwagę sum podciągów mniejszych od zera: w takich przypadkach rozwiązanie jest trywialne: bierzemy zerowy podciąg (bez elementów), gdyż ich suma jest równa 0, co jest większe od wszelkiej ujemnej sumy podciągów. 

Rozwiązanie metodą programowania dynamicznego: 

* znajdź powtarzający się schemat między zadaniem większym a mniejszym: 
* definiujemy funkcję ">s(j)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= zwracającą sumę spójnego ciągu od elementu ">0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= do ">j<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=	* jeśli ">j=0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to ">s(j)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= ma wartość ">0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= lub pierwszy element ciągu (jeśli jest dodatni)
	* jeśli ">j>0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to ">s(j)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= ma wartość ">0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= lub suma elementu ">j<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=-tego (">s(j)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=) i sumy wszystkich poprzednich elementów: ">s(j-1)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=s(j) = \begin{cases} \max(a_0, 0) & j = 0 \\ \max(a_j + s(j-1)) & j>0 \end{cases} ">

* wypełniamy pomocniczą tabelę wartościami ">s(j)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= dla każdego ">j \in [0, n]<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (">n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= to liczba elementów w ciągu: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=s = [1, 3, 1, 0, 4, 3, 8, 10, 7]">

* wybieramy największą wartość, czyli 10 

## Przykład 2: liczba jako suma malejących liczb dodatnich dających największy iloczyn 

Przedstawić podaną liczbę całkowitą ">n>0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jako sumę malejących liczb całkowitych dodatnich, których iloczyn jest największy np.
  
* ">6 = 4+2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (ale nie ">6 = 3+2+1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, bo ">4\cdot 2 > 3\cdot 2 \cdot 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=)
* ">10 = 5+3+2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Rozwiązanie

* definiujemy funkcję rekurencyjną ">m(n,k)<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jako największy iloczyn ze zbioru ">\{1, 2, \dots, k\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, gdzie ">0 \leq k \leq n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=m(n,k) = \begin{cases} 
1 & \text{jeśli}\ n = 0, \\
0 & \text{jeśli}\ n < 0 lub \frac{(1+k)k}{2} < n, \\
\max\{(k \cdot m(n-k, k-1), m(n,k-1)\} & \text{w przeciwnym razie}
\end{cases}">

gdzie:
* ">m<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= to największy iloczyn; 
* ">n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= to liczba, do których mają się sumować znalezione liczby; 
* ">k<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= to granica zbioru, z którego pochodzą liczby sumujące się do ">n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= i dające największy iloczyn. 

Jedynka jako wartość funkcji jest niezbędna, żeby móc zakończyć rekurencyjne mnożenie (mnożenie przez 1 jest neutralne -- nie zmienia wartości). 

Wartość ">0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= oznacza, że albo ">n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest ujemne (wówczas nie da się znaleźć największego iloczynu: mnożenie liczb będzie dawało coraz mniejszą liczbę), albo podzbiór liczb ">\{1, 2, \dots, k\} nie sumuje się do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n">, ale do jakiejś wartości mniejszej od <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n">, co można przedstawić jako sumę pierwszych <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n"> wyrazów ciągu arytmetycznego (suma wyrazów pierwszego i ostatniego pomnożona przez liczbę wszystkich wyrazów i podzielona przez 2). 

W zasadniczej funkcji rekurencyjnej (3. przypadek) rozważamy 2 przypadki: 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=k"> jest uwzględnione w rozwiązaniu: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=k"> razy maksymalny iloczyn liczb od <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1"> do mniejszej o 1 od <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=k"> i tym samym sumujący się nie do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n">, ale do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n-k">, bo <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=k"> już wyodrębniliśy (tu <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n-k"> wchodzi w miejsce parametru <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n"> i może się pojawić sytuacja, że <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n=0"> lub <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n<0">);
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=k"> nie jest uwzględnione w rozwiązaniu: analizujemy ciąg liczb od <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=1"> do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=k-1"> (skoro nie bierzemy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=k"> pod uwagę) i sumujący się do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n">. 

-- i bierzemy pod uwagę większy iloczyn (z <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=k"> lub bez <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=k">). 

Przykładowy zapis w języku ``C#``: 

<iframe width="100%" height="475" src="https://dotnetfiddle.net/Widget/QM05Cs" frameborder="0"></iframe>

Interpretacja wyników: bierzemy pod uwagę tylko te indeksy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=j"> tablicy, przy których zmniejsza się maksymalna suma: 

Maksymalna suma: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=622\ 702\ 080">

Składniki: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=80 = 13+12+11+9+8+7+6+5+4+3+2">

Przykład dla <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n=5">: 

<iframe width="100%" height="475" src="https://dotnetfiddle.net/Widget/UqQ3Mc" frameborder="0"></iframe>

```
i: 1, j: 1, tab: 1  
i: 2, j: 2, tab: 2  -- bierzemy 2
i: 5, j: 3, tab: 6  -- bierzemy 3
i: 5, j: 4, tab: 6  
i: 5, j: 5, tab: 6
```

Maksymalna suma: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=6">

Składniki: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=5 = 3 + 2">

## Przykład 3: znajdowanie najkrótszej drogi

Na wejściu mamy graf skierowany. Każdej krawędzi tego grafu przyporządkowano liczbę całkowitą większą od zera. 

![](https://www.evernote.com/shard/s443/res/409ac6bb-6fe5-08af-7191-ff119f25a163)

Zadanie: wyznaczyć długość najkrótszej drogi między wierzcholkami *s* i *t*. 

Przyjmujemy oznaczenia: 

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=d(i, j, 0)"> -- długość najkrótszej drogi z wierzchołka <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=i"> do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=j">; trzeci parametr oznacza liczność zbioru wierzchołków wziętych do rozwiązania (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=0"> oznacza brak wierzchołków pośrednich)

Zależność rekurencyjna: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=d(i, j, k+1) = \min(d(i,j,k), d(i,k+1,k) + d(k+1,j,k))">

-- najkrótsza droga z wierzchołka <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=i"> do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=j"> licząca <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=k+1"> wierzchołków to mniejsza droga z 2 możliwości: 
 
* rozwiązanie bez wierzchołka <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=k+1"> o długości <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=d(i,j,k)">
* rozwiązanie z wierzchołkiem <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=k+1"> o długości równej sumie odległości:
	* z <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=i"> do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=k+1">: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=d(i,k+1,k)">
	* z <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=k+1"> do <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=j">: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=d(k+1,j,k)">

Tak sformułowana zależność pozwala odpowiedzieć na pytanie, czy do rozwiązania bierzemy wierzchołek <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=k+1">: analizujemy warianty bez wierzchołka <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=k+1"> i z tym wierzchołkiem. 

Rozwiązanie w ``C#``:

<iframe width="100%" height="475" src="https://dotnetfiddle.net/Widget/KutuNL" frameborder="0"></iframe>

# Wykład 5 | 5.12.2020 | Answer Set Programming (1)

Możliwe polskie tłumaczenie ang. _answer set programming_ -- "abdukcyjne programowanie logiczne": "abdukcyjne" -- na podstawie wyników staramy się znaleźć przesłanki, jakie doprowadziły do wyników. 

## Podejścia do programowania

* imperatywne:
	* określamy dokładne algorytm i struktury danych
	* program przebiega od danych wejściowych do wyniku
	* programy są ogólnego przeznaczenia 
	* testowanie: łatwe 
* deklaratywne:
	* określa się fakty i reguły zamiast algorytmu lub ciągów instrukcji
	* fakty reprezentują naszą wiedzę o problemie
	* testowanie: utrudnione (nie da się debugować, testowanie przez zastosowanie różnych zestawów danych)
	* np. 
		* język MathProg (fakty: parametry i zbiory, reguły: ograniczenia)
		* answer set programming (fakty i reguły logiczne)  

### Przykładowe zadanie

Dana jest tablica liczb całkowitych. 

Zadanie: podzielić tablicę na dwie podtablice w taki sposób, by suma elementów w jednej była równa sumie elementów w drugiej. 

Przykład: 

| Wejście | Wyjście |
|-|-|
| <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=[4,5,-2,1,1,5]"> | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=[4,5,-2], [1,1,5]"> |

### Rozwiązanie w języku ``Go`` (programowanie deklaratywne)

```go
package main

import "fmt"

func sum(tab []int) (result int) {
	for _, v := range tab {
		result += v
	}
	return
}

func main() {
	a := []int{4, 5, -2, 1, 1, 5}
	whole, part := sum(a), a[0]
	if whole % 2 == 0 {
		for i := 1; i < len(a); i++ {
			if part == whole /2 {
				fmt.Println(a[:i], a[i:])
				break
			}
			part += a[i]
		}
	}
}
```

### Rozwiązanie w języku ``Prolog`` (programowanie deklaratywne)

```prolog
split(Tab, Al, Ar) :-
	append(Al, Ar, Tab),
	sum_list(Al, X),
	sum_list(Ar, Y),
	X =:=

main :- split([4,5,-2,1,15], A, B), write(A), write(B), nl.
```

## Answer Set Programming -- definicje

* program to zbiór ==reguł normalnych==.
* ogólna postać reguły normalnej: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a \leftarrow b_1, \dots, b_m, \neg c_1, \dots, \neg c_n.">

--- gdzie: 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> -- głowa reguły: wniosek, konkluzja
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b_1, \dots, b_m, \neg c_1, \dots, \neg c_n"> -- ciało reguły: ciąg tzw. ==atomów== -- niepowtarzalnych identyfikatorów warunków prowadzących do konkluzji 
* tradycyjnie atomy zanegowane <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\neg c_k"> zapisuje się na końcu reguły
* przecinki to logiczne "i"
* reguła bez ciała (z pustym ciałem) zwana jest ==faktem== oznacza coś niezmiennego, stałego i zapisywana jest dwojako

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a \leftarrow . \\
a.">

* reguła bez głowy (z pustą głową) zwana jest ==ograniczeniem== i jest rzadko spotykana: można ją zastąpić regułą z głową
* program możeć stałe i zmienne
* zmienne zapisuje się wielkimi literami lub nazwami zaczynającymi się od wielkich liter, np. <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=X">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Y">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Z">
* pod zmienne podstawia się stałe
* zmienne pojawiają się w predykatach -- wyrażaniach zwracające wartość boolowską (prawda, fałsz), np. <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=p"> w <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=p(X)"> 
* predykaty zapisuje się małymi literami
* wielokrotne użycie tego samego identyfikatora zmiennej w tej samej regule(!) oznacza, że po podstawieniu stałych w tych miejscach pojawią się te same wartości, np. ta sama stała wystąpi 3 razy w regule: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=p(X) \leftarrow q(X), \neg s(X).">

* stałe zapisuje się małymi literami, np. 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=p(a) \leftarrow q(a), \neg s(a). \\
p(b) \leftarrow q(b), \neg s(b). \\
p(c) \leftarrow q(c), \neg s(c).">

* predykat ze zmienną lub stałą tworzy atom, np. <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=p(X)">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\neg p(a)">
* zmienną <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=X"> w atomie niezanegowanym (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=p(X)">) czyta się: "wybrano _X_"
* zmienną <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=X"> w atomie zanegowanym (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\neg p(X)">) czyta się: "nie wybrano _X_"
* program bez zmiennych nazywany jest programem ==zakotwiczonym== (solwery działają tylko na zakotwiczonych programach)
* programy zakotwiczone powstają przez podstawienie wszystkich (danych w zadaniu) stałych pod zmienne

## Model Stabilny (Answer Set)

Stabilny model (odpowiedź, rozwiązanie) <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=M"> dla zakotwiczonego (bez zmiennych, tylko samymi stałymi)  programu <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=P"> to zbiór zakotwiczonych atomów, dla których: 

* każda reguła jest spełniona: 
	* tzn. dla każdego reguły <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=P"> postaci <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \leftarrow b_1, \dots, b_m, \neg c_1, \dots, \neg c_n."> 
	* jeśli każde <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b_j \in M"> -- należą do modelu [rozwiązania], 
	* oraz jeśli każde <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c_k \notin M"> -- nie należą do modemu [rozwiązania])
	* to <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> musi należeń do modelu <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=M">

Słownie: 
* jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b_1"> jest w rozwiązaniu oraz <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b_2"> jest w rozwiązaniu... oraz <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b_m"> jest w rozwiązaniu 
* oraz jeśli <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c_1"> NIE jest w rozwiążaniu oraz <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c_2"> NIE jest w rozwiązaniu... oraz <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c_k"> NIE  jest w rozwiązaniu
* to <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> jest w rozwiązaniu

Jeśli wszystkie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b_j"> są w <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=M"> i żadnego <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c_k"> nie ma w <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=M">, a <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> też nie jest w <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=M">, to taki model <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=M"> nie jest stabilny. 

Każdy atom <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \in M"> (należący do modelu [rozwiązania]) mysi być wyprowadzalny z jakiejś reguły -- musi wynikać z jakiejś reguły (wykluczamy błędne koło we wnioskowaniu).

## Przykłady

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=P_1 = \{ a \leftarrow a.\}">

-- z <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> wynika <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a">

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=M = \{a\}"> nie jest stabilnym modelem (chociaż <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=M = \emptyset"> jest stabilnym modelem) -- przykład błędnego koła: nic nie mówi, że <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> musi być. 

---

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=P_2 = \{a \leftarrow \neg b. \}">

-- czytaj: jeśli w odpowiedzi (<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\{ a\}">) nie ma <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b">, to <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> należy do odpowiedzi. Zgadza się: w odpowiedzi nie ma <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b">, a więc <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\{a\}"> jest jedynym stabilnym modelem: każdy podzbiór atomów (pusty, jednoelementowy z samym <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a">, samym <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b"> i dwuelementowy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> i <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b">). 

---

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=P_3 = \{a \leftarrow \neg a. \}">

-- program nie ma stabilnego modelu, skoro jest tylko jeden atom <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a">. Możliwe odpowiedzi: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\{ \emptyset \}"> lub  <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a">, ale <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\emptyset"> nie wejdzie do modelu, bo nie jest wyprowadzalne, poza tym z reguły <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=P_3"> wynika, że do modelu ma wejść <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a">.  Do modelu też nie wejdzie <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a">, bo warunkiem wejścia <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> do modelu jest brak <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> w modelu -- sprzeczność.  

---

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=P_4 = \{a \leftarrow \neg b. b \leftarrow \neg a. \}">

Program z dwiema regułami. Ma 2 stabilne modele: 

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\{a\}"> -- jeśli w odpowiedzi nie ma <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b">, to jest <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> -- zgadza się: do modelu dodano <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\{b\}"> -- jeśli w odpowiedzi nie ma <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a">, to jest w nim <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b">. 

---

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=P_5 = \{ a \leftarrow \neg b. b \leftarrow \neg a. a \leftarrow \neg a. \}">

-- <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\{a\}"> jest jedynym stabilnym modelem 
jeśli a w modelu to b nie ma w modelu (ok), a jest wyprowadzlane (ok) 

## Przykłady w języku ``ansprolog`` (w ``Clingo``)

```
lata(X) :- ptak(X), not nielot(X).
kiedy coś lata: gdy jest ptakiem i nie jest nielotem
nielot(X) :- pingwin(X).
kto jest nielotem - pingwin
ptak(X) :- pingwin(X).
a kto jest ptakiem - pingwin
ptak(antek).
```

Zapis ``:-`` jest odpowiednikiem <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\leftarrow">. 

Zmienne: ``X``

Stałe: ``antek`` 

Konkluzja: ``antek`` lata, bo jest stabilnym modelem: jest ``ptak(antek)``, ``lata(antek)``

Jeśli zamienimy fakt ``pingwin(antek)``, wtedy stabilny  model zawiera ``nielot(antek)``. 

## Więzy (ograniczenia)

Więzy (inaczej ograniczenia) to  reguły bez głowy (z pustą głową), np.  

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\leftarrow b_1, \dots, b_m, \neg c_1, \dots, \neg c_n.">

Słownie: nie może być tak, że jest <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b_1">, jest <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b_2"> itd., i nie ma <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c_1">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c_2"> itd. 

Więzy służą zabronieniu czegoś, wskazujż, że żaden stabilny model nie może zawierać wszystkich atomów <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b_j"> i jednocześnie nie zawierać żadnego <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c_k">

To odpowiedniki równań i nierówności w programowaniu całkowitoliczbowym. 

Więzy można zastąpić regułami z głową: wystarczy przed strzałką wstawić atom, którego nigdzie indziej nie użyto. 

# Laboratorium 5 | 6.12.2020

## Zadanie 6.

Ze bioru: https://gitlab.com/wojtek3dan/zadania-to/-/blob/master/zadania.md

Rozważmy pewną jednoosobową grę, w której rekwizytami są liczby całkowite ułożone w ciągu. W każdym kroku wybieramy dowolną liczbę oprócz dwóch skrajnych i usuwamy ją z ciągu. Zdobywamy za to tyle punktów ile wynosi suma wybranej do usunięcia liczby i jej dwóch przyległych sąsiadów. Gra kończy się, gdy w ciągu zostają dwie liczby. Naszym celem jest maksymalizacja zdobytych punktów. Oczywiście punkty zdobyte w kolejnych krokach sumują się. Na przykład, dla ciągu 2, 1, 5, 3, 4 możemy uzyskać maksymalnie 31 punktów w następujący sposób: usuwamy 3 (12 pkt) -> 2, 1, 5, 4; usuwamy 1 (8 pkt) -> 2, 5, 4; usuwamy 5 (11 pkt) -> 2, 4. Suma = 12 + 8 + 11 = 31.

Napisz program wyznaczający maksymalną możliwą do uzyskania sumę punktów. Zakładamy, że długość wejściowego ciągu nie przekroczy 200, a każdy jego element będzie zawierał się w przedziale [1, 100]. Limit czasowy = 10 sekund.

--------

## Zadanie 3 

Ze zbioru https://gitlab.com/wojtek3dan/zadania-to/-/blob/master/zadania.md

Do oddania do 14.12.2020 

Tablica <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> zawiera liczby całkowite z zakresu od 1 do 50000 
uporządkowane niemalejąco, tzn. _a_[0]≤_a_[1]≤⋯≤_a_[_n_ − 1]. 
Znajdź najmniejszą dodatnią liczbę całkowitą, 
której nie da się przedstawić jako sumę elementów wybranych 
z tablicy _a_ (żaden element z tej tablicy nie może być 
użyty więcej niż raz). Na przykład, jeśli _a_ = [1, 1, 2, 9], 
to taką najmniejszą liczbą będzie 5. 
Zakładamy, że _n_ może wynosić 105. 
Limit czasowy = 10 sekund.

wejście tak samo jak w poprzednim: 
* wpisujemy liczbę liczb
* wpisujemy liczby
* po ostatniej program wykonuje obliczenia

# Wykład 6 | 12.12.2020 | Metoda generuj-ograniczaj 

## Zmienna pomocnicza <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a'">

W tej metodzie wprowadza się atom pomocniczy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a'">, dzięki czemu można zaznaczyć w programie, że inny atom <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> może należeć do rozwiązania, ale nie musi: 

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> musi należeć do rozwiązania, gdy nie ma <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a'">: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \leftarrow \neg a'.">
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> nie może należeć do rozwiązania (żeby <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a'"> mogło): <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a' \leftarrow \neg a.">

Daje nam to 2 stabilne modele 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\{a\}, \{a'\}">

-- ten drugi reprezentuje odpowiedź, że atomu <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> nie ma w rozwiązaniu.

W tej metodzie dochodzimy do sytuacji, w którym atom jest wybrany lub nie jest wybrany, co można zapisać regułami jak wyżej.

Pozwala to uzyskać tyle stabilnych modeli, ile jest zmiennych, plus model ze zbiorem pustym, np. dla zbioru stałych <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\{a, b, c\}"> możemy zapisać reguły: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a \leftarrow \neg a'. \ \ \ \ \ \ b \leftarrow \neg b'. \ \ \ \ \ \ c \leftarrow \neg c'.">
<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=a' \leftarrow \neg a. \ \ \ \ \ \ b' \leftarrow \neg b. \ \ \ \ \ \ c' \leftarrow \neg c.">

## Zapis dodatkowych warunków

### Dowolny podzbiór zbioru <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\{a, b, c\}"> taki, że <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a"> i <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b"> nie występują jednocześnie

Zapis: 

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a \leftarrow \neg a'.\ \ \ \ \ \  b \leftarrow \neg b'. \ \ \ \ \ \  c \leftarrow \neg c'.">
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a' \leftarrow \neg a.\ \ \ \ \ \  b' \leftarrow \neg b. \ \ \ \ \ \  c' \leftarrow \neg c.">
<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\leftarrow a, b.<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=### Jeśli ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to ">b<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Inaczej, jeśli ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest w stabilnym modelu, to ">b<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= też musi być w modelu:">b \leftarrow a.<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=## Przykład 1: Cykl Hamiltona w grafie

W grafie nieskierowanym wskazać **cykl Hamiltona** (cykl, w którym każdy wierzchołek odwiedzany jest tylko 1 raz, za wyjątkiem pierwszego wierzchołka).

Rozwiązanie: 

* patrzymy na cykl Hamiltona nie jak na zbiór wierzchołków, tylko zbiór krawędzi: koniec jednej krawędzi musi być początkiem drugiej
* krawędź oznaczymy predykatem: 

``krawedz(U, V)``

* dowolna krawędź może należeć do tego cyklu, co oznaczymy predykatem: 

``wybrana(U, V)``
 
* wybranie krawędzi do rozwiązania: 

``wybrana(U, V) :- krawedz(U, V), not odrzucona(U, V).``

-- parę wierzchołków ">U<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, ">V<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= można dodać do rozwiązania, jeśli tworzą krawędź, która nie jest odrzucona (**generowanie krawędzi w rozwiązaniu**)

* odwrotność wybrania -- odrzucenie krawędzi (nienależenie do rozwiązania) (**generowanie krawędzi w rozwiązaniu**): 

``odrzucona(U, V) :- krawedz(U, V), not wybrana(U, V).``

-- parę wierzchołków można odrzucić, jeśli tworzą krawędź, która nie jest wybrana 

* powyższe reguły generują wszystkie możliwe podzbiory krawędzi

* zmienne oznaczające wierzchołki: ">U<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, ">V<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* krawędzie w cyklu muszą tworzyć ścieżkę, czyli ciąg połączonych wierzchołków, co oznaczymy regułami (**generowanie wierzchołków osiągalnych**) 

```
osiagalny(V) :- wybrana(v0, V).
osiagalny(V) :- osiagalny(U), wybrana(U, V).
```

-- gdzie ``v0`` oznacza wierzchołek początkowy; pierwsza reguła oznacza możliwość przejścia z wierzchołka ``v0`` do dowolnego ``V``, a druga, przejście z ``U`` do ``V``, co jednocześnie oznacza przejście z ``v0`` do dowolnego wierzchołka ``V``

* z każdego jednego wierzchołka można przejść tylko do jednego innego wierzchołka, co możemy wskazać więzem (**ograniczenie 1.**): 

```
:- wybrana(U, V), wybrana(W, V), U != W.
:- wybrana(U, V), wybrana(U, W), V != W.
```

-- nie może być tak, że jakieś 2 krawędzie wybrane do rozwiązania wchodzą do tego samego wierzchołka ``V``

* ograniczenie zapewniające osiągalność każdego wierzchołka (**ograniczenie 2.**): 

```
:- wierzcholek(U), not osiagalny(U).
```

-- nie może być tak, że ``U`` jest wierzchołkiem i nie jest osiągalny (nie można do niego dojść z wierzchołka początkowego lub innego osiągalnego wierzchołka) (**ograniczenie 3.**)

Przykładowe fakty: 

```
wierzcholek(v0).
wierzcholek(v1).
wierzcholek(v2).
krawedz(v0, v1).
krawedz(v1, v0).
krawedz(v1, v2).
krawedz(v2, v0).
```

## Przykład 2: Kolorowanie grafu przy użyciu 3 kolorów

Pytanie: czy 3 kolorami można pokolorować mapę. Każde państwo może być pokolorowane tylko 1 kolorem. Mapa reprezentowana jest przez zbiór państw i ich granicze: 

Rozwiązanie: 

* za mapę przyjmujemy zbiór państw i ich granice, np. 

```
panstwo(a).
panstwo(b).
```

* państwa sąsiadujące: 

```
sasiedzi(a, b).
```

* kolory: 

```
paleta(czerwony).
paleta(niebieski).
paleta(zolty).
```

* reguły potrzebne do sprawdzenia kolorowania mapy: każde państwo zostanie pokolorowane tylko 1 kolorem (**generowanie kolorów**)

```
kolor(V,K) :- panstwo(V), paleta(K), not innyKolor(V,K).
```

-- państwo ``V`` może być pokolorowane ``K``, jeśli ``K`` jest kolorem (``paleta(k)``), ``V`` jest państwem (``panstwo(V)``) i nie jest pokolorowane innym kolorem (``not innyKolor(V, K)``

* każde państwo musi być pokolorowane (**generowanie innych kolorów** i **generowanie pokolorowanych państw**): 

```
innyKolor(V, K) :- panstwo(V), paleta(K), not kolor(V, K).
maKolor(V) :- panstwo(V), paleta(K), kolor(V, K).
```

-- państwo ``V`` może być pokolorowane kolorem ``K``, jeśli ``V`` jest państwem (``panstwo(V)``), ``K`` jest kolorem (``paleta(K)``) i państwo ``V`` nie jest pokolorowane innym kolorem (**ograniczenie 1.**):

```
:- panstwo(V), not maKolor(V).
```

-- wykluczone jest, że ``V`` jest państwem i nie ma koloru  

* każde państwo musi mieć tylko 1 kolor (**ograniczenie 2.**): 

```
:- panstwo(V), paleta(K1), paleta(K2), kolor(V, K1), kolor(V, K2), K1 != K2.
```

-- wykluczone jest, że państwo ``V`` ma kolor ``K1`` i jednocześnie inny kolor ``K2``

* sąsiadujące państwa nie mogą mieć tego samego koloru (**ograniczenie 3.**): 

```
:- sasiedzi(V, U), kolor(V, K), kolor(U, K).
```

-- dwa państwa, które są sąsiadami, nie mogą mieć tego samego koloru ``K``

Fakty: 

```
panstwo(a).
panstwo(b).
sasiedzi(a, b).
paleta(czerwony).
paleta(niebieski).
paleta(zolty).
```
## Grounding

Przed wykonaniem zadania wykonuje się tzw. **grounding** -- podstawienie pod zmienne wszystkie możliwe stałe.

## Formalna definicja stabilnego modelu

Niech ">P<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= będzie zakotwiczonym programem (bez zmiennych), a ">M<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= podzbiorem jego atomów.

==**Reduktem**== programu ">P<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= ze wzgledu na ">M<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= nazywamy: ">P^M = \{h \leftarrow b_1, \dots, b_m | h \leftarrow b_1, \dots, b_m, \neg c_1, \dots, \neg c_n \in P \wedge \{ c_1, \dots, c_n \} \cap M = \emptyset \} <img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=-- bierzemy wszystkie reguły i odcinamy reguły zanegowane ">c<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, które nie wchodzą do modelu ">M<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=">M<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest stabilnym modelem dla ">P<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= wtedy i tylko wtedy, gdy ==**atomowymi konkluzjami reduktu**== jest dokladnie zbiór ">M<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=**Atomowe konkuzje reduktu** -- głowy reguł, których wszystkie przesłanki zawarte w ciele (predykaty) są spełnione. 

Jeśli tak uzyskany podzbiór atomów (atomowych konkluzji reduktur) jest równy ">M<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to ">M<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest stabilnym modelem. 

### Przyklad 1 ">P = \{ a \leftarrow \neg b. \ \ \ \ \ \ b \leftarrow \neg a. \}<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=-- jeśli nie zostało wybrane ">b<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to musi być wybrane ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=; 
-- jeśli nie zostało wybrane ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, musi być wybrane ">b<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Sprawdzenie dla modelu ">M = \{ a \}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=: 

* patrzymy na każdą regułę:
* jeśli nie wybrano ">b<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to wybrano ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- zgadza się, w modelu jest ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= i nie ma ">b<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- głowę reguły ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= wrzucamy do rozwiązania, mamy pierwszą atomową konkluzję reduktu 
* jeśli nie wybrano ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=... ale ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= wybrano, więc regułę pomijamy 

Zatem odpowiedź: ">M = \{a\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest stabilnym modelem, bo ">P^M = \{a \leftarrow .\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, a jego atomowe klonkluzje to dokladnie zbior ">M<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=.

### Przykład 3

Pytanie: dlaczego ">a \leftarrow \neg a.<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= nie ma stabilnego modelu? 

W regule jest tylko jeden atom, więc rozważać możemy 2 rozwiązania: 
* ">M = \{ a \}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 
* ">M = \{ \emptyset \}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 

-- Zbior  pusty nie jest stabilnym modelem, bo nie zawiera ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, a zgodnie z regułą powinien: 

* analizowane rozwiązanie: ">M = \{ \emptyset \}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=*  atomowe konkluzje reduktu: ">P^M = \{ a \leftarrow .\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* ">M \neq P^M<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, więc ">\{ \emptyset \}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= nie jest rozwiązaniem

-- Zbiór ">\{ a \}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= nie jest stabilnym, modelem, bo: 

* analizowane rozwiązanie: ">M = \{ a \}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 
* redukt: ">\{ \emptyset \}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, bo nie ma niezanegowanych reguł wchodzących do modelu (jest tylko zanegowana ">\neg a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=)
* atomowe konkluzje reduktu (głowy reguł): ">P^M = \{ \emptyset \}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=* ">M \neq P^M<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, bo ">\{ a \} \neq \{ \emptyset \}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, więc reguła nie ma stabilnego modelu. 

# Laboratorium 6 | 13.12.2020 | Niestandardowe konstrukcje w ``Clingo`` 

## Określona liczba elementów 

-- Nie mniej niż ">L<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= i nie więcej niż ">U<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=:">L \{ a_1; \dots; a_m; \neg b_1; \dots; \neg b_k \} U<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=### Przykład 1: ``0 { a; b; not d} 2.`` 

```
0 { a; b; not d} 2.
```
-- wybieramy zbiory 0-elementowe, 1-elementowe (`a`, `b` lub `c`) lub 2-elementowe. 

Ograniczenie może być z lewej, z prawej, albo z obu stron. 

Więzy te mogą być użyte w dowolnym miejscu reguły.

``{a}`` jest stabilnym modelem

``{a, b}`` nie jest stabilnym modelem, bo już ``{a}`` oznacza wybranie 2 elementów: wybranie ``a`` i niewybranie ``d``

### Przykład 2: generowanie wszystkich podzbiorów ">\{ a, b, c, d \}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= takich, że ">a \rightarrow b<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Wygenerować wszystkie podzbiory ">\{a, b, c, d\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= w taki sposób, by wybranie ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= pociągało za sobą wybranie ">b<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=.

Zapis w ``Clingo``:

```Clingo
0 {a; b; c; d} 4.
b :- a.
```

## Skrótowy zapis 4 faktów: ``p(1..4)``

``p(1..4).`` to inaczej: 

* ``p(1)``
* ``p(2)``
* ``p(3)``
* ``p(4)``

## Kolekcje, z których wybieramy ">n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= elementów

``{q(X, Y) : p(X)} = 2 :- p(Y).`` 

-- jeśli ">p(X) = \{ p(1), p(2), p(3), p(4) \}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, to z kolekcji

* ``q(1, 1)``
* ``q(2, 1)``
* ``q(3, 1)``
* ``q(4, 1)``
* ``q(1, 2)``
* ``q(2, 2)``
* ``q(3, 2)``
* ``q(4, 2)``
* ``q(1, 3)``
* ``q(2, 3)``
* ``q(3, 3)``
* ``q(4, 3)``
* ``q(1, 4)``
* ``q(2, 4)``
* ``q(3, 4)``
* ``q(4, 4)``

wybieramy 2 elementy. 

### Przykład: generowanie podzbiorów ">\{a, b, c, d\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= takich, że pominięcie ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= implikuje ">b<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Wygeneruj wszystkie podzbiory ">\{a, b, c, d\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, aby pominięcie ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= implikowało ">b<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=: 

``0 {a; b; c; d}.`` 

-- podzbiory od 0-elementowych, przez 1-elementowe, 2 itd. aż do 4, bo są tylko 4 elementy 

``b :- not a.``

-- pominięcie ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= implikuje ">b<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=.

Czy to są stabilne modele dla ww. programu? 

* ">M_1 = \{a, b, c\}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- tak: nie ma reguły mówiącej, że wybranie ">a<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= oznacza brak ">b<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=; jest reguła, że jeśli nie ma 4a">, to musi być ``b``

* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=M_2 = \{b, c, d, e\}"> -- nie: w programie nie ma <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=e">

## Wzajemne wykluczanie predykatów (graf Hamiltona)

W grafie Hamiltona dowolna krawędź może należeć do cyklu, ale jeśli należy, to nie jest odrzucona, a jeśli jest odrzucona, to nie należy do cyklu:  

``wybrana(U, V) :- krawedz(U, V), not odrzucona(U, V).``
``odrzucona(U, V) :- krawedz(U, V), not wybrana(U, V).``

W ``Clingo`` można zapisać to krócej: 

``0 { wybrana(U, V) : krawedz(U, V) }.``

-- po prawej mamy wszystkie możliwe krawędzie ``krawedz(U, V)`` które zasilają wybrane krawędzie

-- wybieramy od 0 do nieskończonej liczby krawędzi 


# Wykład 7 | 19.12.2020 | Answer Set Programming (2) -- przykłady

## Agregacje i optymalizacja

Niestandardowe konstrukcje. Umożliwjają umożliwiają otrzymywanie pojedynczej wartości ze zbioru danych. 

W ``Clingo`` zaimplementowano: 

* ``count`` (moc zbioru, liczność)
* ``sum`` (suma elementów zbioru)
* ``max`` i ``min`` (element maks. i minim.)
* ``maximize`` i ``mnimize`` (optymalizacja)

### Przykład 1

```
edge(a, b).
edge(b, c).
edge(c, a).

edge(X, Y) :- edge(Y, X).
vertex(X) :- edge(X, Y).
degreeOf(X, N) :- vertex(X), N = #count{X, Y : edge(X, Y)}.

#show degreeOf/2.
```

-- jeśli mamy ``edge(X, Y)``, to jednocześnie  ``edge(Y, X)`` (a więc graf jest nieskierowany)

-- wierzchołek ``X`` jest wtedy, gdy jest krawędź ``(X, Y)`` (wierzchołek staje się faktem) 

-- predykat ``degreeOf`` określa stopień wierzchołka: wierzcholek ``X`` ma stopien ``N`` pod warunkiem, że ``X jest ``vertex``, a ``N`` jest równe liczbie takich ``(X, Y)``, które mają ``edge(X, Y)``

-- dyrektywa ``show``: bez tego program pokazuje wszystkie atomy wchodzące do rozwiązania (cały stabilny model), co nie jest zawsze potrzebne, a dzięki ``show`` program wyświetla tylko ``degreeOf``

-- ``/2`` -- liczba argumentów danego predykatu

Wynik:

```
>clingo degree_count.lp
clingo version 5.4.0
Reading from degree_count.lp

Answer: 1
degreeOf(a, 2) degreeOf(b, 2) degreeOf(c, 2)
```

-- ``degree_count.lp`` -- plik tekstowy

### Przykład 2: sumowanie

```
val(a, 20).
val(b, 12).
val(c, 8).

{in(X)} :- val(X, N). 
:- #sum{N, X : in(X), val(X, N)} != 20. 

#show in/1. //pokaż tylko in z 1. parametrem
```

-- ``val(a, 20)``, ``val(b, 12)`` -- fakty: ``a`` ma wartość <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=20">, ``b`` -- <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=12"> itd.

-- ``{in(X)} :- val(X, N).`` -- jeśli mamy jakąś wartość przypisaną do ``X``, to albo bierzemy tę wartość do podzbioru, albo ją odrzucamy

-- ``:- #sum{N, X : in(X), val(X, N)} != 20.`` -- więzy: w rozwiązaniu (wśród wybranych ``in(X)``)  nie może być tak, że suma ``N`` (w przypadku krotek sumujemy pierwszy element krotki) jest różna od 20 (``!= 20``) 

-- czyli sprośród <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=a">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=b">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c"> wybierz taki podzbiór, których wartości zsumują się do 20

-- ``# show in/1.`` -- pokaż tylko wybrane (``in``)

Wynik

```
>clingo lata.lp -n 0
clingo version 5.4.0
Reading from lata.lp

Answer: 1
in(b) in(c)
Answer: 2
in(a)
```

### Przykład 3: ekstremum

```
val(a, 20).
val(b, 12).
val(c, 8).

{in(X)} :- val(X, N).
unwantedValue(M) :- M = #min{Y, X : val(X, Y)}. 
:- #sum{N, X: in(X), val(X, N)} != 20. 
:- val(X, N), unwantedValue(N), in(X). 

#show in/1.
```

-- ``val(a, 20)`` itd. -- fakty

-- ``{ in(X) } :- val( X, N).`` -- rozwiązanie (``in``) 

-- ``unwantedValue(M) :- M = #min{Y, X : val(X, Y)}.`` -- M to minimum z 

-- ``:- #sum{N, X: in(X), val(X, N)} != 20.`` -- jw.

-- ``:- val(X, N), unwantedValue(N), in(X).`` -- nie może być tak, że wybrano ``X``, mające przypisane ``N``, które jest jednocześnie ``unwantedValue``

Wynik

```
Answer: 1
in(a)
```

### Przykład 4: optymalizacja 

```
val(a, 20). 
val(b, 12).
val(c, 8). 

{in(X)} :- val(X, N). 
:- #sum{N, X : in(X), val(X, N)} > 30. 
#maximize{N, X : in(X), val(X, N)}. 

#show in/1.
```

-- fakty jw. 

-- ``{in(X)} :- val(X, N).`` -- jw.

-- ``:- #sum{N, X : in(X), val(X, N)} > 30.`` -- nie może być tak, że suma wybranych elementów jest <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=> 30">

-- ``#maximize{N, X : in(X), val(X, N)}.`` -- wybierz takie rozwiązanie, które zmaksymalizuje sumę ``N`` dodanych do rozwiązania ``in(X)``

Wynik:

```
Answer: 1

Optimizarion: 0
Answer: 2
in(c)
Optimization: -8
[...]
Answer: 5
in(a) in(c)
Optomization: -28
OPTIMUM FOUND
```

Jak widać, system maksymalizuje przez minimalizację -- wynik maksymalizacji jest z minusem.

### Przykład 5: maksymalna klika

Model:

```
e(1, 2).
% [...] reszta krawedzi
e(5, 6).
v(X) :- e(X, Y).
v(X) :- e(Y, X).

1 {in(X) : v(X)}.
:- in(X), in(Y), v(X), v(Y), X < Y, not e(X, Y).
#maximize{1, X : in(X)}.

#show in/1.
```

-- graf zamodelowany zbiorem krawędzi: fakty ``e(1, 2)`` itd. oznaczające, że wystęuje krawędź

-- generowanie wierzchołków: jeśli coś jest krawędzią (``e(X, Y)``), to ``X`` jest wierzchołkiem (spełnia predykat ``v``)

-- bierzemy do rozwiązania minimum 1 wierzchołek: ``1 {in(X) : v(X)}.`` (zakładamy, że graf nie jest pusty: ma co najmniej 1 wierzchołek)

-- więzy:  wybrane wierzchołki muszą być połączone krawędzią: nie może być tak, że: w rozwiązaniu są 2 różne wierzchołki``Y`` i ``X`` zapisane tak, że <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=X < Y"> (najpierw mniejszy wierzchołek -- a więc graf jest nieskierowany), które nie tworzą krawędzi (predykat ``e(X, Y)`` nie jest spełniony)

-- maksymalizujemy liczbę wierzchołków w rozwiązaniu (``in(X)``), w tym celu tworzymy krotki ``(1, X)`` z ``in(X)`` (sumujemy jedynki)

-- ``show in/1`` -- pokaż same rozwiązania

### Przykład 6: problem komiwojażera

Fakty

```
cost(1,2,2). cost(1,3,3). cost(1,4,1).
cost(2,4,2). cost(2,5,2). cost(2,6,4).
cost(3,1,3). cost(3,4,2). cost(3,5,2).
cost(4,1,1). cost(4,2,2).
cost(5,3,2). cost(5,4,2). cost(5,6,1).
cost(6,2,4). cost(6,3,3) cost(6,5,1).
```

-- ``cost(x, y, z) -- x -- skąd, y -- dokąd, z -- ile czasu (jak daleko, koszt przejscia)

-- chyba graf skierowany, a więc komiwojazer niesymetryczny (przejście z ``A`` do ``B`` ma inny koszt niż droga z ``B`` do ``A`` 

Model:

```
edge(X, Y) :- cost(X, Y, _).
node(X) :- cost(X, _, _). 
node(Y): - cost(_, Y, _).

{ cycle(X, Y) : edge(X, Y) } = 1 :- node(X). //jeli wezmiemy cykl, to liczba krawedzi wychodzacych z wierzcholka musi wynosic 1, patrzymy tylko na te wziete do cyklu - krawedz wzieta do cyklu, czyli liczba krawedzi wzietych to cyklu musi byc rowna 1
{ cycle(X, Y) : edge(X, Y) } = 1 :- node(Y). 

reached(Y) :- cycle(1, Y). //ustalamy wierzcholek poczatkowy, jakis numer 1 bedzie, zakladajac, ze numerujemy od 1
reached(Y) :- cycle(X, Y), reached(X). //zeby nie bylo rozlacznych cykli, kiedy Y jest osiagalny z X, jesli do cyklu wzieto X i Y; definijca rekurencyjna
:- node(Y), not reached(Y). //nie moze byc tak, ze jest jakich wiezcholek i on nie jest osiagniety - mowimy, ze kazdy musi byc osiagniety

#minimize{C, X, Y: cycle(X, Y), cost(X, Y, C) }. //przecinek oznacza "i", sumuje C, ale biore pod uwage tylko te, ktore sa w cycle(X, Y) 
```

-- generowanie krawędzi: ``edge(X, Y) :- cost(X, Y, _).`` -- niezależnie od kosztu, jeśli para ``X``, ``Y`` ma koszt, to jest krawędzią

-- graf jest skierowany, bo inaczej model zawierałby regułę mówiącą, że krawędź w jedną stronę jest równa krawędzi w drugą 

-- generowanie wierzchołków: jeśli istnieje jeden element pary mającej ma koszt (``X`` lub ``Y``), to ``X`` (``Y``) jest wierzchołkiem: to generuj z krawędzi ``edge`` cykl (``cycle``); liczba takich krawędzi wynosi zawsze 1

-- ograniczenie (w komiwojażerze graf ma cykl Hamiltona): dla dowolnego wierzchołka ``X`` (lub ``Y``)  musi istnieć tylko 1 krawędź wychodząca z tego wierzchołka (stąd jedynka dopisana do każdej krotki) 

-- ograniczenie: każdy ``Y`` wierzchołek, jeśli tworzy cykl z wierzchołkiem startowym (``1``), to jest osiągalny i jeśli jest osiągalny i jest w cyklu od ``X`` do ``Y``, to ``Y`` też jest osiągalne

-- ograniczeni: wykluczone, że jest jakiś wierzchołek (``node(Y)``), który nie jest osiągalny: komiwojażer musi odwiedzić wszystkie miejsca  

-- cel: zminimalizować koszt ``C`` generowany na podstawie zbioru krawędzi wziętych do rozwiązania (``cycle``) 

### Przykład 7: problem pokrycia

Definicja pokrycia: dane są: 

* zbiór miast, 
* czasy przejazdów (możliwe niesymetryczne), między każdą parą miast 
* dopuszczalny maks. czas _max_time_ dojazdu wozu strażackiego

Pytanie: W których miastach rozmieścić remizy strażackie, by nie przekraczając czasu <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=t"> móc dojechać do każdego miasta i aby liczba wymaganych remiz była najmniejsza?

Fakty

```
#const num_cities = 6. 			% liczba miast (stala)
#const max_time = 15. 			% maksymalny czas dojazdu (stala)
cities(1 .. num_cities). 		% fakty od 1 do num_cities

% odleglosci miedzy miastami
dist(1, 2, 10). 				% odleglosci 10 miedzy miastami 1 i 2
dist(1, 5, 30).
% [...]
dist(5, 1, 35).
dist(6, 5, 14).

% regula: jesli mamy miasto City, to mamy odleglosc 0 miedzy nim a nim samym
dist(City, City, 0) :- cities(City).

% regula: liczba remiz co najmniej 1
1 { x(City) : cities(City) }. 	% x to predykat - czy miasto City wybrano

% wiezy
:- { x(C2) : cities(C2), dist(C1, C1, Dist), Dist <= max_time } 0, cities(C1).
								% brak cyfry przed lewa klamra - od 0
								% przy ustalonym miescie C1
								% nie moze 0 takich wybranych C2 (x(C2))
								% bedacych miastami (cities(C2))
								% i dla ktorych czas dojazdu z C2 do C1 (dist)
								% jest mniejszy lub rowny max_time
% inaczej: dla kazdego miasta musi sie znalezc remiza, z ktorej dojdziemy w czasie max_time
% inaczej: liczba remiz, z ktorych dojezdzamy z miasta C1 do C2 w czasie nie wiekszym od max_time - musi byc niezerowa 

% cel
#minimize {1, City : x(City), cities(City) }. 
								% minimalizujemy sume wybranych miast (jedynek)
								% branych z wybranych miast (x(City)) 
								% i bedacych miastami (cities(City))
#show x/1. 
```

### Przykład 8: problem Max-Cut

Podział (_cut_) wierzchołków grafu na 2 rozłączne podzbiory w taki sposób, żeby liczba krawędzi łączących wierzchołki obu podzbiorów była jak największa (_max_). 

```
% fakty

#const n = 20. 				% liczba wierzcholkow
v(1..n). 					% deklaracja wierzcholkow od 1 do n

<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= krawedzie
e(1,2).		e(1,5).		e(1,10).		e(1,11).		e(2,3).
e(3,6).		e(3,7).		e(3,10).		e(4,8).			e(4,14).
e(4,17).	e(5,11).	e(5,13).		e(5,19).		e(6,7).
e(6,18).	e(7,8).		e(7,10).		e(8,10).		e(9,15).
e(12,13).	e(13,16).	e(13,19).		e(14,18).
e(15,18).	e(16,17).	e(16,19).		e(16,20).
e(17,19).	e(17,20).	
 
% liczba wierzcholkow w rozwiazaniu (v_in) od 1
1 { v_in(X) : v(X) }.

% generowanie krawedzi
e_in(X,Y) :- e(X,Y), v_in(X), not v_in(Y).
						% jesli wierzcholek X jest w rozwiazaniu 	(v_in(X))
						% oraz Y nie jest w rozwiazaniu				(not v_in(Y))
						% oraz istnieje krawedz e(X, Y)
						% to ta krawedz jest w rozwiazaniu e_in(X, Y)
% to, co wyzej, ale w odwrotnej kolejnosci 
e_in(X,Y) :- e(X, Y), v_in(Y), not v_in(X).

% cel
#maximize{ 1, X, Y : e_in(X, Y), e(X, Y) }.
						% jak najwięcej jedynek, dla kazdego X, Y
						% bedacego w rozwiazaniu e_in(X, Y)
						% i bedacych krawedziami

% show v_in/1.			% rozwiazanie - wierzcholki w jednym podgrafie
```

Przykład rozwiązania: 

![](https://www.evernote.com/shard/s443/res/104b7aba-60e2-9ad8-6edc-9e1e5705d72e)

### Przykład 9: korekcja błędów

...

# Laboratorium 7 | 20.12.2020

...

# Wykład 8 | 9.01.2020 | SMT (_Satisfiability Modulo Theories_)

Nowa metoda (trudno znaleźć opracowania po polsku). 

Do stosowania tam, gdzie wszystko inne zawodzi, np. programowanie całkowitoliczbowe lub liniowe nie działa, bo jedno z ograniczeń lub funkcja celu zawierają mnożenie (nie jest zatem liniowe). 

## Podstawowe zadanie

To metoda rozwiązywania formuły logicznej, w której część klauzul podmieniono i wstawiono w ich miejsce coś innego, np. w">(x_1 \vee \neg x_2 \vee x_3) \wedge (y + 1 \geq 7) \wedge (f(y) + 2 = z^2)<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=-- gdzie ">x<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= to zmienne boolowskie

-- zamiast zmiennej lub alternatywy zmiennej jest równanie lub nierówność (">y+1\geq 1<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, ">f(y) +2 = z^2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=)

-- zadanie SMT: sprawdzenie, czy taka formuła jest spełnialna, a jeśli tak, to co należy podłożyć pod zmienne

Można też korzystać z ">\forall<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= i ">\exists<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (ale nie wszystkie biblioteki na to pozwalają). 

Można minimalizować i maksymalizować (nie we wszystkich bibliotekach)

'theories' -- metody dotyczą dodatkowych teorii (np. boolowskie)

## Programowanie: język ``SMT``, biblioteka ``z3``

``Z3``: 

* oprogramowanie: https://github.com/Z3Prover/z3/releases
* podręcznik ``Z3`` + przykłady w ``SMT-LIB``: https://rise4fun.com/Z3/tutorial/guide
* inne języki, m.in. ``C++``: https://github.com/Z3Prover/z3/tree/master/examples
* ``Z3 C++ API``: http://z3prover.github.io/api/html/group_cppapi.html
* ``Z3`` i ``Python``: http://theory.stanford.edu/~nikolaj/programmingz3.html

Cechy biblioteki ``Z3``: 

* dokładne wyniki działań całkowitoliczbowych
* dokładne wyniki działań rzeczywistych (tzw. ==liczby algebraiczne== -- jeśli liczba jest pierwiastkiem jakiegoś wielomianu, to jest reprezentowana dokładnie w danym narzędziu) 

## Przykład 1: łamigłówka

Każda litera to cyfra. Odgadnąć, jaka to cyfra.

```
	s e n d
+   m o r e
-------------
m o n e y
```

Przykład w c++

```c++
#include"z3++.h"
#include <iostream>

using namespace z3;

int main() {
	context c;
	expr S = c.int_const("S");
	expr E = c.int_const("E");
	expr N = c.int_const("N");
	expr D = c.int_const("D");
	expr M = c.int_const("M");
	expr O = c.int_const("O");
	expr R = c.int_const("R");
	expr Y = c.int_const("Y");

	solver sol(c); 				//deklaracja solwera	

	sol.add(S >= 1 && S <= 9);	//ograniczenia każdej cyfry
	sol.add(E >= 0 && E <= 9);	//od 0, jeśli cyfra stoli na miejscu jedności
	sol.add(N >= 0 && N <= 9);
	sol.add(D >= 0 && D <= 9);
	sol.add(M >= 1 && M <= 9);
	sol.add(O >= 0 && O <= 9);
	sol.add(R >= 0 && R <= 9);
	sol.add(Y >= 0 && Y <= 9);

	sol.add(	1000 * S + 100 * E + 10 * N + D +
				1000 * M + 100 * O + 10 * R + E ==
				10000 * M + 1000 * O + 100 * N + 10 * E + Y); 
				// ograniczenie wynikające z działania
	
	expr_vector vars(c);
	vars.push_back(S);
	vars.push_back(E);
	vars.push_back(N);
	vars.push_back(D);
	vars.push_back(M);
	vars.push_back(O);
	vars.push_back(R);
	vars.push_back(E);
	vars.push_back(Y);
	sol.add(distinct(vars)); 	//każda z tych zmiennych ma się różnić
	
	if (sol.check() == sat) {	//sprawdzamy, czy jest rozwiązanie
		model mod = sol.get_model();	//jeśli tak, bierzemy je
		std::cout << "S=" << mod.eval(S) << std::endl;
		std::cout << "E=" << mod.eval(E) << std::endl;
		std::cout << "N=" << mod.eval(N) << std::endl;
		std::cout << "D=" << mod.eval(D) << std::endl;
		std::cout << "M=" << mod.eval(M) << std::endl;
		std::cout << "O=" << mod.eval(O) << std::endl;
		std::cout << "R=" << mod.eval(R) << std::endl;
		std::cout << "E=" << mod.eval(E) << std::endl;
		std::cout << "Y=" << mod.eval(Y) << std::endl;
	}
	Z3_finalize_memory();
	return 0;
}
```

Rozwiązanie: 

```
	s e n d			9 5 6 7
+   m o r e		+	1 0 8 5
-------------	-----------
m o n e y		  1 0 6 5 2 
```

## Przykład 2: znajdowanie przecięcia 2 wykresów

Znaleźć ">x>0<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= z dokładnością do 50 miejsc po przecinku, dla którego parabola ">y=x^2<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= przecina się z prostą ">y=-2x+10<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Rozwiązanie w ``C++``

```c++
context c;
expr x = c.real_const("x");		// deklaracja zmiennej
solver s(c);					// deklaracja solwera
s.add(x > 0);					// ograniczenie dla x
s.add(x * x == -2*x + 10);		// ograniczenie dot. przecięcia wykresów
if (s.check() == sat) {			// jeśli jest wynik
	model m = s.get_model();	// pobierz model
	std::cout << m.eval(x).get_decimal_string(50) << std::endl;
}	
```

## Przykład 3: obliczanie sum skończonych na podstawie rachunku różnicowego

**Twierdzenie.** 
* jeśli funkcja ">F_n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest wynikiem zastosowania operatora ">\Delta_z^{-1}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= do funkcji ">f_n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=,
* to każda funkcja postaci ">F_n + Cz^n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (">C<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= jest dowolną stałą), jest także wynikiem działania operatora ">\Delta_z^{-1}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= na funkcję ">f_n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=:

Definicja operatora ">\Delta_z f_n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=: ">\begin{array}{ll}
\Delta_z f_n = f_{n+1} - zf_n & \\
\Delta_z^{-1} f_n = F_n & \text{gdy}\ \Delta_z F_n = f_n
\end{array}"><img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=**Zadanie:**
* znaleźć ">f_n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=, dla której ">\Delta_2 f_n = n<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= (czyli: ">f_{n+1} - 2f_n = n$). 

Rozwiązanie w ``C++``

```c++
context c;
sort I = c.int_sort();				//deklaracja: I jest typu całkowitego
func_decl f = function("f", I, I);	//deklaracja funkcji f z parametrem I
									//zwracającej typ I
solver s(c);
s.add(f(2) - 2 * f(1) == 1);
s.add(f(3) - 2 * f(2) == 2);
s.add(f(4) - 2 * f(3) == 3);
s.add(f(5) - 2 * f(4) == 4);
s.add(f(6) - 2 * f(5) == 5);

if (s.check() == sat) {
	model m = s.get_model();
	for (int j=1; j<=6; j++)
		std::cout << "f(" << j << ") = " << m.eval(f(j)) << std::endl;
}
```
 


## zadanie

wybrać 1 ze zbioru 20 zadań i rozwiązać dowolną metodą, np. asp lub smt

nietypowe zadanie - użyć smt

# Laboratorium 8 | 10.01.2021

Zerówka z wykładu za 2 tygodnie na lab. (24.01.2021)

Zadania do wyboru - zapisy na https://onedrive.live.com/edit.aspx?resid=72C9A8E5D9D3AE47%211814&id=documents&authkey=!ANCh2eLG1ccyEsQ&

Wstępnie: zad. 11 - SMT




































# Laboratorium 8 | 09.01.2021

Na ost. ćwiczeniach będzie test zerowy - ocena do poprawy, do zobaczenia wymagań z zagadnień na wykładzie

Nie będzie algorytmów zachłannych - nie zdążymy

------





























> Written with [StackEdit](https://stackedit.io/).


