
# Optymalizacja kombinatoryczna -- zadania, seria 2

## Zadanie A -- Pestycydy

### Dane wejściowe

* składniki każdego pestycydu: Carb, Mal
* pestycydy: Pest, Bug
	* a zatem kombinacja pestycydów i składników: 
		* Pest { Carb, Mal }
		* Bug { Carb, Mal }
* ceny składników:
	* Pest: 3
	* Bug: 2,5
* minimalna zawartość każdego składniku w każdym pestycydzie: 
	* Carb: 120
	* Mal: 60
* zawartość składników w 1 jednostce każdego pestycydu: 

| | Carb | Mal | 
| - | - | - |
| Pest | 30 | 40 |
| Bug | 40 | 20 |
 
 ### Szukane 
Minimalny koszt pestycydów zawierających minimalną zawartość każdego składnika. 

### Zapis danych wejściowych 

...w GNU MathProg i ich analogiczne zapisy matematyczne. 

| Kod GNU MathProg | Zapis matematyczny |
| - | - |
| ``set Pestycydy := Pest Bug;`` | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Pestycydy = \{ Pest, Bug \}"> |
| ``set Skladniki := Carb Mal;`` | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=Skladniki = \{ Carb, Mal\}"> |
| ``param cena := Pest 3 Bug 2.5;`` | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=cena = \{3_{Pest}, 2.5_{Bug}\}"> |
| ``param zawartosc :=``<br/>``Carb Pest 30``<br/>``Carb Bug 40``<br/>``Mal Pest 40``<br/>``Mal Bug 20`` | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=zawartosc = \{"><br/><img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=30_{Carb,Pest}, 40_{Carb,Bug},"><br/><img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=40_{Mal,Pest}, 20_{Mal,Bug}"><br/><img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\}"> |
| ``param norma := Carb 120 Mal 60;`` | <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=norma = \{120_{Carb}, 60_{Mal}\}"> |

Przepisanie danych z kodu GNU MathProg na zapis w postaci zbiorów i wartości z indeksami jest pomocny: w GNU MathProg operuje się na indeksach. 

### Formuły ograniczeń i celu

Ilość pestycydu ``Pest`` i ``Bug`` musi być taka, by zawarte w nich składniki były większe lub równe normie. 

Norma wynosi 120 dla ``Carb`` i 60 dla ``Mal``. 

1 jednostka  ``Pest`` zawiera 30 jednostek ``Carb`` i 40 jednostek ``Mal``. 

1 jednostka  ``Bug`` zawiera 40 jednostek ``Carb`` i 20 jednostek ``Mal``.

Zdefiniujmy więc ilość jednostek obu pestycydów: 
* ``p`` -- liczba jednostek ``Pest``
* ``b`` -- liczba jednostek ``Bug`` 

Ograniczenie zatem wyglądają następująco: 
* dla ``Carb``: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=p \times 30 + b \times 40 >= 120">
* dla ``Mal``: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=p \times 40 + b \times 20 >= 60"> 

Cena wszystkich pestycydów natomiast: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=p \times 3 + b \times 2.5"> -- musi być minimalna. 

Zapiszmy powyższe formuły z użyciem indeksów: 

* ograniczenie ``Carb``: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=p \times 30_{Carb, Pest} + b \times 40_{Carb, Bug} >= 120_{Carb}"> 
* ogranicznie ``Mal``: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=p \times 40_{Mal, Pest} + b \times 20_{Mal, Bug} >= 60_{Mal}"> 
* cena: <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=p \times 3_{Pest} + b \times 2.5_{Bug}"> 

W każdej formule mamy sumy. Zapiszmy je przy użyciu operatora sumy <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=\sum">: 

* ograniczenie ``Carb``: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\sum_{p \in P} j_p \times z_{Carb, p} >= n_{Carb} ">

* ograniczenie ``Mal``: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\sum_{p \in P} j_p \times z_{Mal, p} >= n_{Mal}">

* cena: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\sum_{p \in P} j_p \times c_p">

gdzie: 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=j_p"> -- liczba jednostek pestycydu _p_ 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=z_{Carb,p}">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=z_{Mal,p}"> -- zawartość składnika ``Carb`` i ``Mal`` w pestycydzie _p_
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n_{Carb}">, <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=n_{Mal}"> -- norma dla składnika
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=c_p"> -- cena pestycydu _p_ 
* <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=P"> -- zbiór pestycydów

Te same ograniczenia zapisane w kodzie GNU MathProg: 

* ograniczenie ``Carb``: 

``s.t. carb{s in Carb}:``<br/>``sum{p in Pestycydy} jednostki[p] * zawartosc[s,p] >= norma[s];``

* ograniczenie ``Mal``: 

``s.t. mal{s in Mal}:``<br/>``sum{p in Pestycydy} jednostki[p] * zawartosc[s,p] >= norma[s]; ``

* cena: 

``minimize cena_calkowita:``<br/>``sum{p in Pestycydy} jednostki[p] * cena[p];``

* gdzie: 
	* ``s`` indeks zbiorów ``Carb`` i ``Mal``
	* ``Carb`` jednoelementowy zbiór zawierający etykietę ``'Carb'``
	* ``p`` indeks zbioru ``Pestycydy``	
	* ``jednostki`` -- zbiór jednostek pestycydów
	* ``zawartosc`` -- zbiór zawartości
	* ``norma`` -- zbiór norm
	* ``Mal`` jednoelementowy zbiór zawierający etykietę ``'Mal'`` 
	* ``cena`` -- zbiór cen 

### Dane

```
data;

set Pestycydy := Pest Bug;
set Skladniki := Carb Mal;

param cena := Pest 3 Bug 2.5;
param zawartosc :=
   Carb Pest 30
   Carb Bug 40
   Mal Pest 40
   Mal Bug 20;

param norma := Carb 120 Mal 60;

end;
```

### Model

```
set Pestycydy; # deklaracja zbioru pestycydow
set Skladniki; # deklaracja zbioru skladnikow
 
# deklaracja ceny -- parametr indeksowany elementami ze zbioru Pestycydy
param cena{p in Pestycydy};
 
# deklaracja zawartosci -- parametr indeksowany elementami ze zbiorow Pestycydy i Skladniki
param zawartosc{s in Skladniki, p in Pestycydy};
 
# deklaracja normy -- parametr indeksowany elementami ze zbioru Skladniki
param norma{s in Skladniki};
  
# deklaracja jednostek
#param jednostki{p in Pestycydy}, integer, >= 0;
#param jednostki{p in Pestycydy};
param jednostki{p in Pestycydy}, default 0;
  
# ograniczenia
s.t. carb{s in Skladniki: s <> 'Mal'}: sum{p in Pestycydy} jednostki[p] * zawartosc[s,p] >= norma[s];
s.t. mal{s in Skladniki: s <> 'Carb'}: sum{p in Pestycydy} jednostki[p] * zawartosc[s,p] >= norma[s];

#s.t. carb: sum{p in Pestycydy} jednostki[p] * zawartosc['Mal',p] >= norma['Mal'];
#s.t. mal: sum{p in Pestycydy} jednostki[p] * zawartosc['Carb',p] >= norma['Carb'];
 
# cel
minimize cena_calkowita: sum{p in Pestycydy} jednostki[p] * cena[p];
  
solve;
 
#display "Jednostki: ", jednostki;
printf{p in Pestycydy} "Jednostka %s = <img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math=.2f", p, jednostki[p];

end;
```

## Zadanie B - Inwestowanie

### Dane wejściowe

* ``X`` -- kwota do zainwestowania
* możliwości: 
	* fundusz A -- zysk: 9% z X
	* fundusz B -- zysk: 11% z X
	* lokata L -- zysk: 10% z X
* ograniczenia:
	* maksymalna inwestycja w A: 1/2 X
	* maksymalna inwestycja w B: 1/2 X
	* maksymalna inwestycja w B: Y
	* minimalna inwestycja w L: Z
 
### Szukane 

Maksymalny zysk z inwestycji. 

### Zapis danych wejściowych 

...w GNU MathProg i ich analogiczne zapisy matematyczne. 

| Kod GNU MathProg | Zapis matematyczny |
| - | - |
| ``param X := 200000;`` | ">X = 200000<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= |
| ``param Y := 40000;`` | ">Y = 40000<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= |
| ``param Z:= 70000;`` | ">Z = 70000<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= |

### Formuły ograniczeń i celu

Przyjmijmy zmienne: 
* ">ile_A<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- kwota zainwestowana w A
* ">ile_B<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- kwota zainwestowana w B
* ">ile_L<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- kwota zainwestowana w L

Zyski: 
* ">zysk_A<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- procent zysku w A
* ">zysk_B<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- procent zysku w B
* ">zysk_L<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= -- procent zysku w L

Wówczas ograniczenia: 
* ogrA: ">ile_A <= \frac{X}{2}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 
* ogrB1: ">ile_B <= \frac{X}{2}<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 
* ogrB2: ">ile_B <= Y<img style="min-width: 300px;" src="https://render.githubusercontent.com/render/math?math= 
* ogrL: ">ile_L >= Z$ 

Cel: 

<img style="min-width: 400px; display: block; margin-left: auto; margin-right: auto;" src="https://render.githubusercontent.com/render/math?math=\sum_{i \in \{A, B, L\}} ile_i \times zysk_i">

Zapis ograniczeń w języku GNU MathProg

* ``s.t. ogrA: ile['A'] <= 0.5 * X;``
* ``s.t. ogrB1: ile['B'] <= 0.5 * X;``
* ``s.t. ogrB2: ile['B'] <= Y;``
* ``s.t. ogrL: ile['L'] >= Z;``

Zapis celu w języku GNU MathProg

* ``maximize zysk_calk: sum{m in mozliwosci} ile[m] * zysk[m];``


### Dane

```
data;

set Pestycydy := Pest Bug;
set Skladniki := Carb Mal;

param cena := Pest 3 Bug 2.5;
param zawartosc :=
   Carb Pest 30
   Carb Bug 40
   Mal Pest 40
   Mal Bug 20;

param norma := Carb 120 Mal 60;

end;
```

### Model

```
# deklaracja wartosci
param X default 0;
param Y default 0;
param Z default 0;

# mozliwosci
set mozliwosci := {'A', 'B', 'L'};

# ile zainwestowano
param ile{m in mozliwosci} default 0;

# ograniczenia
s.t. ogrA: ile['A'] <= 0.5 * X;
s.t. ogrB1: ile['B'] <= 0.5 * X;
s.t. ogrB2: ile['B'] <= Y;
s.t. ogrL: ile['L'] >= Z;

# cel
maximize zysk_calk{m in mozliwosci}: ile[m] * .09 + ile[m] * .11 + ile[m] * .1;

solve;
display "Zysk: ", zysk_calk;  

end;
```


























> Written with [StackEdit](https://stackedit.io/).


