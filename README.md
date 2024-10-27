"# demoSpring" 

TP : SpringBoot & Thymeleaf

Etape 1 : Les dépendances Maven

•	Dans ce cas, nous nous appuierons sur spring-boot-starter-parent pour la gestion simple des dépendances, la gestion des versions et la configuration des plug-ins. Par conséquent, nous n'aurons pas besoin de spécifier les versions des dépendances du projet dans notre fichier pom.xml, sauf pour remplacer la version Java:
 
  
Figure 1 : Fichier « pom.xml ».

Etape 2 : Configuration application.properties

•	Nous allons utiliser la configuration standard
 
Figure 2 : Fichier « application.properties ».

 Etape 3 : La couche de domaine

•	Entité « User »
 
 
Figure 3 : Script de l’entité « User ».

Etape 4 : La couche de référentiel

•	Pour fournir à notre application des fonctionnalités CRUD de base sur les objets utilisateur, tout ce que nous devons faire est d'étendre l'interface CrudRepository :
 
Figure 4 : Script de l’interface « CrudRepository ».

Etape 5 : La couche contrôleur

 
 
 
Figure 5 : Script de la classe « UserController ».

 Etape 6 : La couche présentation

•	Fichier « add-user.html »
 
Figure 6 : Script de fichier « add-user.html ».

•	Fichier « update-user ».
 
 
Figure 7 : Script du fichier « update-user.html ».

•	Fichier « index.html »
 
 
 
Figure 7 : Script de fichier « index.html ».

Etape 7 : Exécution de l'application

•	Enfin, définissons le point d'entrée de l'application. Comme la plupart des applications Spring Boot, nous pouvons le faire avec une ancienne méthode main ():
 
Figure 8 : Script de la classe « DemoApplication ».
Resultats


