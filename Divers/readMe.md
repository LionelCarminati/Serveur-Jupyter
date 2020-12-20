# Arbres Binaires de Recherche

Un arbre binaire de recherche est un arbre binaire pour lequel le sous arbre gauche ne contient que des valeurs inférieures ou égales à la valeur de la racine, et le sous arbre de droite des valeurs supérieures.

Dans ce devoir nous allons utiliser la classe ```Noeud``` déjà utilisée dans les précédents TPs, implémentée dans l'onglet ```classeNoeud.py```

Cette classe a ici comme attributs ```_valeur```,```_sag``` et ```_sad```

Les méthodes déjà implémentées sont : ```setArbreDroit```, ```setArbreGauche```, ```affiche``` et ```afficheInfixe```

## 1 Création de la méthode ajouteValeur

Ajouter à la classe Noeud la méthode ```ajouteValeur``` qui
* prend en arguments ```self``` et une valeur ```x```
* suit l'algorithme du cours

## 2 Création de la méthode ```ajouteListeValeur```

Ajouter à la classe Noeud la méthode ```ajouteListeValeurs``` qui
* prend en arguments self et une liste d'entiers ```L```
* suit l'algorithme suivant :

```bash
  pour chaque valeur x de L:
    ajouter x à l'arbre en utilisant la méthode ajouteValeur
```

## 3 Mise en application

Dans le main, créer un noeud ```A``` de valeur 50 qui sera la racine de l'arbre

En utilisant la fonction ```creeListeAleatoire``` qui
* prend en entrée un entier ```n>0```
* renvoie une Liste de n nombres aléatoires compris entre 1 et 100 inclus

créer une liste ```L``` de 20 valeurs aléatoires et ajouter toutes les valeurs de ```L``` à ```A``` avec la fonction ```ajouteListeValeurs```

Afficher le parcours infixe de A. Si tout s'est bien passé, la liste est croissante. Vérifiez.

## 4 Ecriture de la méthode ```equilibre```

On dit qu'un ABR est équilibré si pour chaque noeud, la différence entre la hauteur de son sous-arbre droit et celle de son sous-arbre gauche est comprise entre -1 et 1.

* Ecrivez la methode ```Equilibre``` qui utilise la méthode existante hauteur et qui renvoie la différence entre la hauteur du sous-arbre gauche et du sous-arbre droit. (inspirez-vous de ```hauteur```)
* Ecrivez la méthode récursive ```estEquilibre``` qui renvoie __True__ ou __False__ suivant que le noeud est équilibré ou non, ainsi que tous ses sous-arbres.

## 5 Ecriture de la méthode ```recherche```

Les arbres binaires de recherche permettent une recherche en ```O(ln(n))```.

Ecrivez la méthode ```recherche```
* qui prend en paramètre un entier x
* qui renvoie __True__ ou __False__ suivant que x est dans l'arbre ou pas.

On pourra trouver l'algorithme dans le cours. Il faut simplement l'adapter à la POO.

Une fois votre méthode écrite, ecrivez le ```main``` nécessaire pour la tester dans différents cas.

Complétez ce [formulaire] (https://forms.gle/9RjNPYnA5ozEMurE7) pour terminer ce TP

