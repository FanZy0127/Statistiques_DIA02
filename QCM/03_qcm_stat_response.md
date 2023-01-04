# QCM 

## Question 1

Soit le jeu de données titanic de seaborn. Quelle méthode pouvez-vous utiliser ci-dessous pour construire un graphique de type bar ? 

Répondez en choisissant une seule et bonne réponse ci-dessous.

```python
import seaborn as sns
import matplotlib.pyplot as plt

titanic = sns.load_data('titanic')

countPclass = titanic['pclass'].value_counts()
```

- [] 
```python
countPclass.bar;
```

- [X] 
```python
countPclass.plot.bar();
```

- [] 
```python
countPclass.bar();
```

## Question 2

Donnez la définition de la médiane d'une série statistique de valeurs quantitatives.

On suppose que les données sont ordonnées par ordre croissant.

Répondez en choisissant une seule et bonne réponse ci-dessous.

- [X] La médiane est la valeur qui permet de scinder la population étudiée en deux sous-populations de même effectif.

- [ ] La médiane est la valeur qui permet de scinder la population étudiée en trois sous-populations de même effectif.

- [ ] La médiane est la valeur qui permet de scinder la population étudiée en quatre sous-populations de même effectif.


## Question 3

Donnez la définition de l'interquartile.

On suppose que les données sont ordonnées par ordre croissant.

Répondez en choisissant une seule et bonne réponse ci-dessous.

- [ ] C'est la différence entre le troisième dernier et le deuxième quartile.

- [ ] C'est la différence entre le deuxième quartile et le premier quartile.

- [X] C'est la différence entre le troisième quartile et le premier quartile.

## Question 4

Comment interprétez-vous l'interquatile de la série statistique suivante, voir le calcul ci-après :

| nombre buts | 0  |  1  | 2  | 3  | 4  | 5 | 6 | 7 |
|-------------|----|-----|--- |----|----|---|---|---|
| nombre match| 7  | 17  | 13 | 14 | 8  | 6 | 0 | 1 |

```txt
I = Q3 - Q1 = 2
```

Répondez en choisissant une seule et bonne réponse ci-dessous.

- [ ]  On a au moins 75% dans l'intervalle I des valeurs de la série qui sont séparées d'au plus de 2 buts.

- [X]  On a au moins 50% dans l'intervalle I des valeurs de la série qui sont séparées d'au plus de 2 buts.

- [ ]  On a au moins 25% dans l'intervalle I des valeurs de la série qui sont séparées d'au plus de 2 buts.

- [ ]  On peut espérer pour n'importe quel match marquer 2 buts.

## Question 5 *

Quel est la valeur du troisième index créé ci-dessous avec la fonction date_range ?

```python
import pandas as pd

index = pd.date_range('1 jan 2018', periods=1000, freq='43h36min')
```

Répondez en choisissant une seule et bonne réponse ci-dessous.

- [ ]  2018-01-06 10:48:00

- [ ]  2022-12-20 20:24:00

- [ ]  2022-12-19 00:48:00

- [X]  2018-01-04 15:12:00


## Question 6

On aimerait récupérez un dataframe, à l'aide de la méthode loc, à partir du dataframe du titanic, uniquement constitué des colonnes suvived, sex et class.

Répondez en choisissant une seule et bonne méthode ci-dessous.

```python
import seaborn as sns

```

- [] 
```python
sns.load_dataset('titanic').loc(['survived', 'sex', 'class'])
```

- [X] 
```python
sns.load_dataset('titanic').loc[:, ['survived', 'sex', 'class']]
```

- [] 
```python
sns.load_dataset('titanic').loc(:, ['survived', 'sex', 'class'])
```

- [] 
```python
sns.load_dataset('titanic').loc[['survived', 'sex', 'class'], :]
```

## Question 7

Lorsque vous faites un groupby sur un dataset et que vous calculez par exemple la moyenne, que fait Pandas sur les colonnes qui n'ont pas de sens pour ce calcul ? Voyez l'exemple suivant pour vous faire une idée de la question posée :

