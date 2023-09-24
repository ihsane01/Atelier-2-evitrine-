Atelier 2
Mise en place d’une Vitrine online basée sur le Framework Laravel



Objectif :
*  l’objectif principal de cet atelier est la mise en place d’une application web sous frome d’une vitrine virtuelle online, en utilisant le Framework Laravel, l’application sera composée de deux parties, une première « back end » qui va servir pour la gestion interne du site, et une deuxième partie « Front end » sous forme d’une vitrine pour proposer les articles onlines.
Réalisation :
1.	Développer le digramme de classe équivalant à cette application web :
![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/c9f3cb0a-f6a9-4f90-be40-42d1f393775a)



2.	Créer un projet Laravel « evitrine » en utilisant la ligne decommande équivalente :![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/00ee1b27-55bf-4375-909b-2bfb3b2ce553)

3.	Créer les fichiers migrations selon les classes du diagramme de classe déjà établie :
	Création du fichier migration de la table catégories :
![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/6ea886a0-3316-41e4-87fc-716f39482cbd)

	Création du fichier migration de la table articles :
  ![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/e4d17527-6e89-4d35-b026-0127a45ecce1)

	Création du fichier migration de la table panier :

![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/a5deec18-7bf1-498f-8ce2-dd362346f7b0)

4.	Lancer une migration vers une BDD MySQL :
 ![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/a05ecf7f-639f-431f-95b3-95dec6c647f6)

5.	les classes modèles en se basant sur le digramme de classe :
    ![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/72ecac70-2fba-4313-9928-8db5fed3ec06)

![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/371d12a2-2d5a-4bc6-a9ca-ba3adf3cfad3)
![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/d7fd47c4-cc4a-4b29-a28b-ad1a04ef4b1c)
![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/7183732f-386e-4f6a-8a75-a415404f84c0)

![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/3afbd505-4542-4f9d-be78-b2f3f8728c68)

6.	Créer les Contrôleurs de chaque sous gestions de l’application, pour les deux parties back end et front end : 

![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/e3b4424b-5bd7-4ffa-8718-dd660427c8ae)

![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/02250683-79da-4b31-a64c-73bdd9993237)

7.	Créer deux Templates « backend.blade.php, frontend.blade.php » basées sur le moteur Blade, une pour la partie back end et autre pour front end.

 	PARTIE COMMUN ENTRE ADMIN ET SIMPLE USER : 
o	 welcome page :

![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/75f55cbb-9cf1-48aa-949a-ea40ce922714)


o	Login page : 
![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/27f45eb5-a819-44dc-843a-26d29df5027b)

o	Login comme un admin :
![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/47d7af48-8fe8-4dcd-aa24-d87da9c4c480)

 	HOME PAGE DE L’ADMIN 
 
o	Le Button Admin view apparait à l’admin seulement pour la gestion de tous qui est en relation avec les opérations de classe admin que j’ai déjà cité en haut et qui nous emmène à la partie backend. 


	PARTIE BACKEND : 

 	LA TEMPLATE BACKEND.BLADE.PHP : ![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/1eb9c314-c075-48f7-abc7-c38ef6f3f181)

 
8. les interfaces web qui héritent du Template « backend.blade.php : 

•	Le Click 1 de la partie backend :

o	C’est le Button qui nous emmène à la partie de gestion des articles :
 ![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/d03e0115-5f50-4527-859e-4a09613d88d5)

o	Le Button Add new Product pour ajouter des nouveaux articles à la base de données 

![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/ea812824-b4c3-426f-830b-ded2c5debff8)


•	Le Click 2 de la partie backend :
-	C’est le Button qui nous emmène à la partie de gestion des catégories 
Button Add new Catégorie pour ajouter des nouvelles catégories. 

![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/166c3164-ee5a-49b7-822e-ba4023ac1ddb)


9.	Développer une interface principale de la vitrine basée sur le fichier Template « frontend.blade.php » :
10.	
o	Login comme un simple user :
![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/aaf72f57-771f-46d8-84fa-0cf2fd8098fc)

o	Le Button 1 :
-	Catégorie Homme : nous emmène à la vue qui nous affiche les produits qui concernent les hommes avec Un système de pagination, tel que l’utilisateur peut acheter un article avec le clic sur ajouter au panier avec la détermination de la quantité :
-	

 ![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/a703b8cb-4ac2-4e07-840f-b2c2eeceee35)



o	Le Button 2 
-	Catégorie Femme : nous emmène à la vue qui nous affiche les produits qui concernent les femmes avec Un système de pagination, tel que l’utilisateur peut acheter un article avec le click sur ajouter au panier avec la détermination de la quantité![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/c6232cd5-6928-4f23-bc1b-2d731a071d40)



o	Le Button 3 :
Panier : affiche le panier d’user contenant les produits qui ajoutent l’utilisateur à son panier, avec totale calculé, et il peut supprimer les produits avec le click supprimer![image](https://github.com/ihsane01/Atelier-2-evitrine-/assets/101754865/e9817264-8884-48cc-a2c1-7c33fa50ee46)

