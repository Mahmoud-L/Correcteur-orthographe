# Correcteur d'orthographe

Travail de Jerome Emery, Dereck Piche, Mahmoud Labidi

## Utilisation

Cette application permet à un utilisateur d'entrer du texte ou bien d'importer un fichier texte depuis son ordinateur, et de corriger celui-ci. Pour ce faire, on importe un dictionnaire (fichier texte), et ensuite on entre le texte à corriger. Appuyer sur le bouton "Corriger" compare chaque mot entré aux mots du dictionnaire et surligne en rouge les mots incorrects. Il est possible de "right click" sur un mot surligné en rouge pour faire apparaitre une liste de 5 mots similaires et de remplacer le mot incorrect par un de ceux proposés. Finalement, l'utilisateur peut sauvegarder le document corrigé en tant que fichier texte. 


## Fonctionnement du code

Lorsque le dictionnaire est importé, il est stocké dans un hashtable qui, quant à lui, est contenu dans un objet de type dictionnaire. Cette classe contient des fonctions pour remplir son attribut hashtable, verifier si un mot appartient au dictionnaire et trouver des mots similiares à un mot incorrect. Le modèle MVC, geré par les classes modèle, contrôle et vue, assure la gestion entre l'interface graphique et les fonctions accomplies par le dictionnaire. En itérant a travers chaque mot du textArea, on crée des objets MotIncorrect si le mot n'appartient pas au dictionnaire. Cet objet contient le mot, son index dans le text area ainsi qu'une ArrayList avec des recommandations de mots. On utilise cet objet pour ensuite surligner les mauvais mots et recommander des mots. 




