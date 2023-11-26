# La prophétie d'Atlantis

Peu de gens le savent, mais certaines grandes inventions de l'informatique et des mathématiques ont en réalité été imaginées et réalisées par l'ancienne civilisation d'Atlantis, il y a de ça très longtemps. Par exemple, le monde moderne doit en réalité l'abacus, le relais électromécanique et le transistor au peuple d'Atlantis.

Le mythique CPU 6502, utilisé notamment dans le Apple II, le Commodore 64 et le Nintendo Entertainement System, a lui aussi été développé par le peuple d'Atlantis, et est considéré comme l'une de leurs plus grandes réalisations technologiques.

Ce n'est donc pas surprenant que cette technologie fût choisie lorsqu'est venu le temps pour eux de développer une solution d'encryption pour protéger leur plus importante prophétie, la fameuse prophétie d'Atlantis.

En effet, des recherches ont permis de mettre la main sur l'image binaire d'un programme développé pour une architecture 6502, qui, si on lui fournit la bonne clé d'encryption, révèlera la fameuse prophétie d'Atlantis ainsi que le nom du sage qui en est le messager.

## Résumé

Le comité des universités désire conserver l'histoire de l'ancienne civilisation d'Atlantis. Pour ce faire, il demande à votre équipe de déchiffrer le message de la prophétie. Ensuite, il vous demande de comprendre le fonctionnement du mythique processeur 6502 afin de conserver les connaissances et d'être en mesure de les transmettres aux futurs ingénieurs logiciels qui seront formés dans les grandes universités de notre nouvelle civilisation.

## Informations techniques

**Vous devez utiliser le langage _C_**

### Détails sur l'émulateur 6502

-   Le système a 64kB (65536 bytes) de mémoire vive ;
-   Vous devez fournir à l'émulateur (donc implémenter) 2 fonctions, _read6502_ et _write6502_ qui seront appelées par ce dernier pour lire ou écrire en mémoire ;

### Détails sur le fichier binaire mystérieux:

-   La clé d'encryption est une chaîne de 3 caractères contenant uniquement des chiffres. Il y a donc 10^3 ("000" - "999") clés possibles ;
-   La clé d'encryption doit être placée à l'adresse 0x200 avant l'éxécution du binaire. La clé occupera donc les cellules 0x200, 0x201, 0x202 ;
-   Pour chaque éxécution, le binaire fera 48 écritures à l'adresse de mémoire 0xFFF1 une fois la décryption terminée. Si la clé est bonne, la prophétie sera révélée ainsi. Si la clé est mauvaise, le charactère '#' sera écrit 48 fois à l'adresse mentionnée. Note: La prophétie ne contient pas le charactère '#' ;

## Tâches

### Faire fonctionner l'émulator 6502

-   Utiliser la librairie fournie (20 points)
-   Implémenter la gestion de la mémoire dans votre programme (100 points)
-   Créer la fonction _read6502_ (30 points)
-   Créer la fonction _write6502_ (100 points)
-   Votre programme doit copier le binaire en mémoire avant l'exécution (50 points)

### Trouver la clé d'encryption et révéler la prophétie

-   Implémenter une méthode _brute force_ (250 points)
-   Bonne utilisation des adresses mémoire (50 points)
-   Trouver le bonne clé d'encryption et le message (200 points)

### Comprendre le fonctionnement du mythique émulateur 6502

Ici vous avez deux choix:

**Si vous faites les deux, le correcteur va en choisir un au hasard et l'autre sera ignoré**

> 1.  Écrire un document _markdown_ qui explique **EN PROFONDEUR** comment l'émulateur 6502 fonctionne au niveau technique et théorique.

-   Document clair et précis (450 points)
-   Document propre et facile à parcourir (50 points)

> 2.  Créer un simple programme qui calcule le 10e nombre de la suite de fibonacci en utilisant uniquement les opérations disponibles dans _fake6502.c_

-   Votre programme fonctionne (440 points)
-   Imprimer le 10e nombre dans la console en utilisant le _langage c_ (10 points)
-   Votre programme fonctionne sans modifications ni erreurs (25 points)
-   Le code est propre et commenté (25 points)

### Général (pour le programme principal)

-   Le code est propre et commenté (25 points)
-   Le projet fonctionne sans modifications ni problèmes (25 points)
-   Un Makefile permet de compiler et lancer le programme (50 points)

## Remise

Pour la remise de votre code, svp placer **TOUS** vos fichiers dans un ZIP et envoyer le tout à [info-externe.asetin@ift.ulaval.ca](mailto:info-externe.asetin@ift.ulaval.ca).
**N'oubliez pas d'indiquer nom!**
