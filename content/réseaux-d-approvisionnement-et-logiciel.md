---
title: Réseaux d'approvisionnement et logiciel
subtitle: Quel rapport entre container et programmation orienté-objet ?
author: Victor Lebref
date: May 05, 2022
category: Divers
summary: Quel rapport entre container et programmation orienté-objet ?
---

L’article [See no Evil](https://logicmag.io/scale/see-no-evil/) de la fantastique revue [logicmag](http://logicmag.io/) parle des chaînes d'approvisionnement et fait des liens avec le monde du logiciel. Synthétisons et allons plus loin…


## D'abord, qu'est-ce qu'une chaîne d'approvisionnement ?

En gros, la chaîne d'approvisionnement d'une entreprise, c'est l'ensemble de ses fournisseurs, et des fournisseurs des fournisseurs, etc. (cette définition est purement personnelle et absolument imprécise).

Comme le note l'article, on devrait plutôt parler d'un réseau d'approvisionnement. Car on est loin d'une structure en chaîne où l'approvisionnement est linéaire comme suit : 
    
    
    Entreprise A -> Entreprise B -> ... -> Entreprise Z -> Vente du produit final.
    

On aurait plutôt une arborescence inversée, où certains fournisseurs peuvent se substituer à d'autres en cas de pépin : 
    
    
    Entreprise A \
    Entreprise B  ---- > Entreprise D \
    Entreprise C /                     \
                                         --- > Entreprise E -> Vente du produit final.  
    Entreprise A' \                     /
    Entreprise B'  ---- > Entreprise D'/
    Entreprise C' /
    

Cette structure mobile souvent très profonde fait qu'il est très difficile de savoir, pour une entreprise, d'où proviennent ses intrants. La mondialisation fait aussi que les fournisseurs sont très loin les uns des autres.

Certaines entreprises disent pouvoir garantir certains critères de qualités, sociaux et écologiques. En réalité, c'est très difficile à faire, car il faut s'assurer que ces critères soient respectés sur tous les nœuds du réseau.

Si c'est un si gros bazar, comment ça peut marcher ? Comment, devant cette complexité, arrive-t-on tout de même à acheminer les biens sans se perdre dans la complexité ?

## Le conteneur et la programmation orientée objet

Le conteneur est un symbole de la mondialisation. Et en effet, c'est l'invention qui a permis ce développement gigantesque des chaînes de production. L'idée est simple, on a des marchandises, et on les met dans une boîte. Sur la boîte, il est écrit où elle doit être transportée. L'intérêt est qu'on a pas à se soucier de ce qu'il y a dans la boite, on a juste à l'amener à bon port ([à condition qu'elle ne tombe pas dans la mer !](https://fr.euronews.com/2022/01/13/transport-maritime-nouvelle-perte-de-conteneurs-en-mer-et-toujours-pas-de-reglementation)). Chaque acteur de la chaîne du réseau d'approvisionnement n'est exposé qu'à l'information dont il a besoin.

C'est ici qu'est fait un parallèle avec le logiciel. Une méthode de programmation appelée programmation orientée objet consiste à mettre le code dans des objets. Un objet contient des attributs et peut effectuer des actions. Cependant, un programmeur qui utilise l'objet, peut effectuer ses actions sans savoir comment les actions sont programmées. La complexité du programme est "cachée" dans l'objet. Vous voyez le lien avec le conteneur ?

Pour donner un autre exemple, je crois avoir lu quelque part une métaphore de la programmation orientée objet avec les machines à café. Quand on fait un café sur une machine Nespresso, on la laisse faire sa tambouille interne, on lui demande : "fait un café" et elle fait un café. (note : je déteste les cafetières Nespresso, c'est juste un bon exemple) 

À l'inverse, lorsqu'on utilise une cafetière à filtre, on est confronté à plus de complexité, il faut mettre l'eau dedans, puis le café, puis le mettre sur le feu, allumer le feu, etc.

Donc pour résumer, la programmation objet est l'équivalent de la conteneurisation ou de la machine à café Nespresso en programmation. C'est l'idée de mettre la complexité dans des objets, pour ne pas avoir à interagir avec cette complexité à chaque fois qu'on utilise l'objet.

## Et alors ?

L'article s'arrête là et nous laisse sur notre faim. Et donc ? Qu'est-ce qu'on peut en conclure de ça ? C'est partit pour les réflexions alambiquées et les raisonnements capillotractés !

Le mécanisme qui sous-tend la mondialisation et la complexification des réseaux d'approvisionnement s'appuie sur la même "méthode" que le développement logiciel. Est-ce qu'il faut s'attendre aux mêmes horreurs qui sortent de la mondialisation dans le développement logiciel ? A priori, je dirai non, parce que la programmation orientée objet, c'est cool. Mais je suis développeur, alors c'est comme demander à Amazon ce qu'elle pense de la conteneurisation, elle trouve ça cool bien sûr.

Alors posons plutôt la question : est-ce qu'il y a des effets indésirables de la modularité dans les logiciels ?

Peut-être. Il y a un problème de "bloat" logiciel et web. C'est-à-dire que les logiciels, même pour faire des tâches simples, ont une taille énorme. Est-ce que ce problème n'est pas le fruit de cette modularité ? Si on avait pas des objets modulaires et indépendants les unes des autres, on serait forcé de considérer toute la chaîne logicielle dans son ensemble, ce qui forcerait à la garder à une taille raisonnable. Au lieu de ça, on a des logiciels qui tournent sur des couches de millions de lignes de code pour nous afficher des recettes de cuisines... À méditer.
