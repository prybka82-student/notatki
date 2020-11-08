
# Optymalizacja kombinatoryczna

## Zadania 1 (A) -- Pestycydy

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

### Formuły ograniczeń 

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





> Written with [StackEdit](https://stackedit.io/).


