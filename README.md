# Gestionnaire de Mots de Passe

Ce projet est un gestionnaire de mots de passe complet avec un backend Node.js et un frontend React. Il permet aux utilisateurs de stocker, récupérer, modifier et supprimer des mots de passe en toute sécurité.

## Technologies Utilisées

### Backend
- Node.js
- Express.js
- MongoDB avec Mongoose
- bcrypt pour le hachage des mots de passe

### Frontend
- React.js
- Axios pour les requêtes HTTP
- CSS pour le style

### Déploiement
- Docker
- Docker Compose

## Structure du Projet

Le projet est divisé en deux parties principales :

- `password-manager-backend/`: Contient le code du serveur backend
- `password-manager-frontend/`: Contient le code de l'application frontend React

## Lancement rapide avec Docker Compose

1. Clonez ce dépôt :
   ```
   git clone https://github.com/votre-nom/password-manager.git
   cd password-manager
   ```

2. Lancez l'application avec Docker Compose :
   ```
   docker-compose up --build
   ```

L'application sera accessible à l'adresse `http://localhost`.

## Installation manuelle (pour le développement)

1. Clonez ce dépôt :
   ```
   git clone https://github.com/Ewuly/password-manager.git
   cd password-manager
   ```

2. Installez les dépendances du backend :
   ```
   cd password-manager-backend
   npm install
   ```

3. Installez les dépendances du frontend :
   ```
   cd ../password-manager-frontend
   npm install
   ```

## Configuration

1. Backend :
   - Créez un fichier `.env` dans le dossier `password-manager-backend/` avec les variables suivantes :
     ```
     MONGODB_URI=votre_uri_mongodb
     PORT=5000
     ```

2. Frontend :
   - Si nécessaire, modifiez l'URL de l'API dans `src/App.js` et les autres composants qui font des appels API.

## Lancement manuel de l'Application

1. Démarrez le serveur backend :
   ```
   cd password-manager-backend
   npm start
   ```

2. Dans un nouveau terminal, démarrez l'application frontend :
   ```
   cd password-manager-frontend
   npm start
   ```

L'application sera accessible à l'adresse `http://localhost:3000`.

## Fonctionnalités

- Ajout de nouveaux mots de passe
- Modification des mots de passe existants
- Suppression des mots de passe

## Sécurité

- Les mots de passe sont hachés avec bcrypt avant d'être stockés dans la base de données.
- Le backend utilise des routes sécurisées pour gérer les opérations sur les mots de passe.

## Contribution

Les contributions sont les bienvenues ! N'hésitez pas à ouvrir une issue ou à soumettre une pull request.

## Licence

Ce projet est sous licence MIT. Voir le fichier `LICENSE` pour plus de détails.
