# Arbres Binaires et Files

## Création de la classe File

En révisant le cours sur la structure de données Files, complétez la classe File du fichier FilePOO 

## Copiez-collez la classe Noeud

reprenez la du TP précédent et copiez la dans le fichier adéquat. Copiez également le main qui définit un arbre à partir de cette classe.

## Ajout de méthodes

Ecrivez puis testez les méthodes suivantes :

### parcoursEnLargeur

Cette méthode suit l'algorithme suivant :

```
F est une File vide
enfiler SELF dans F
P est une liste initialisée avec SELF._NOM
TANT QUE F n'est pas vide :
  défiler F dans la variable ARBRE
  GAUCHE = _sag de ARBRE
  DROIT = _sad de ARBRE
  si GAUCHE n'est pas vide (ie =None)
    enfiler GAUCHE dans F
    ajouter _NOM de GAUCHE à P
  si DROIT n'est pas vide (ie =None)
    enfiler DROIT dans F
    ajouter _NOM de DROIT à P
Renvoyer P
```

### Minimum et Maximum

On peut définir récursivement le minimum d'un  arbre : si un noeud est une feuille (pas de sous arbres), le minimum est sa valeur, sinon c'est le minimum entre sa valeur et celui de ses feuilles.

Utilisez cette définition pour définir une méthode récursive qui renvoie un nombre égale au minimum des valeur de l'arbre.

Dupliquez et adaptez la pour renvoyer le maximum.

### RENDU

Une fois ce TP terminé, [complétez le formulaire](https://forms.gle/RxXaP8oAwpksKm8o8)


