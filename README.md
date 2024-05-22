# God Of GD

## I) Modifications du 1st person template (5 pts)

I.I
- ajouter le bp component d'ame au BP_FirstPersonCharacter et supprimer le pickup qui est dans la scene
- ajouter un widget de crosshair

I.II
- le BP_FirstPersonProjectile ne doit plus rebondir
- le BP_FirstPersonProjectile se détruit à l'impact
- le BP_FirstPersonProjectile spawn un niagara emiter au moment où il est détruit (prendre un emitter par defaut type burst)

### Helper I
- pour creer un niagara system : FX > niagara system > new system from selected emitters > Omnidirectional burst
- spawn system at location pour faire spawn ce system de particule 

---

## II) Séquencer (5 pts)

II.I) Créer une sequencer qui modifie le niveau et donne accàs au joueur à une nouvelle zone

II.II) Créer une Acteur interactif qui servira à déclencher cette sequence

II.III) Ajouter une action d'intéraction au BP_FirstPersonCharacter sur la touche E

### Helper II
- C'est une bonne idée d'y aller en SphereTraceByChanel avec une Interface car il y aura un autre element interactif dans la 3eme partie (le coffre)
- Pour que des changements faits par le level sequencer persiste dans le level une fois la sequence terminée ; il faut click droit sur la track (transform par pexemple) puis dans **properties > when finished > keep state**

---

III) Coffre runique (10 points)
Reproduire la mécanique de coffre runique de God of war

### Helper III
- On peut convertir des boolean en int avec le node toInt
- L'event dispatcher est votre ami
- Il serait interessant de pouvoir utiliser ce systeme de lock sous la forme d'un bp_component

---
Exemple de rendu
https://youtu.be/vsFIyGO63-o

Bon courage les Boys :)
