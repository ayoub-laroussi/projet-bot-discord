# Role-Based Access Control (RBAC)

## Rôles et Permissions

### 1. Nouvel Arrivant
- **Permissions de lecture** :
  - Lecture limitée des ressources
  - Lecture des messages dans les canaux publics
- **Restrictions** :
  - Pas de partage de ressources
  - Pas de vote sur les ressources
  - Pas de signalement

### 2. Membre Standard
- **Permissions de base** :
  - Lecture complète des ressources
  - Création de ressources
  - Modification de ses propres ressources
  - Suppression de ses propres ressources
- **Permissions d'interaction** :
  - Vote "utile"/"inutile" sur les ressources
  - Signalement de contenu inapproprié
  - Participation au système de gamification
  - Ajout de tags aux ressources

### 3. Modérateur
- **Toutes les permissions des membres standards**
- **Permissions de modération** :
  - Modification de toutes les ressources
  - Suppression de tout contenu
  - Gestion des signalements
  - Accès aux logs de modération
- **Permissions d'administration** :
  - Accès à l'interface web de gestion
  - Visualisation des statistiques
  - Gestion des utilisateurs

### 4. Administrateur
- **Toutes les permissions des modérateurs**
- **Permissions système** :
  - Gestion complète du bot (démarrage/arrêt)
  - Configuration du système
  - Gestion des rôles
  - Gestion de la liste noire
- **Permissions avancées** :
  - Modification des seuils de signalement
  - Gestion des catégories de signalement
  - Configuration des règles de sécurité

## Matrice des Permissions

| Permission                    | Nouvel Arrivant | Membre Standard | Modérateur | Administrateur |
|------------------------------|-----------------|-----------------|------------|----------------|
| Lecture des ressources       | Limitée         | ✓              | ✓          | ✓              |
| Création de ressources       | ✗              | ✓              | ✓          | ✓              |
| Modification ressources      | ✗              | Propres         | Toutes     | Toutes         |
| Suppression ressources       | ✗              | Propres         | Toutes     | Toutes         |
| Vote sur ressources          | ✗              | ✓              | ✓          | ✓              |
| Signalement                  | ✗              | ✓              | ✓          | ✓              |
| Accès interface web          | ✗              | ✗              | ✓          | ✓              |
| Gestion du bot              | ✗              | ✗              | ✗          | ✓              |
| Configuration système        | ✗              | ✗              | ✗          | ✓              | 