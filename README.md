# Projet Symfony - Intégration Stripe Checkout

---

![Image d'illustration](../public/images/screenshoot.png)


Ce projet Symfony implémente un système de paiement via Stripe Checkout, avec gestion des commandes et webhook pour la validation des paiements.

---

## Fonctionnalités

- Paiement Stripe Checkout avec plusieurs articles dynamiques
- Stockage des commandes en base de données (`Order` et `OrderItem`)
- Webhook Stripe pour mise à jour automatique du statut de la commande
- Gestion sécurisée des clés API via `.env.local`
- URLs de succès et d’annulation avec redirection propre

---

## Prérequis

- PHP 8.x
- Composer
- Symfony CLI (optionnel)
- Base de données configurée (MySQL/PostgreSQL...)
- Compte Stripe avec clés API (test et production)
- ngrok (pour exposer localement le webhook)

---

## Installation

1. Cloner le repo
   ```bash
   git clone https://github.com/ton-repo/stripe-payment.git
   cd stripe-payment/app
   composer install
   cd ..
   docker compose up
