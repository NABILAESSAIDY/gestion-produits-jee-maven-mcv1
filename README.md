# 📦 GestionProduitsMVC1 – Application Web Java EE (MVC1)

## 📌 Description
GestionProduitsMVC1 est une application web développée en **Java EE (Servlets + JSP)** suivant le pattern **MVC1**.  
Elle permet la gestion complète de produits avec un système d’authentification et de contrôle d’accès basé sur les rôles (**ADMIN / USER**).

---

## 🚀 Fonctionnalités

### 🔐 Authentification
- Connexion utilisateur (login / mot de passe)
- Gestion de session
- Déconnexion sécurisée

### 👤 Gestion des rôles
- **ADMIN** : accès complet (CRUD produits)
- **USER** : consultation uniquement

### 📦 Gestion des produits (CRUD)
- Ajouter un produit (ADMIN)
- Modifier un produit (ADMIN)
- Supprimer un produit (ADMIN)
- Lister tous les produits (ADMIN / USER)
- Rechercher un produit par ID

### ⚠️ Gestion des erreurs
- Page personnalisée **403 (Accès interdit)**
- Page personnalisée **404 (Page introuvable)**
- Page d’erreur générique

---

## 🏗️ Architecture du projet
GestionProduitsMVC1/
├── pom.xml
└── src/main/
├── java/
│ ├── dao/ # Accès aux données (Produit)
│ ├── models/ # Modèles (Utilisateur, etc.)
│ ├── services/ # Logique métier + Auth
│ ├── filters/ # AuthFilter + RoleFilter
│ └── web/ # Servlets (contrôleurs)
└── webapp/
├── css/
├── WEB-INF/
│ └── views/ # JSP (vues)
└── index.jsp

---

## ⚙️ Technologies utilisées

- Java EE (Servlets, JSP)
- JSTL
- HTML / CSS
- Apache Tomcat
- Maven
- Architecture MVC1
