# TESKERTI SPA -- Frontend Moderne

Le frontend de TESKERTI est une Single Page Application (SPA) ultra-rapide developpee en Vanilla JavaScript (ES Modules).

## Concept & Design

- Esthetique : Identite visuelle "Noir Charbon & Or Electrique" pour une ambiance cinematographique premium.
- Fluidite : Navigation instantanee via un routeur custom utilisant l'API History.
- Reactivite : Entierement responsive avec un systeme de grille hybride (Flexbox/Grid).

## Architecture Logicielle

- ES Modules : Code decoupe en modules reutilisables (js/auth.js, js/ui.js, etc.).
- Centralisation :
    - js/config.js : Point unique pour les URLs API et reglages globaux.
    - js/ui.js : Systeme de notifications (Toasts) et indicateurs de chargement.
- Evenements : Utilisation intensive de la delegation d'evenements.

## Fonctionnalites Cles

1. Booking Engine : Selection de sieges interactive avec calcul dynamique des tarifs.
2. Gestion Auth : Integration transparente du JWT avec persistance localStorage.
3. Systeme de Notifications : Toasts non-intrusifs.
4. Experience Paiement : Simulation visuelle de carte Visa avec validation Luhn.

## Developpement local

Le projet ne necessite aucune compilation. Vous pouvez le lancer avec n'importe quel serveur statique.

Design & Developpement par Antigravity - Moderniser le Cinema.
