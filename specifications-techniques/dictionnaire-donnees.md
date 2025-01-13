# Dictionnaire de Données

## Table : Users

| **Column Name**      | **Type**  | **Size** | **Description**                                  |
|----------------------|-----------|----------|--------------------------------------------------|
| user_uuid            | UUID      |          | Identifiant unique de l'utilisateur.             |
| user_pseudo          | VARCHAR   | 255      | Pseudonyme ou nom d'affichage de l'utilisateur.  |
| role_id              | NUMBER    |          | Identifiant du rôle attribué à l'utilisateur.    |
| role_name            | VARCHAR   | 100      | Nom descriptif du rôle attribué à l'utilisateur. |
| user_xp              | NUMBER    |          | Points d'expérience accumulés par l'utilisateur. |
| user_level           | NUMBER    |          | Niveau de l'utilisateur.                         |
| user_badges          | VARCHAR[] |          | Liste des badges obtenus par l'utilisateur.      |
| report_count         | VARCHAR   |          | Nombre de signalements reçus.                    |
| user_ranking         | NUMBER    |          | Classement de l'utilisateur.                     |

[... autres tables du dictionnaire de données ...] 