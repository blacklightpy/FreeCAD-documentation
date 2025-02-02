---
- GuiCommand:/fr
   Name:PartDesign Boolean
   Name/fr:PartDesign Opérations booléennes
   MenuLocation:Part Design → Opération booléenne
   Workbenches:[PartDesign](PartDesign_Workbench/fr.md)
   Version:0.17
---

# PartDesign Boolean/fr

## Description

L**\'Opération booléenne** importe un ou plusieurs [PartDesign Corps](PartDesign_Body/fr.md) ou [PartDesign Clones](PartDesign_Clone/fr.md) (désignés comme \"corps d\'outils\") dans un PartDesign Corps actif et applique une opération booléenne (fusion, soustraction ou intersection).

![](images/PartDesign_Boolean_example.png )



*A gauche : un corps actif (A) avec des corps (B) et (C). A droite : le résultat après une soustraction booléenne.*

## Utilisation

1.  [Activer le corps](PartDesign_Body/fr#Statut_actif.md) qui doit recevoir la fonction booléenne. ***Remarque** : il est important de s\'assurer que ni le corps actif, ni aucune des fonctions qu\'il contient ne soit sélectionné avant de passer à l\'étape 2.*
2.  Pressez le bouton **<img src="images/PartDesign_Boolean.svg" width=16px> [Opération booléenne...](PartDesign_Boolean/fr.md)**.
3.  Dans **Paramètres booléens**, cliquez le bouton **Ajouter un corps**. Le corps actif va temporairement disparaître de la vue 3D pour faciliter les sélections.
4.  Dans la [vue 3D](3D_view/fr.md), sélectionnez le corps à utiliser dans la fonction booléenne. Répétez pour ajouter plus de corps.
5.  Sélectionnez le type d\'opération booléenne dans le menu déroulant (fusion, soustraction ou intersection).
6.  Cliquer **OK**.

Alternativement, un ou plusieurs corps peuvent être sélectionnés avant d\'appuyer sur le bouton booléen. Ils seront automatiquement ajoutés.

## Options

-   **Union :** fusionne le ou les corps désignés avec le corps actif.
-   **Soustraction :** soustrait le corps ou les corps désignés du corps actif.
-   **Intersection :** extrait l\'intersection du ou des corps sélectionnés avec le corps actif.
-   Presser le bouton **Enlever un corps** pour retirer un corps, en le sélectionnant dans la [vue 3D](3D_view/fr.md).

## Propriétés

-    **Type**: définit l\'opération booléenne (Fuse, Cut, Common)

-    **Label**: nom donné à l\'opération, ce nom peut être changé à volonté.

-    **Group**: liste des corps d\'outils.

-    **Display**: définit l\'affichage entre 2 modes :

    -   Résultat (par défaut) : affiche le résultat de la fonction booléenne. Dans ce mode, les corps d\'outils ne peuvent pas être affichés dans leur état original, même si leur visibilité est activée.
    -   Outils : affiche les corps d\'outils dans leur état d\'origine. Ce mode est utile lorsque les corps d\'outils doivent être modifiés ou utilisés dans des opérations ultérieures.

-    **Selectable**: vrai ou faux. Si la valeur est false, l\'élément ne peut pas être sélectionné dans la vue 3D.

-    **Visibility**: vrai ou faux. Permet de basculer la visibilité de l\'élément dans la vue 3D.

## Limites

-   Pour que Intersection puisse fonctionner avec plus d\'un corps d\'outil, ils doivent tous avoir une partie commune avec le corps actif.
-   Les corps utilisés adoptent l\'origine locale du corps actif. Si le corps actif n\'est pas situé à (0,0,0) dans le système de coordonnées global, le placement des corps d\'outils doit être relatif au corps actif. Il peut être plus facile de laisser le placement du corps actif à l\'origine avant d\'appliquer la fonction booléenne, que de modifier son placement.





{{PartDesign Tools navi

}}



---
![](images/Right_arrow.png) [documentation index](../README.md) > [PartDesign](PartDesign_Workbench.md) > PartDesign Boolean/fr
