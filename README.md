#🏠 HBnB - AirBnB Clone
🏠 App de Location de Logements

Une application **full-stack** inspirée du concept d'Airbnb, où les utilisateurs peuvent rechercher des logements, consulter leurs détails ainsi que laisser des avis.

## 📁 Architecture du Projet

```
part4/
├── hbnb_backend/           # Serveur Flask côté backend
│   ├── app/
│   │   ├── api/           # Endpoints REST
│   │   ├── models/        # Modèle de données
│   │   ├── services/      # Logique métier
│   │   └── utils/         # Scripts utilitaires
│   └── run.py             # Point de départ du backend
└── hbnb_frontend/         # Ressources côté frontend
    ├── css/               # Styles
    ├── js/                # Scripts JS
    ├── images/            # Images
    └── templates/         # Fichiers HTML
```

## ✨ Fonctionnalités

- 👤 Authentification des utilisateurs (connexion / déconnexion)  
- 🔍 Exploration des logements disponibles  
- 🗺️ Affichage détaillé des propriétés  
- 💵 Tri des logements par prix  
- 🌟 Ajout et consultation des avis  

## ⚡️ Prérequis

- 🐍 Python 3.8 ou supérieur
- 📦 `pip` (gestionnaire de paquets Python)
- 🐳 Serveur MySQL opérationnel
- 🌐 Navigateur Web moderne

## 🚀 Installation

1️⃣ **Récupérer le dépôt** :
```bash
git clone https://github.com/SoliraZ/holbertonschool-hbnb
cd holbertonschool-hbnb/part4
```

2️⃣ **Préparer l’environnement backend** :
```bash
cd hbnb_backend
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

3️⃣ **Configurer la base de données** :
- Créez une base de données nommée `hbnb_dev`
- Paramétrez vos accès MySQL dans `hbnb_backend/app/config.py`

4️⃣ **Préparation du schéma de la base** :
```bash
python3 -m app.utils.db_setup
```

## 🏁 Lancement de l’application

Pour démarrer rapidement le frontend ainsi que le backend :
```bash
cd part4
./start_servers.sh
```

Ce script :
1. Lance le backend (Flask) à l’adresse `http://127.0.0.1:5000`
2. Ouvre le frontend à `http://localhost:8000`  
3. Ouvre automatiquement le site dans le navigateur par défaut

### Lancement manuel

#### Backend
```bash
cd hbnb_backend
source venv/bin/activate    # Windows : venv\Scripts\activate
python3 run.py
```

#### Frontend
- Ouvrir le fichier `part4/hbnb_frontend/index.html` directement
- Ou lancer un serveur local :
```bash
cd hbnb_frontend
python3 -m http.server 8000
```

Rendez‑vous alors sur `http://localhost:8000` !

## 🔗 Endpoints de l'API

- `POST /api/v1/auth/login` — Connexion utilisateur
- `GET /api/v1/places` — Liste des logements
- `GET /api/v1/places/<place_id>` — Détails d’un logement
- `GET /api/v1/places/<place_id>/reviews` — Avis associés
- `POST /api/v1/reviews` — Ajout d’un nouvel avis

## 📱 Utilisation

### 👁️ Consulter des logements
Parcourir la page d’accueil pour découvrir toutes les offres disponibles, appliquer des filtres de prix et cliquer sur **Voir détails** pour en savoir plus.

### 🗺️ Détails d'un logement
Consulter la fiche complète du lieu, découvrir les équipements, la localisation ainsi que les avis déjà publiés.  
Pour laisser un commentaire, connectez‑vous.

### 👤 Authentification
Se connecter pour accéder à toutes les fonctionnalités du site, laisser des avis et gérer son compte.

## ⚡️ Dépannage

- Le serveur backend ne répond pas :
  - Vérifier que MySQL est actif
  - Confirmer que vos accès en base (`config.py`) sont valides
  - S’assurer que toutes les dépendances sont installées
- Le site frontend ne charge pas :
  - Consulter la console du navigateur
  - Confirmer que le backend est actif
  - Effacer le cache du navigateur

## 📄 Licence

Ce projet est publié sous licence MIT — voir le fichier `LICENSE` pour plus d'informations.
