# TP3bis : Classes et Objets

### Objectifs
Manipuler les classes :

- Création de classe & instanciation d'objet
- Constucteurs
- Méthodes
- Attributs

### Prérequis
- Cloner le projet sur votre poste dans le repertoire de votre choix
- Ouvrir le projet USSI2A-TP3bis
    - *File > New > Project from Exiting Sources* (ou *Import Project* si vous êtes sur l'écran d'accueil)
    - Selectionner le dossier du projet
    - Selectionner **Create project from existing sources**
    - Conserver les informations (*Nom, Location, Format*)
    - IntelliJ détecte que c'est un projet Java
    - Aucune bibliothèque n'est integtée au projet
    - IntelliJ créé un modules USSI2A-TP3bis
    - Choisir JDK13, s'il n'est pas dans la liste, cliquer sur le <span style="color:green">**+**</span> et selectionner le dossier du JDK 13
    - Aucun Framework n'est detecté
    - Aller dans File > Project Structure et Choisir 13 **Project language level**

### Utilisation de GIT

- Créer une nouvelle branche **prenomNom**
- Faire **1 commit** par exercice (sauf exercice 0)
- Ouvrir **une seule** *pull request* sur github et **ne pas** la fermer/merger !!

----

### Exercice 1

- Compléter la classe **Exec** avec une méthode **main()** dans le package *net.lecnam.ussi2a.tp3bis*
- Modéliser un **Etudiant**. Pensez a respecter l'encapsulation (ajouter les accesseurs), ajouter le/les constructeurs qui vous paraissent judicieux.
	- Caractéristiques :
		- nom
		- prenom
		- Ensemble de notes (maxi 50)
	- Actions :
		- getMoyenne() : Retourne la moyenne de l'eleve
		- ajouterNote(double) : ajoute une note à l'ensemble
		- une méthode pour retourner la description de l'étudiant (nom, prenom, moyenne) 
- Dans la méthode **main()** de **Exec**, créé un étudiant, ajouter lui des notes, afficher sa description

> Pensez a faire un commit !!

### Exercice 2
- Modéliser une classe **Division **(représente une classe d'étudiant, une promotion). Ajouter le/les constructeurs qui vous paraissent judicieux.
	- Caractéristiques :
		- nom
		- un ensemble d'étudiant (maxi 50)
	- Actions
		- getMoyenne() :  Retourne la moyenne de la division
		- getNombreEtudiant() : Indique le nombre d'étudiant de la division
		- ajouterEtudiant(Etudiant)
		- chercherEtudiant(String) : recherche dans le tableau le 1er etudiant dont le nom ou le prenom contiennent la chaine saisie. Retourne un etudiant ou null si aucun étudiant ne correspond.
		- listerEtudiant() : affiche a l'écran le nom de la division et la liste des description des étudiants;
- Dans la méthode **main()** de **Exec**, créé une division, ajouter lui des étudiants, ajouter des notes à ces étudiants, rechercher un étudiant, lister les étudiants de la classe.

> Pensez a faire un commit !!


### Exercice 3
- Modéliser une classe **Ecole**
	- Caractéristiques :
		- nom
		- un ensemble de divisions (maxi 50)
	- Actions
		- ajouterDivision(Division)
		- chercherEleve(String) : recherche sur le nom ou prénom de l'éleve, retourne un éleve et le nom de sa classe.
- Dans la méthode **main()** de **Exec**, créé une école, ajouter lui des classes, rechercher un étudiant

> Pensez a faire votre commit !!  
> Pensez à faire un push (```git push origin *prenomNom*```)  
> Si elle n'est pas déjà ouverte, ouvrez une pull request (branche **prenomNom** vers **master**) NE PAS LA FERMER/MERGER !


### Exercice 4 (bonus)
- Compléter la classe **Ecole** pour récupérer le meilleur élève de l'école

### Exercice 4 (bonus)
- Compléter la classe Etudiant avec une date de naissance
- Compléter les autres classes pour récupérer le plus vieil étudiant

