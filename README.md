# TESKERTI -- Plateforme de Reservation de Cinema

TESKERTI est une solution complete de billetterie pour le cinema tunisien, alliant une API REST PHP securisee et une Single Page Application (SPA) moderne en Vanilla JavaScript.

## Architecture du Projet

Le projet est divise en deux parties principales :

1. [Backend (teskerti-api)](./teskerti-api/README.md) : Moteur robuste en PHP (MVC), gestion des paiements et securite JWT.
2. [Frontend (teskerti)](./teskerti/README.md) : SPA performante en JavaScript pur (ES Modules), sans framework.

## Points Forts

- Modernite : Migration complete vers ES Modules cote client et PSR-4 cote serveur.
- Securite : JWT avec rotation des refresh tokens, hashing Argon2id, et protection anti-CSRF/CORS.
- Integrite : Transactions SQL atomiques pour garantir que chaque paiement correspond a une reservation confirmee.
- UX Premium : Design "Dark Mode" sophistique, Toasts personnalises, et navigation fluide.

## Demarrage Rapide

Le frontend peut etre servi par n'importe quel serveur HTTP statique.
L'API necessite PHP 8.2+ et MySQL.

## Stack Technique

- Frontend : HTML5, CSS3 (Vanilla), JavaScript (ES6+).
- Backend : PHP 8.2+ (Vanilla MVC), MySQL.
- Auth : JSON Web Tokens (HS256).

Developpe avec passion pour le cinema tunisien.
