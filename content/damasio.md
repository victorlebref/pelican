---
title: Analyse de phonèmes: la Horde du Contrevent de Alain Damasio
author: Victor Lebref
date: March 24, 2020
category: Analyse de donnée
summary: Analyse des caractéristiques de langage des personnages
---


Cet article fait une analyse de texte de la Horde du Contrevent de Alain
Damasio en se focalisant sur l'hétérogénéité dans les interventions des
différents personnages. On essaye de voir si une analyse quantitative du
texte nous permet de détecter des particularité du language des
personnages.

## Nombre d'interventions


|Caracole |Golgoth  |Oroshi |Pietro  | Sov |
|---------|---------|--------|--------|--------|
|      50 |     33  |    70  |    128 |     177|

Sov est le personnage qui fait le plus d'interventions. J'ai été surpris
de constater que Pietro parle aussi beaucoup, alors que ses
interventions ne m'ont pas particulièrement marquées dans le livre.
Comme expliqué
[ici](https://blogs.mediapart.fr/raphadasilva/blog/181117/la-horde-du-contrevent-un-aller-retour-eprouvant),
même si le livre se veut polyphonique, il y a quand même des narrateurs
principaux (Sov et Pietro notamment), qui parlent beaucoup plus que les
autres et dont, on le verra, le language est plus neutre.


## Longueur moyene des interventions

![]({attach}media/928b675bccb7980b6c6a3d6c727f8e8e014a9330.svgz){width="672"}

Non seulement Sov fait le plus d'intervention, mais c'est aussi celui
qui fait les interventions les plus longues. A l'inverse de Caracole qui
est percutant mais concis.


## Longueur des phrases

![]({attach}media/4e6e211aa491174f53336f63878282901ef879da.svgz){width="672"}

La longueur des phrases est calculées en terme de caractère, pas de
mots. Caracole et Pietro disent beaucoup de phrases très courtes, comme
le montre la forme ramassée de la distribution. Sov, Aoi et Larco au
contraire font au contraire des phrases plus longues.


## Longueur des mots

![]({attach}media/792501f505c2ab8a624ac728dd5c1d01aea90d2e.svgz){width="672"}

Ici j'ai retiré du graphique une valeur extrême : un mot de Sov de plus
trente lettre ! Ce mot est "nnnnnnnnnnooooooooooooorrrrrrrrrrrrrr". de
"NORS-KA !" que Pietro crie en réponse à Golgoth.


## Vocabulaire

Ici on calcul le nombre de mots différents utilisés divisé par le nombre
total de mots utilisés. A la manière de cette célèbre analyse du
vocabulaire chez les rappeurs
:<https://pudding.cool/projects/vocabulary/index.html>

![]({attach}media/455096fda0928da9b3bb44e130e864b1574c431a.svgz){width="50%"}![](media/a1076810a02c85c8ad6d07165222cc2a8050ec02.svgz){width="50%"}

Sans surprise Caracole caracole en tête, presque 40% des mots qu'il
utilise ne sont utilisés qu'une seule fois. Cela n'est guère étonnant
pour ce personnage de vif, maître de l'art oratoire. Sov le plus bavard,
se répète beaucoup plus. Mais plus l'on parle, plus il est difficile de
ne pas répéter des mots, cela explique pourquoi ce graphique ressemble au
graphique inverse du nombre d'interventions.


## Nuage de mots

Qu'est ce que les personnages disent ? On fait un nuage de mots pour
voir les concepts qui sont les plus présents dans leurs interventions

On doit d'abord faire un peu de nettoyage des données. Retirer la
ponctuation, retirer les noms des personnages (je suis seulement
intéressé par les mots, pas les noms.)

### Caracole

![]({attach}media/75a651f4503e1b93c4e750e2e7239d31ca06732f.png){width="672"}

### Golgoth

![]({attach}media/66a73f5731a98695f9c8f893f8714b67b30b2ec1.png){width="672"}

### Oroshi

![]({attach}media/7eb158aad950bd19eb8618d5b59399964f3337b4.png){width="672"}

### Pietro

![]({attach}media/b71fd331c415ff29aacecf53f033befb8bfc60ae.png){width="672"}

### Sov

![]({attach}media/947ce0e3d893fa01713785ae082b9d9f54f504b6.png){width="672"}

Comme on l'a vu, Caracole a un très grand vocabulaire. Il est normal que
son nuage de mot ne soit pas dominé (il était dominé par Sélème parce
que son nom était écrit à chacune de ses interventions sur tout un passage, je l'ai donc
retiré).

Golgoth est un jusqu-au-boutiste, il ne fait pas de compromis. Ses mots
sont "rien", "bout" comme "au bout", "dessus", "toute", "personne",
"premier". Il est aussi le chef de la horde, il est normal qu'il en
parle beaucoup de cette horde, de sa structure et son objectif ("horde",
"pack", "contre")

# Analyse des phonèmes

Dans cette partie, on fait une analyse des phonèmes les plus utilisés
par les personnages.

> J'ai toujours travaillé sur une écriture assez
physique, fondée sur les phonèmes, sur la puissance d'expressivité des
consonnes, des voyelles.
<https://www.centrepompidou.fr/fr/magazine/article/alain-damasio-lecrivain-des-zones-imaginaires>

On va donc éssayer de voir de manière quantitative quel travail il a
fait sur le profil phonétique des personnages.

Pour chaque personnage j'ai regardé quels phonèmes il utilisait le plus,
en donnant sa "traduction" en français (le son correspondant écrit en lettre alphabétique). Je me suis concentré sur Caracole, Golgoth et Sov car ils ont chacun une manière particulière de s'exprimmer surtout les deux premiers, Sov est plutôt pris comme référence.

### Golgoth

"Dès que **j**'ai reniflé le **b**l**aa**st, à l'odeur de froid,
**j**'ai su que ç**a** allait **cha**rcler. **J**'ai enfoncé mon
c**a**s**qu**e de **c**uir, plein front, san**g**lé le pourpoint,
sec. **J**usqu'au **g**roin."


![]({attach}media/19876c5db2b4b498a75fe27727259415ea34cfe7.svgz){width="50%"}

|Phonème  |"Équivalent français"
|---------|-----------------------
|ɡ        |gu
|ʃ        |ch
|a        |a
|b        |b
|ʒ        |j


### Caracole

"Des cy**ch**r**o**nes, des psy**ch**r**o**nes, des **ch**r**o**tales à
la l**ou**che, en vrac, par pa**q**uets de cin**q**, par de **d**ouze,
gris métallisé, r**ou**ge garance ou bleu **cou**rge, pour t**ou**tes
les c**ou**rses et les dég**oû**ts, ne **f**uyez pas n**ou**s
**au**tres, pas enc**o**re !"

![]({attach}media/cc927cfcb5bdab77b0cd4c5fe93bc4bf73e027d7.svgz){width="50%"}

|Phonème  |"Équivalent français"
|---------|-----------------------
|ɔ        |o ouvert
|o        |o fermé
|f        |f
|k        |k
|u        |ou


### Sov

![]({attach}media/92dac954ad0fb8e2d3889cb0f59ef1e59aa399a2.svgz){width="50%"}

|Phonème  |"Équivalent français"
|---------|-----------------------
|ʃ        |ch
|f        |f
|i        |i
|d        |d
|n        |n

