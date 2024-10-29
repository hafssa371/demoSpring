"# demoSpring" 

TP : SpringBoot & Thymeleaf

Etape 1 : Les dépendances Maven

•	Dans ce cas, nous nous appuierons sur spring-boot-starter-parent pour la gestion simple des dépendances, la gestion des versions et la configuration des plug-ins. Par conséquent, nous n'aurons pas besoin de spécifier les versions des dépendances du projet dans notre fichier pom.xml, sauf pour remplacer la version Java:
 ![image](https://github.com/user-attachments/assets/4352db92-8489-4dd3-9892-a4ad3fa6befe)
 ![image](https://github.com/user-attachments/assets/dd8d88ae-b84e-43ef-9876-92690a906203)
 ![image](https://github.com/user-attachments/assets/72110ba0-3df3-490d-9125-132932d87013)
 ![image](https://github.com/user-attachments/assets/22e35476-88ae-421f-b45e-a32fcf4f3852)
 
Figure 1 : Fichier « pom.xml ».


Etape 2 : Configuration application.properties

•	Nous allons utiliser la configuration standard

 ![image](https://github.com/user-attachments/assets/41a07867-3f74-4344-a23c-dca10283f3c2)

Figure 2 : Fichier « application.properties ».

 Etape 3 : La couche de domaine

•	Entité « User »
 
 ![image](https://github.com/user-attachments/assets/5b52510c-9982-4355-9801-ff579c1e27f8)
 ![image](https://github.com/user-attachments/assets/b4f91e3e-61cc-40a7-be25-8488b11627e5)

Figure 3 : Script de l’entité « User ».

Etape 4 : La couche de référentiel

•	Pour fournir à notre application des fonctionnalités CRUD de base sur les objets utilisateur, tout ce que nous devons faire est d'étendre l'interface CrudRepository :

 ![image](https://github.com/user-attachments/assets/cb1c8531-88c3-40e2-bb63-d5dc9e44025c)

Figure 4 : Script de l’interface « CrudRepository ».

Etape 5 : La couche contrôleur

 
 ![image](https://github.com/user-attachments/assets/a78d41b7-6955-4720-ae64-85dc1e3925f6)
 ![image](https://github.com/user-attachments/assets/a1f48eb4-7e10-41b6-9c7f-be0b2a961052)
 ![image](https://github.com/user-attachments/assets/91d7d003-2d8c-4764-b145-05011fa1e233)
 
Figure 5 : Script de la classe « UserController ».

 Etape 6 : La couche présentation

•	Fichier « add-user.html »
![image](https://github.com/user-attachments/assets/c693c70d-4d33-4784-91d4-09dcfc9458a4)

Figure 6 : Script de fichier « add-user.html ».

•	Fichier « update-user ».
 ![image](https://github.com/user-attachments/assets/3617a41c-a031-48ba-84d2-21e1761fbeed)
 ![image](https://github.com/user-attachments/assets/fc974a6f-438c-4d2f-a580-e2f92a6380f9)

Figure 7 : Script du fichier « update-user.html ».

•	Fichier « index.html »
 
 ![image](https://github.com/user-attachments/assets/35d2f15b-e2db-4920-81fd-fbd7ca65dd25)
 ![image](https://github.com/user-attachments/assets/caf4e666-96e7-49b1-b7f6-7ab3d38c5a38)
 ![image](https://github.com/user-attachments/assets/0a671682-8cd5-4515-83c4-ba91e6ca2c60)

Figure 7 : Script de fichier « index.html ».

Etape 7 : Exécution de l'application

•	Enfin, définissons le point d'entrée de l'application. Comme la plupart des applications Spring Boot, nous pouvons le faire avec une ancienne méthode main ():
 ![image](https://github.com/user-attachments/assets/3505fae8-bd82-4d84-90a0-819df9a9cf03)
Figure 8 : Script de la classe « DemoApplication ».


Resultats

![WhatsApp Image 2024-10-27 à 13 58 08_7231396f](https://github.com/user-attachments/assets/bdb6af4d-c6d3-4e63-8ada-1e1f72e1973e)
Figure 9 : Résultat de test.

![image](https://github.com/user-attachments/assets/d3b487b6-5124-4f24-8091-e7bd447755c2)

Figure 10 : Résultat de test.

![image](https://github.com/user-attachments/assets/c875c177-fbdd-4a21-928d-47e643a971bc)

Figure 11 : Résultat de test.

![WhatsApp Image 2024-10-29 à 13 55 33_78095468](https://github.com/user-attachments/assets/2d14e00d-20eb-4cef-b5d6-874c7b2cfbed)

Figure 12 : Résultat de test.

![image](https://github.com/user-attachments/assets/07052a38-59a5-46e5-9502-e82d51c62331)

Figure 13 : Résultat de test.









