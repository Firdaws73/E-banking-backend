 **Digital Banking**

**Introduction**

**Digital Banking** est une application Java EE qui illustre les concepts fondamentaux de la gestion bancaire numérique.
Son objectif est de fournir une plateforme complète pour la gestion des comptes bancaires, des clients, et des opérations financières. 
L'application met en avant deux types de comptes :

- **Comptes Courants** : Conçus pour les transactions bancaires quotidiennes (dépôts, retraits, virements) .
- **Comptes Épargnes** : Dédiés à l'épargne.

**Fonctionnalités Principales**

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

**Structure de la Base de Données**

La base de données est structurée autour de trois tables principales :

- **`customer`** : Informations sur les clients (ID, nom, données personnelles).
- **`bank_account`** : Détails des comptes bancaires (type, solde, date de création).
- **`account_operation`** : Enregistrement des transactions (type d’opération, montant, date).


2. **Création de la base de données** :
   ![image](https://github.com/user-attachments/assets/f9b6971c-7fa9-40f5-940b-13a6706528db)


3. **Ajoutez les configurations dans `application.properties`** :
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/digital_banking
   spring.datasource.username=your_username
   spring.datasource.password=your_password
   spring.jpa.hibernate.ddl-auto=update
   ```

4. **Lancez l'application** :
   ```bash
   mvn spring-boot:run
   ```

---

## **Utilisation**

### **Endpoints Clés**

1. **Gestion des Comptes** :
   - GET `/accounts` : Liste de tous les comptes.
   - GET `/accounts/{id}` : Détails d’un compte par ID.

2. **Gestion des Clients** :
   - POST `/customers` : Ajouter un client.
   - GET `/customers/{id}` : Récupérer un client.
   - PUT `/customers/{id}` : Modifier un client.
   - DELETE `/customers/{id}` : Supprimer un client.

3. **Opérations Bancaires** :
   - POST `/accounts/credit` : Créditer un compte.
   - POST `/accounts/debit` : Débiter un compte.

---

## **Exemples de Tests avec Postman**

1. **Ajouter un client** :
   - Méthode : POST  
   - URL : `http://localhost:8085/customers`  
   - Corps de la requête :
     ```json
     {
         "name": "John Doe",
         "email": "johndoe@example.com"
     }
     ```

2. **Récupérer un client** :
   - Méthode : GET  
   - URL : `http://localhost:8085/customers/1`

3. **Créditer un compte** :
   - Méthode : POST  
   - URL : `http://localhost:8085/accounts/credit`  
   - Corps de la requête :
     ```json
     {
         "accountId": "12345",
         "amount": 1000
     }
     ```

---

## **Capture d'Écran**

### Affichage des Comptes
![Affichage des comptes](https://github.com/user-attachments/assets/caae2d97-6ac5-40ee-8be9-b38c9bcba2e0)

### Gestion avec Postman
- **Ajout d’un client** :  
![Ajout d'un client](https://github.com/user-attachments/assets/f939bc3c-5f6f-4044-b0a9-e4a1abd9fc12)

---

## **Auteur**

**Firdawsse Ahchouche**  
Projet réalisé dans le cadre de l’apprentissage des concepts de Java EE et des systèmes bancaires numériques.

--- 

Avec ce fichier, vos utilisateurs auront une compréhension claire et complète de votre projet !
