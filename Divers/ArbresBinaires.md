# Arbres Binaires

## Création de la classe Noeud

En utilisant le cours, écrivez la classe Noeud et son constructeur, permettant de définir des arbres binaires.
Cette classe définit les attributs `_valeur`, `_nom`, `_sag` et `_sad`.
 `_sag` et `_sad` sont initialisés à `None`.

## Ajoutez ensuite les méthodes suivantes

### setArbreGauche

* a comme paramètre (outre self), `noeud` (qui doit être un objet de type `Noeud`), qu'elle attribue à `self._sag`.
* Vérifie au moyen d'un assert que la variable `noeud` est bien du bon type.
  
### setArbreDroit 

* définie comme précédemment pour attibuer un noeud à `self._sad`
  
### affiche

* a un paramètre entier : `dec` qui a pour `valeur par défaut 1`
* permet d'afficher récursivement un abre en mettant en valeur simplement les branches.
* suit cet algorithme récursivement :
``` python
si _sag est None, afficheGauche="" 
sinon afficheGauche = "\n"+dec*"  "+self._sag.affiche(dec+1)

de même pour _sad (adapter !)
on renvoie la chaine f"{self._nom}:{self._valeur}{afficheGauche}{afficheDroit}"
```
## tester cette première partie :
écrivez dans le **main.py** un programme créant un arbre binaire de 7 noeuds nommés A,B,C,D,E et F où E et F sont les fils gauche/droit de C, B et C les fils gauche/droit de A et D le fils droit de B. 
Mettez les **valeurs** de votre choix.
Affichez cet arbre (la méthode `affiche` renvoie une chaine de caractère, il faut donc utiliser un `print`)

## Ajout des parcours
En utilisant le cours et en vous inspirant de la méthode `affiche`, écrivez les méthodes `parcoursPrefixe`, `parcoursInfixe`, `parcoursPostfixe` et testez les sur l'arbre précédent ou d'autres de votre invention.

## Ajout de méthodes

Ecrivez puis testez les méthodes suivantes :

### taille

On peut définir récursivement la taille d'un arbre en disant que s'il est vide (=None) elle vaut 0, sinon c'est `1+taille(sag)+taille(sad)`
Utilisez cette définition pour définir une méthode récursive qui renvoie un entier égal à la taille d'un arbre

### hauteur

On peut définir récursivement la hauteur d'un arbre en disant que s'il est vide (=None) elle vaut 0, sinon c'est `1+max(hauteur(sag)+hauteur(sad))`
Utilisez cette définition pour définir une méthode récursive qui renvoie un entier égal à la taille d'un arbre

### RENDU

Une fois ce TP terminé, [complétez le formulaire](https://forms.gle/cTEcV2GDJ9v84QUV9)



