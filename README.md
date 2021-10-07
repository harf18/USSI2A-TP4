# TP4 : Classes et Objets

### Objectifs
Manipuler les classes :

- Création de classe & instanciation d'objet
- Constucteurs
- Méthodes
- Attributs

### Prérequis
- Cloner le projet sur votre poste dans le repertoire de votre choix
- Ouvrir le projet TP4 :
	- Sur l'écran d'accueil d'IntelliJ, cliquer sur **New Project**
	- Selectionner **Java** dans la liste de gauche et **17** dans **Project SDK** puis Next
	- Ne rien cocher puis **Next**
	- Cliquer sur les **...** de **Project location** puis selectionner le dossier du projet tp4-xxxxx et cliquer sur **OK**
	- Cliquer sur **Finish**
	- Le projet s'ouvre

### Utilisation de GIT

- Créer une nouvelle branche **prenomNom**
- Faire **1 commit** par exercice (sauf exercice 0)
- Ouvrir **une seule** *pull request* sur github et **ne pas** la fermer/merger !!

----

### Exercice 1

- Compléter la classe **Exec** avec une méthode **main()** dans le package *net.lecnam.ussi2a.tp4*
- Modéliser un **Etudiant**. Pensez a respecter l'encapsulation (ajouter les accesseurs), ajouter le/les constructeurs qui vous paraissent judicieux.
	- Caractéristiques :
		- nom
		- prenom
		- Tableau de notes (maxi 50) (Bien utiliser un tableau, même si vous connaissez les ArrayList)
	- Actions :
		- getMoyenne() : Retourne la moyenne de l'eleve
		- ajouterNote(double) : ajoute une note à l'ensemble. Attention une note doit être entre 0 et 20.
		- une méthode pour retourner la description de l'étudiant (nom, prenom, moyenne) 
- Dans la méthode **main()** de **Exec**, créé un étudiant, ajouter lui des notes, afficher sa description

> Pensez a faire un commit !!

### Exercice 2
- Modéliser une classe **Division** (représente une classe d'étudiant mais le mot classe porte a confusion ici). Ajouter le/les constructeurs qui vous paraissent judicieux.
	- Caractéristiques :
		- nom
		- un ensemble d'étudiant (maxi 50) (Bien utiliser un tableau, même si vous connaissez les ArrayList)
	- Actions
		- getMoyenne() :  Retourne la moyenne de la division
		- getNombreEtudiant() : Indique le nombre d'étudiant de la division
		- ajouterEtudiant(Etudiant)
		- chercherEtudiant(String) : recherche dans le tableau le 1er etudiant dont le nom ou le prenom contiennent la chaine saisie. Retourne un objet etudiant ou null si aucun étudiant ne correspond.
		- listerEtudiant() : affiche a l'écran le nom de la division et la liste des description des étudiants;
- Dans la méthode **main()** de **Exec**, créé une division, ajouter lui des étudiants, ajouter des notes à ces étudiants, rechercher un étudiant, lister les étudiants de la classe.

> Pensez a faire un commit !!


### Exercice 3
- Modéliser une classe **Ecole**
	- Caractéristiques :
		- nom
		- un ensemble de divisions (maxi 50) (Bien utiliser un tableau, même si vous connaissez les ArrayList)
	- Actions
		- ajouterDivision(Division)
		- chercherEleve(String) : recherche sur le nom ou prénom de l'éleve, retourne un éleve et le nom de sa classe.
- Dans la méthode **main()** de **Exec**, créé une école, ajouter lui des classes, rechercher un étudiant

> Pensez a faire votre commit !!  
> Pensez à faire un push (```git push origin *prenomNom*```)  
> Si elle n'est pas déjà ouverte, ouvrez une pull request (branche **prenomNom** vers **master**) NE PAS LA FERMER/MERGER !


### Exercice 4 (bonus)
- Compléter la classe **Ecole** pour récupérer le meilleur élève de l'école

### Exercice 5 (bonus)
- Compléter la classe Etudiant avec une date de naissance
- Compléter les autres classes pour récupérer le plus vieil étudiant

### Exercice 6 (bonus)
- Compléter la classe Etudiant avec le genre (Masculin / Feminin)
- Compléter les autres classes pour faire une moyenne par genre

