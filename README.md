**Introduction**
Le projet Digital Banking est une application Java EE (JEE) qui illustre les concepts fondamentaux de la gestion bancaire numérique. L'objectif principal est de développer une plateforme permettant de gérer les comptes bancaires de manière efficace, en mettant l'accent sur deux types de comptes :

Comptes Courants : Permettent des opérations bancaires quotidiennes telles que les dépôts, les retraits, et les virements avec une autorisation de découvert.
Comptes Épargnes : Destinés à l'épargne, offrant des taux d'intérêt mais sans autorisation de découvert.

**Création de la ase de données MySQL:**
![image](https://github.com/user-attachments/assets/81310477-5ebb-4c64-b4c8-eb9a8ef17ff8)

La base de données du projet Digital Banking est structurée autour de trois tables principales :
customer : Contient les informations sur les clients, tels que leur identifiant, leur nom, et d'autres données personnelles.
bank_account : Gère les comptes bancaires associés aux clients, avec des détails comme le type de compte (courant ou épargne), le solde, et la date de création.
account_operation : Enregistre les opérations effectuées sur les comptes bancaires (crédit, débit, transfert), y compris les montants et les dates des transactions.
Ces tables utilisent le moteur de stockage InnoDB et le collationnement ut

![image](https://github.com/user-attachments/assets/b2b48630-8b89-4b1d-86e0-f9143efb17ab)

**On affiche un compte par l'id:**
![image](https://github.com/user-attachments/assets/caae2d97-6ac5-40ee-8be9-b38c9bcba2e0)

**Affiche de tous les comptes bancaires avec /accounts:**
![image](https://github.com/user-attachments/assets/86ef1d37-36ee-4722-8a09-604920355d6f)

**Test avec postamn:**
-Ajout d'un custumor.
![image](https://github.com/user-attachments/assets/f939bc3c-5f6f-4044-b0a9-e4a1abd9fc12)

-Récuperation d'un custumor par id.
![image](https://github.com/user-attachments/assets/8c0bf528-95b6-4ee1-b49f-3a92540468be)

-Modification d'un custumor.

![image](https://github.com/user-attachments/assets/6683e875-d2fc-48f2-857c-a326af7aed4a)

-Suppresion d'un customer
![image](https://github.com/user-attachments/assets/9b460e53-f041-43f6-b388-28e6b2103706)

**On change les données d'un compte :**
L'URL de l'API à appeler : http://localhost:8085/accounts/credit.

![image](https://github.com/user-attachments/assets/fba73ca9-c595-4797-8947-001bec1d477c)
![image](https://github.com/user-attachments/assets/94a51997-616b-4f26-bb42-dbfa683bce94)

**Conclusion**
Le projet Digital Banking illustre les concepts fondamentaux de la gestion bancaire numérique en offrant une solution complète et fonctionnelle pour la gestion des comptes bancaires, des clients, et des opérations financières. Grâce à l'utilisation des technologies robustes telles que Java EE, Hibernate, et Spring Boot, ce projet met en avant les meilleures pratiques de développement d'applications web.

Les principales fonctionnalités, comme la gestion des comptes courants et des comptes épargnes, les opérations de crédit et de débit, ainsi que le suivi des historiques, permettent d'expérimenter une solution proche des systèmes bancaires réels. De plus, l'intégration d'outils comme H2 Database pour le stockage des données et Swagger/OpenAPI pour la documentation des API garantit un environnement de développement moderne et bien structuré.


**Auteur:Firdawsse Ahchouche**








