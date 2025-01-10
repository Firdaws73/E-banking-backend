 **Digital Banking**

**Introduction**

**Digital Banking** est une application Java EE qui illustre les concepts fondamentaux de la gestion bancaire numérique.
Son objectif est de fournir une plateforme complète pour la gestion des comptes bancaires, des clients, et des opérations financières. 
L'application met en avant deux types de comptes :

- **Comptes Courants** : Conçus pour les transactions bancaires quotidiennes (dépôts, retraits, virements) .
- **Comptes Épargnes** : Dédiés à l'épargne.

1.**Fonctionnalités Principales**

   1. **Gestion des Comptes Bancaires** :
   - Création de comptes courants et épargnes.
   - Affichage des détails d’un compte par son ID.
   - Affichage de la liste de tous les comptes bancaires.

   2. **Gestion des Clients** :
   - Ajout de nouveaux clients.
   - Modification des informations des clients.
   - Suppression de clients.
   - Récupération des détails d’un client par ID.

   3. **Gestion des Opérations Bancaires** :
   - Créditer ou débiter un compte.
   - Historique des opérations de chaque compte.

2.**Structure de la Base de Données**

La base de données est structurée autour de trois tables principales :

- **`customer`** : Informations sur les clients (ID, nom, données personnelles).
- **`bank_account`** : Détails des comptes bancaires (type, solde, date de création).
- **`account_operation`** : Enregistrement des transactions (type d’opération, montant, date).

3. **Création de la base de données** :
   
   ![image](https://github.com/user-attachments/assets/f9b6971c-7fa9-40f5-940b-13a6706528db)

5. **Création de la base de données** :

  **Gestion des Clients avec Postman**
  
   -**Ajout d’un client:**

![image](https://github.com/user-attachments/assets/e03f2fd3-db22-4bfe-817a-6d9221105252)

 -**Récupération d’un client par ID:**

![image](https://github.com/user-attachments/assets/85852001-2565-43ce-9f06-8710bbdad106)


-**Modification des informations d’un client:**

![image](https://github.com/user-attachments/assets/26392555-cbfd-4756-9fa6-ebe3a32ba93c)

-**Suppression d’un client:**

![image](https://github.com/user-attachments/assets/f812fd84-1aed-42c4-8af3-c1ec9377e329)


**Vérification de l'ajout  des clients  dans la base de données avec swagger-ui:**

![image](https://github.com/user-attachments/assets/46578d3e-9e68-4ddf-803b-a0d5fe6d9d07)

**Vérification de l'ajout  des clients  dans la base de données avec swagger-ui:**

![image](https://github.com/user-attachments/assets/4bb57b75-ddf8-4574-b65e-153eb77d1043)


---
**Conclusion:**
Le projet **Digital Banking** offre une solution intégrale pour la gestion des comptes bancaires, des clients et des transactions financières. S'appuyant sur des technologies telles que Java EE, Hibernate et Spring Boot. Doté de fonctionnalités comme la gestion des comptes courant et d'épargne, le suivi des opérations financières.

## **Auteur**
**Yahya Sernane**  