```python

ti = sns.load_dataset('titanic')
ti.groupby('class').mean()
``` 

Répondez en choisissant une seule et bonne réponse ci-dessous.

- [ ]  Pandas met la valeur nan dans les colonnes catégorielles.

- [ ]  Pandas lance une erreur et s'arrête.

- [X]  Pandas ignore les colonnes sur lesquelles il ne peut pas faire le calcul.

- [ ]  Pandas met la valeur 0 dans les colonnes catégorielles.

## Question 8

Déterminez le premier et le troisième quartile de la série statistique suivante, vous pouvez faire les calculs à la main.

```txt
ser = [ 2, 5, 6,   7, 7, 9,   12, 16, 22,    45 , 90, 100 ]

12/4 = 3
12*3/4 = 9

```

Répondez en choisissant une seule et bonne réponse ci-dessous.

- [ ]  7, 45

- [ ]  2, 45

- [X]  6, 22

- [ ]  6,  45



## Question 8 bis

Déterminez le premier et le troisième quartile de la série statistique suivante, vous pouvez faire les calculs à la main.

```txt
ser = [ 2, 5, 6, 7, 7, 9, 12, 16, 22, 45 , 90, 100 , 200]



```

Répondez en choisissant une seule et bonne réponse ci-dessous.

- [X]  7, 45

- [ ]  2, 45

- [ ]  6, 22

- [ ]  6,  45


## Question 9

Soit la variable statistique Sex d'un individu, définissez son type.

Répondez en choisissant une/des bonne(s) réponse(s) ci-dessous.


- [X] Variable qualitative nominale.

- [ ] Variable qualitative ordinale.

- [ ] Variable quantitative discrète.

- [ ] Variable quantitative continue.


## Question 10

Soit la variable statistique nombre d'enfants, définissez son type.

Répondez en choisissant une/des bonne(s) réponse(s) ci-dessous.


- [ ] Variable qualitative nominale.

- [ ] Variable qualitative ordinale.

- [X] Variable quantitative discrète.

- [ ] Variable quantitative continue.

## Question 11

Soit la variable statistique taille d'un individu, définissez son type.

Répondez en choisissant une/des bonne(s) réponse(s) ci-dessous.


- [ ] Variable qualitative nominale.

- [ ] Variable qualitative ordinale.

- [ ] Variable quantitative discrète.

- [X] Variable quantitative continue.


## Question 12

Soit la variable statistique nationalité d'un individu, définissez son type.

Répondez en choisissant une/des bonne(s) réponse(s) ci-dessous.


- [X] Variable qualitative nominale.

- [ ] Variable qualitative ordinale.

- [ ] Variable quantitative discrète.

- [ ] Variable quantitative continue.


## Question 13

Soit la variable statistique mention d'un examen d'un individu, définissez son type.

Répondez en choisissant une/des bonne(s) réponse(s) ci-dessous.


- [ ] Variable qualitative nominale.

- [X] Variable qualitative ordinale.

- [ ] Variable quantitative discrète.

- [ ] Variable quantitative continue.

## Question 14

Soit la variable statistique couleur des yeux  d'un individu, définissez son type.

Répondez en choisissant une/des bonne(s) réponse(s) ci-dessous.


- [X] Variable qualitative nominale.

- [ ] Variable qualitative ordinale.

- [ ] Variable quantitative discrète.

- [ ] Variable quantitative continue.


## Question 15

Soit la variable statistique nombre de bonnes réponses à un QCM, définissez son type.

Répondez en choisissant une/des bonne(s) réponse(s) ci-dessous.


- [ ] Variable qualitative nominale.

- [ ] Variable qualitative ordinale.

- [X] Variable quantitative discrète.

- [ ] Variable quantitative continue.


## Question 16

Calculez la fréquence conditionnelle des personnes dont le sang est de rhésus positif, parmi les personnes de groupe sanguin A.


              A        B      AB     O
