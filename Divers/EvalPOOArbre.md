# Arbres Binaires et tri

On peut utiliser certains arbres binaires pour trier simplement une liste de nombres.

Dans ce devoir nous allons utiliser la classe ```Noeud``` déjà utilisée dans les précédents TPs, implémentée dans l'onglet ```classeNoeud.py```

Cette classe a ici comme attributs ```_valeur```,```_sag``` et ```_sad```

Les méthodes déjà implémentées sont : ```setArbreDroit```, ```setArbreGauche```, ```affiche``` et ```afficheInfixe```

## 1.A Création de la méthode ajouteValeur

Ajouter à la classe Noeud la méthode ```ajouteValeur``` qui
* prend en arguments ```self``` et une valeur ```x```
* suit l'algorithme suivant :

```
  si x > valeur de la racine
    si sad = None
      On crée un nouveau noeud N de la valeur x 
      le sous-arbre droite égale N
    sinon on appelle récursivement la méthode ajouteValeur sur l'arbre droite, avec la valeur x
  sinon
    si sag = None
      On crée un nouveau noeud N de la valeur x 
      le sous-arbre gauche égale N
    sinon on appelle récursivement la méthode ajouteValeur sur l'arbre gauche, avec la valeur x
```

### 1.B Validation de la méthode

Dans le main, créer un noeud A de valeur 50 qui sera la racine de l'arbre

Avec la méthode ```ajouteValeur```, lui ajouter les valeurs 60,40,10,20,100 puis afficher le résultat avec la méthode ```affiche```. Vous devriez obtenir ce résultat :

```bash
50
| g:40
|  | g:10
|  |  | d:20
| d:60
|  | d:100
 ```

## Copiez-collez votre méthode dans ce [formulaire] (https://forms.gle/t8jXhyBjvs5MSxHu9)  
###(faites clic-droit pour l'ouvrir dans un onglet)

## 2.A Création de la méthode ```ajouteListeValeur```

Ajouter à la classe Noeud la méthode ```ajouteListeValeur``` qui
* prend en arguments self et une liste d'entiers ```L```
* suit l'algorithme suivant :

```bash
  pour chaque valeur x de L:
    ajouter x à l'arbre en utilisant la méthode ajouteValeur
```

## 2.B création de la fonction ```creeListeAleatoire```

Ecrire dans le ```main``` la fonction ```creeListeAleatoire``` qui
* prend en entrée un entier ```n>0```
* renvoie une Liste de n nombres aléatoires compris entre 1 et 100 inclus

On pourra utiliser la fonction ```randint(a,b)``` qui renvoie un entier aléatoire entre a et b inclus.

## 2.C Mise en application

Dans le main, créer un noeud ```A``` de valeur 0 qui sera la racine de l'arbre

Créer une liste ```L``` de 20 valeurs aléatoires avec la fonction appropriées et l'affiche.

Ajouter toutes les valeurs de ```L``` à ```A``` avec la fonction ```ajouteListeValeurs```


Afficher le parcours infixe de A. Si tout s'est bien passé, la liste est croissante. Vérifiez.

## Aller plus loin : minimum et maximum

Affichez l'arbre de A au moyen de la fonction ```affiche```. La mention **g** ou **d** indique si le sous arbre est à droite ou à gauche.
Que peut-on dire de la valeur qui est à gauche d'un noeud ? De celle qui est à droite d'un noeud ?

Utilisez cette observation pour écrire les méthodes ```minimum``` et ```maximum``` de la classe ```Noeud```, qui renverront le minimum et le maximum de l'arbre dont un noeud est la racine.

## Faites SUBMIT. Vérifiez que vous avez tout bien copié dans le formulaire avant de quitter. 

