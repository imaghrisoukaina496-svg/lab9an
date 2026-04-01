📚 Projet Web Service PHP + Android
📝 Description
Ce projet consiste à créer une application mobile Android qui communique avec un Web Service PHP pour gérer des étudiants. L'application permet d'ajouter et de consulter des étudiants stockés dans une base de données MySQL via des requêtes HTTP.

🛠️ Technologies utilisées

Base de données : MySQL (XAMPP)
Backend : PHP (PDO)
Frontend Mobile : Android (Java)
Librairies Android : Volley (requêtes HTTP), Gson (parsing JSON)
Outils de test : Postman


🗄️ Partie 1 — Base de données MySQL

Base de données : school1
Table : Etudiant (id, nom, prenom, ville, sexe)


🌐 Partie 2 — Web Service PHP
Structure du projet
PhpProject9/
├── classes/        → Etudiant.php
├── connexion/      → Connexion.php
├── dao/            → IDao.php
├── service/        → EtudiantService.php
└── ws/
    ├── loadEtudiant.php
    └── createEtudiant.php
Test GET — Charger les étudiants

![WhatsApp Image 2026-04-01 at 12 44 48 AM](https://github.com/user-attachments/assets/1aa0202f-b081-4f7a-91e1-62b410d37826)
URL : http://localhost/PhpProject9/ws/loadEtudiant.php
Méthode : GET
Réponse :
```
json[
  {"id":"1","nom":"Lachgar","prenom":"Mohamed","ville":"Rabat","sexe":"homme"},
  {"id":"2","nom":"Safi","prenom":"Amine","ville":"Marrakech","sexe":"homme"}
]
```
Test POST — Ajouter un étudiant
![WhatsApp Image 2026-04-01 at 12 51 48 AM](https://github.com/user-attachments/assets/1466d469-1b2d-49e3-8e91-2eed58736486)

URL : http://localhost/PhpProject9/ws/createEtudiant.php
Méthode : POST
Body (x-www-form-urlencoded)

📱 Partie 3 — Application Android
Fonctionnalités

Formulaire d'ajout d'un étudiant (Nom, Prénom, Ville, Sexe)
Envoi des données via Volley (POST)
Parsing de la réponse JSON via Gson
Affichage des résultats dans Logcat
🎥 Vidéo démonstrative


⚙️ Instructions d'installation
Prérequis

XAMPP (Apache + MySQL)
Android Studio
Postman

Étapes

Démarrer XAMPP et activer Apache + MySQL
Importer la base de données school1 via phpMyAdmin
Copier le dossier PhpProject9 dans C:\xampp\htdocs\
Ouvrir le projet Android dans Android Studio
Lancer l'émulateur et exécuter l'application


👨‍💻 Auteur

Soukaina Imaghri
