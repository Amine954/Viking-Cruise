# 🚢 Viking Cruise

> Plateforme web e-commerce de réservation de croisières en mer Baltique.

Viking Cruise est une application web **full-stack** permettant de rechercher, consulter et réserver des croisières à travers les destinations nordiques (Norvège, Suède, Finlande, Estonie, Danemark, Lettonie). Le projet inclut l'authentification, un panier de réservation et une interface d'administration.

---

## 📋 Sommaire

- [Stack technique](#-stack-technique)
- [Fonctionnalités](#-fonctionnalités)
- [Flux utilisateur](#-flux-utilisateur)

---

## 🛠️ Stack technique

- **Backend :** PHP
- **Frontend :** HTML, CSS, JavaScript
- **Données :** CSV (voyages, utilisateurs) et JSON (descriptions détaillées)

---

## ✨ Fonctionnalités

### 🔐 Authentification
Inscription (validation e-mail + confirmation du mot de passe), connexion avec session PHP, profils modifiables, déconnexion sécurisée et gestion de statuts (`client` / `admin`).

### 🔎 Recherche de voyages
5 croisières disponibles (Nordhavn, Solstorm, Fjorddrakkar, Yggdrasil, Valkyra), avec filtrage par ville, tri dynamique (prix, alphabétique), pagination et pages de détail avec itinéraires.

### 🎫 Réservation
Formulaire complet (date, durée, cabine, parcours, voyageurs) avec **calcul de prix en temps réel** :

- **Cabines :** Standard · Balcon · Suite Deluxe
- **Parcours :** Pass Liberté · Flex 1 (+100 €) · Flex 2 (+300 €)
- **Add-ons :** Wi-Fi (+10 €/jour) · Animaux (+8 €/jour)

### 🛒 Panier
Affichage des réservations en session avec leurs détails complets et des liens pour modifier ou acheter.

### 🛠️ Administration
Espace réservé aux admins pour gérer les utilisateurs : ⭐ statut VIP, 🎟️ réductions, 🔨 bannissement — le tout en temps réel via JavaScript.

### 🌗 Thème clair / sombre
Basculement depuis le header, avec persistance en `localStorage`.

---

## 🧭 Flux utilisateur

1. **Accueil** → présentation et destinations populaires
2. **Recherche** → consultation de tous les voyages
3. **Détails** → description complète et itinéraire
4. **Authentification** → redirection vers la connexion si nécessaire
5. **Réservation** → paramètres et calcul de prix en temps réel
6. **Récapitulatif** → résumé avant validation
7. **Panier** → réservations en session

> **Côté admin :** un lien « Administration » donne accès à la gestion des utilisateurs et de leurs statuts.

---

**Bon voyage ;)**