| Rh+      | 3000  |  800  | 400  | 3000 |
|----------|-------|-------|----- |----- |
| Rh-      | 700   |  200  |  809 | 1000 |


Répondez en choisissant une/des bonne(s) réponse(s) ci-dessous.


- [X] Frh+A = 3000/3700

- [ ] Frh+A = 3700/3000

- [ ] Frh+A = 3000/7200

- [ ] Frh+A = 3000/3700


## Question 16

Calculez la fréquence conditionnelle des personnes dont le sang est de rhésus négatif, parmi les personnes de groupe sanguin B.


              A        B      AB     O
| Rh+      | 3000  |  800  | 400  | 3000 |
|----------|-------|-------|----- |----- |
| Rh-      | 700   |  200  |  809 | 1000 |


Répondez en choisissant une/des bonne(s) réponse(s) ci-dessous.


- [ ] Frh-B = 200/3700

- [X] Frh-B = 200/1000

- [ ] Frh-B = 1000/800

- [ ] Frh-B = 800/7200


## Question 17

Calculez la fréquence conditionnelle des personnes dont le sang est de rhésus négatif, parmi les personnes de groupe sanguin AB.


              A        B      AB     O
| Rh+      | 3000  |  800  | 400  | 3000 |
|----------|-------|-------|----- |----- |
| Rh-      | 700   |  200  |  809 | 1000 |


Répondez en choisissant une/des bonne(s) réponse(s) ci-dessous.


- [ ] Frh-B = 400/3700

- [ ] Frh-B = 809/400

- [ ] Frh-B = 400/1209

- [X] Frh-B = 809/1209


## Question 18

Calculez la fréquence conditionnelle des personnes dont le groupe sanguin est A parmi les Rh+


              A        B      AB     O
| Rh+      | 3000  |  800  | 400  | 3000 |
|----------|-------|-------|----- |----- |
| Rh-      | 700   |  200  |  809 | 1000 |


Répondez en choisissant une/des bonne(s) réponse(s) ci-dessous.


- [ ] FARh+ = 400/3700

- [X] FARh+ = 3000/7200

- [ ] FARh+ = 400/1209

- [ ] FARh+ = 1209/400

## Question 19

Qu'affiche la table croisée suivante ? ti est le datatset du titanic vu en cours.


```python

pd.crosstab(ti['sex'], ti['survived'], margins=True)

```

Répondez en choisissant une/des bonne(s) réponse(s) ci-dessous.


- [ ] Le nombre de survivants par sex sans les totaux marginaux.

- [X] Le nombre de survivants par sex avec les totaux marginaux.

- [ ] Le nombre de survivants sans les totaux marginaux.


## Question 20

Donnez la définition du mode en statistiques ?


Répondez en choisissant une/des bonne(s) réponse(s) ci-dessous.


- [ ] Le mode correspond à la valeur de la variable pour laquelle l'effectif (ou la fréquence) est le plus bas.

- [ ] Le mode correspond à la valeur de la variable pour laquelle l'effectif (ou la fréquence) est le plus moyen.

- [X] Le mode correspond à la valeur de la variable pour laquelle l'effectif (ou la fréquence) est le plus grand.

- [ ] Le mode correspond à la valeur de la variable pour laquelle l'effectif (ou la fréquence) est le plus médian.


## Question 21

L'écart type est selon vous un indicateur de quel type ? 


Répondez en choisissant une/des bonne(s) réponse(s) ci-dessous.


- [ ] De position.

- [X] De dispertion.

- [ ] De bruit de fond.


## Question 22

La moyenne est selon vous un indicateur de quel type ? 

Répondez en choisissant une/des bonne(s) réponse(s) ci-dessous.


- [X] De position.

- [ ] De dispersion.

- [ ] De bruit de fond.


## Question 23

La médiane est selon vous un indicateur de quel type ? 


Répondez en choisissant une/des bonne(s) réponse(s) ci-dessous.


- [X] De position.

- [ ] De dispersion.

