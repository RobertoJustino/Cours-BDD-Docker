# Cours-BDD-Docker

## Modélisations de bases NoSQL

### Documents Structurés : XML, JSON (http://b3d.bdpedia.fr/files/sldocstruct.pdf)

  Qu'est ce qu'un document ?

* une valeur atomique (un entier, une chaîne de caractères); 
* une paire clé-valeur; 
* un tableau de valeurs est un document; 
* un agrégat de paires clé-valeur est un document;  

  et de manière générale, toute composition des possibilités précédentes (un tableau d’agrégats de
paires clé-valeur par exemple) est un document.  

  Notions essentielles
* Les données sont auto-décrites. Le contenu vient avec sa propre description.
* Structures riches. Le contenu se décrit avec des listes, des enregistrements imbriqués,
des ensembles.
* Typage flexible. Les données peuvent être typées (“c’est un entier”), et/ou structurées
(“cette partie du graphe doit avoir telle forme”).
* Sérialisation. Structure et contenu doivent pouvoir être transformés ensemble en une
chaîne de caractères autonome.

  La construction récursive d’un document structuré implique une représentation sous forme d’un arbre dans
lequel on représente à la fois le contenu (les valeurs) et la structure (les noms des clés et l’imbrication des
constructeurs élémentaires).  

  Modélisation arborescente : arbre dans lequel les étiquettes sont sur les arêtes et les valeurs sur les feuilles.  
  On peut aussi représenter la structure et les valeurs comme des noeuds (XML)

#### Sérialisation des documents structurés 

La sérialisation désigne la capacité à coder un document sous la forme d’une séquence d’octets qui peut
« voyager » sans dégradation sur le réseau, une propriété essentielle dans le cadre d’un système distribué.

#### JSON 

* Javascript Object Notation
* Initialement créé pour la sérialisation et l’échange d’objets JavaScript ;
* Langage pour l’échange de données semi-structurées (et éventuellement structurées) ;
* Format texte indépendant du language de programmation utilisé pour le manipuler.  
  Utilisation première : échange de données dans un environnement Web  
  Extension : sérialisation et stockage de données


