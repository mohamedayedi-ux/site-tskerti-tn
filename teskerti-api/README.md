# TESKERTI API -- Backend Technique

L'API de TESKERTI est un moteur de billetterie robuste concu pour la performance, la securite et l'extensibilite.

## Architecture System

- Pattern : MVC leger avec Front Controller (public/index.php).
- Core : Router custom, gestion unifiee des requetes/reponses (JSON-first).

## Securite avancee

- Authentification : JWT (JSON Web Tokens) avec Rotation des Refresh Tokens. Chaque renouvellement de session revoque l'ancien token.
- Mots de passe : Hachage securise via Argon2id.
- Cors & Headers : Configuration CORS granulaire et headers de securite.

## Integrite des Donnees

- Transactions Atomiques : Toutes les operations sensibles (Paiement + Confirmation) sont enveloppees dans des transactions SQL.
- Verrouillage des Sieges : Utilisation de SELECT ... FOR UPDATE pour seriliser les reservations.
- Timeout automatique : Les reservations pending expirent apres 15 minutes.

## Liste des Endpoints (v1)

### Authentification
- POST /auth/register : Creation de compte.
- POST /auth/login : Connexion.
- POST /auth/refresh : Rotation des tokens.
- GET /auth/me : Profil de l'utilisateur.

### Films & Seances
- GET /movies : Liste des films.
- GET /movies/{id} : Details d'un film.
- GET /movies/{id}/sessions : Seances pour un film.
- GET /cinemas : Liste des cinemas.
- GET /sessions/{id}/seats : Plan de salle et disponibilite.

### Reservations & Paiements
- POST /bookings : Creer une reservation temporaire (15 min).
- POST /payments/process : Traitement du paiement Visa.

## Installation

Propulse par PHP 8.2+ et passion pour le code propre.
