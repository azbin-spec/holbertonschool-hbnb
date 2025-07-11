# 📘 HBNB Project - Partie 2 : Schéma de Base de Données

## 📚 À propos

Ce fichier fournit une documentation structurée autour du schéma de base de données utilisé dans le projet HBnB. Il présente les différentes entités, leurs champs, les types de relations entre elles, et les choix de conception réalisés. L’objectif est d’assurer une organisation cohérente pour gérer les utilisateurs, les hébergements, les avis, et les services associés à chaque logement.

---

## 📊 Diagramme Entité-Relation (ERD)

Ci-dessous, le diagramme illustre la structure de la base de données avec toutes les entités principales et leurs relations :

```mermaid
erDiagram
    USERS {
        string id
        string first_name
        string last_name
        string email
        string password
        bool is_admin
    }

    PLACES {
        string id
        string title
        text description
        decimal price
        float latitude
        float longitude
        string user_id
    }

    REVIEWS {
        string id
        text text
        int rating
        string user_id
        string place_id
    }

    AMENITIES {
        string id
        string name
    }

    PLACES_AMENITIES {
        string place_id
        string amenity_id
    }

    USERS ||--o{ PLACES : "owns"
    USERS ||--o{ REVIEWS : "writes"
    PLACES ||--o{ REVIEWS : "has"
    PLACES }o--o{ AMENITIES : "has"
    PLACES_AMENITIES }o--|| PLACES : "references"
    PLACES_AMENITIES }o--|| AMENITIES : "references"
