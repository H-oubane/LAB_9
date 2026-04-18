# LAB 9 Android – Web Service PHP + Volley + Gson

Application Android qui communique avec un Web Service PHP pour gérer une liste d'étudiants dans une base de données MySQL.

## Objectif
Créer une application Android qui :
- Envoie des données (nom, prénom, ville, sexe) vers un Web Service PHP
- Reçoit une réponse JSON du serveur
- Affiche les résultats dans Logcat

## Architecture du projet

### Partie 1 : Base de données MySQL (XAMPP)
- Base : `school1`
- Table : `etudiant (id, nom, prenom, ville, sexe)`

### phpMyAdmin (base de données)
<img width="578" height="234" alt="image" src="https://github.com/user-attachments/assets/158566ee-8b2b-409c-b2a5-3c807cb29469" />



### Partie 2 : Web Service PHP
- `createEtudiant.php` → ajoute un étudiant (POST)
- `loadEtudiant.php` → retourne la liste des étudiants (GET)

### Test Postman
<img width="1265" height="722" alt="image" src="https://github.com/user-attachments/assets/7bf03c31-5880-461c-9308-7eedddc04797" />



### Partie 3 : Application Android
- `AddEtudiant.java` → interface d'ajout
- `Etudiant.java` → modèle de données
- Volley → requêtes HTTP
- Gson → parsing JSON

### capture video
https://github.com/user-attachments/assets/472c31e8-d801-4d90-83b6-9e80734d72ed


###  Logcat (réponse JSON)
<img width="1326" height="680" alt="image" src="https://github.com/user-attachments/assets/0880792c-9a97-4a01-852d-7d3c5db9e30c" />


### phpMyAdmin (base de données)
<img width="1062" height="531" alt="image" src="https://github.com/user-attachments/assets/5211c206-36bf-4d5f-a55d-5597f1172012" />



## Structure du projet

### PHP (dans `C:\xampp\htdocs\projet\`)
projet/

├── connexion/

     └── Connexion.php
   
├── classes/

     └── Etudiant.php
   
├── dao/

     └── IDao.php
   
├── service/

     └── EtudiantService.php
   
└── ws/

├── createEtudiant.php

└── loadEtudiant.php



### Android
app/src/main/java/com/example/projetws/

├── AddEtudiant.java

└── beans/
  
    └── Etudiant.java

app/src/main/res/layout/

    └── activity_add_etudiant.xml

app/src/main/res/xml/

    └── network_security_config.xml


## Scan mobsf
<img width="1362" height="676" alt="image" src="https://github.com/user-attachments/assets/577c6ee0-dbfc-49b2-89b6-12507ced204f" />


## Technologies utilisées

### Backend (Serveur)
- XAMPP (Apache + MySQL)
- PHP 8
- PDO
- JSON

### Frontend (Android)
- Android Studio
- Java
- Volley (requêtes HTTP)
- Gson (parsing JSON)
- API minimum : 24 (Android 7.0)


## Auteur
H-oubane