- [ ] De bruit de fond.


## Question 24

Qu'indique la covariance pour deux variables statistiques quantitatives ?


Répondez en choisissant une/des bonne(s) réponse(s) ci-dessous.


- [ ] La covariance indique ou mesure la fréquence. 

- [X] La covariance indique ou mesure le degré de dépendance entre deux variables X et Y.

- [ ] La covariance indique ou mesure la moyenne des écarts des variables séparemment.


## Question 25

Qu'indique le coefficient de corrélation suivant pour deux variables X et Y quantitatives ?


```txt
-0.25 
```

Répondez en choisissant une/des bonne(s) réponse(s) ci-dessous.


- [ ] Une forte corrélation entre X et Y négative.

- [ ] Une forte corrélation entre X et Y positive.

- [X] Une faible corrélation entre X et Y négative.

- [ ] Une indépendance total entre X et Y.

## Question 26

Qu'indique le coefficient de corrélation suivant pour deux variables X et Y quantitatives ?


```txt
-0.75 
```

Répondez en choisissant une/des bonne(s) réponse(s) ci-dessous.


- [X] Une forte corrélation entre X et Y négative.

- [ ] Une forte corrélation entre X et Y positive.

- [ ] Une faible corrélation entre X et Y négative.

- [ ] Une indépendance total entre X et Y.

## Question 28

Qu'indique le coefficient de corrélation suivant pour deux variables X et Y quantitatives ?


```txt
0.75
```

Répondez en choisissant une/des bonne(s) réponse(s) ci-dessous.


- [ ] Une forte corrélation entre X et Y négative.

- [X] Une forte corrélation entre X et Y positive.

- [ ] Une faible corrélation entre X et Y négative.

- [ ] Une indépendance total entre X et Y.


## Question 29

Considérons une famille avec trois enfants. Chaque enfant a autant de chance d’être une fille que d’être un garçon.

Le sexe du deuxième et du troisième enfant est indépendant du sexe du précédent. On donne le script suivant pour effectuer cette estimation :

```python
NB_CHILD = 3
N = 1_000
all_girls = 0 # tous des filles
either_girl = 0 # au moins une est une fille

for _ in range(N):
    younger, middle, older = np.random.choice(['girl', 'boy'], NB_CHILD)

        #  Le nombre de familles dont les deux enfants sont une fille
    if older == 'girl' and younger == 'girl' and middle == 'girl':
        all_girls += 1

        #  Le nombre de familles qui ont au moins une fille
    if older == 'girl' or younger == 'girl' or middle == 'girl':
        either_girl += 1

```

Quel est la probabilité que tous les enfants soient des filles ?

Choisissez un script ci-dessous permettant de déterminer cette probabilité.


- [X]

```python
print(all_girls/N)
```

- [ ]

```python
print(all_girls/3)
```

- [ ]

```python
print(either_girl/all_girls)

```


## Question 30

Considérons une famille avec trois enfants. Chaque enfant a autant de chance d’être une fille que d’être un garçon.

Le sexe du deuxième et du troisième enfant est indépendant du sexe du précédent. On donne le script suivant pour effectuer cette estimation :

```python
NB_CHILD = 3
N = 1_000
all_girls = 0 # tous des filles
either_girl = 0 # au moins une est une fille

for _ in range(N):
    younger, middle, older = np.random.choice(['girl', 'boy'], NB_CHILD)

        #  Le nombre de familles dont les deux enfants sont une fille
    if older == 'girl' and younger == 'girl' and middle == 'girl':
        all_girls += 1

        #  Le nombre de familles qui ont au moins une fille
    if older == 'girl' or younger == 'girl' or middle == 'girl':
        either_girl += 1

```

Quel est la probabilité qu'au moins un des enfants soient une fille ?

Choisissez un script ci-dessous permettant de déterminer cette probabilité.


- [ ]

```python

            
#
print(all_girls/N)
```


- [ ]

```python
print(all_girls/3)
```

- [X]

```python
print(either_girl/N)
```