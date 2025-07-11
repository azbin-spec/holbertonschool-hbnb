# Partie 3 : Backend Avancé avec Authentification et Base de Données 🚀

Bienvenue dans la troisième partie du projet HBnB. Ici, tu vas enrichir le backend en ajoutant des fonctionnalités d’authentification, de gestion des rôles, et d’intégration avec une base de données à l’aide de SQLAlchemy. Le développement se fera avec SQLite, tandis que MySQL sera prévu pour la production.

## Objectifs 🎯

- **🔐 Authentification & Autorisation** : Mettre en place une authentification via JWT et un système de permissions selon les rôles.
- **🗄️ Connexion à une Base de Données** : Remplacer le stockage en mémoire par SQLite pour le développement et préparer MySQL pour la production.
- **🛠️ Opérations CRUD** : Adapter les opérations CRUD pour qu’elles interagissent avec une base de données persistante.
- **📊 Modélisation** : Concevoir le schéma de base de données avec mermaid.js.
- **✅ Validation des Données** : Appliquer des validations et des contraintes au niveau des modèles.

## Compétences Acquises 📚

À la fin de cette section, tu seras capable de :

- 🔑 Mettre en place l’authentification via JWT et gérer les sessions utilisateurs.
- 🛡️ Appliquer un contrôle d’accès basé sur les rôles.
- 🗃️ Migrer le stockage vers SQLite avec SQLAlchemy et configurer MySQL pour l’environnement de production.
- 🖼️ Créer et illustrer un schéma relationnel avec mermaid.js.
- 🔒 Construire un backend sécurisé, robuste et extensible.

## Contexte du Projet 🏗️

Jusqu’à maintenant, le backend fonctionnait avec un système de stockage en mémoire. Dans cette partie, tu passeras à SQLite pour le développement tout en préparant le projet à un déploiement en MySQL. L’authentification par jeton JWT et le contrôle des accès selon les rôles feront aussi leur apparition.

## Ressources Utiles 📖

- [🔐 Authentification JWT avec Flask-JWT-Extended](https://flask-jwt-extended.readthedocs.io/en/stable/)
- [🗄️ ORM SQLAlchemy](https://docs.sqlalchemy.org/en/14/)
- [🗃️ Documentation SQLite](https://www.sqlite.org/docs.html)
- [🌐 Guide Flask Officiel](https://flask.palletsprojects.com/en/2.0.x/)
- [📊 Mermaid.js pour la modélisation](https://mermaid-js.github.io/mermaid/#/)

## Étapes du Développement 🗂️

1. **🔒 Mise à jour du modèle utilisateur** : Gestion des mots de passe avec bcrypt2.
2. **🔑 Authentification avec JWT** : Sécurisation de l’API via des tokens JWT.
3. **🛡️ Mise en place des rôles** : Définition des droits d’accès en fonction des utilisateurs.
4. **🗃️ Passage à SQLite** : Utilisation de SQLite en environnement de développement.
5. **🗄️ Mapping des entités** : Utilisation de SQLAlchemy pour définir les modèles et les relations.
6. **🗄️ Préparation à MySQL** : Configuration de l’environnement de production avec MySQL.
7. **📊 Conception du schéma** : Création de diagrammes ER avec mermaid.js.

À la fin de cette étape, ton backend sera sécurisé, prêt pour la production, et capable de gérer de manière fiable des données persistantes avec une logique d’accès par rôle.
