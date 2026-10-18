# E-ZARAtrans
Système Intelligent de Gestion, Réservation et Prédiction pour les Coopératives de Transport à Madagascar
# SmartTrans Madagascar

> **Système Intelligent de Gestion, Réservation et Prédiction de la Demande pour les Coopératives de Transport**

 Projets de Fin d'Études — Licence 3 (ISPM)  
 **Spécialité :** Génie Logiciel et Intelligence Artificielle (IGGLIA)  

---

##  1. Contexte et Présentation du Projet

### 1.1 Contexte
À Madagascar, le transport national et régional (taxibrousses) ainsi que les services de livraison font face à des défis majeurs :
- Attentes prolongées aux gares routières (Andohatapenaka, Ampasampito, etc.) et absence de visibilité en temps réel sur les places disponibles.
- Gestion manuelle (sur papier) des réservations et du suivi financier par les coopératives.
- Absence de planification intelligente des départs, entraînant des retards ou des trajets à vide non rentables.

### 1.2 Objectif du Projet
Développer une solution globale (Web & Mobile) couplée à un moteur d'Intelligence Artificielle permettant de :
1. Digitaliser la gestion administrative et financière des coopératives de transport.
2. Offrir aux usagers une application mobile de réservation de billets et de suivi en temps réel.
3. Utiliser un modèle d'IA pour prédire la demande de transport et optimiser le planning des trajets.

---

## 👥 2. Périmètre et Architecture

### 2.1 Acteurs du Système
- **Client / Passager :** Effectue les réservations, suit l'emplacement du véhicule et reçoit ses e-tickets.
- **Guichetier / Agent :** Enregistre les départs, valide les réservations et gère la caisse au niveau des gares.
- **Administrateur Coopérative :** Visualise les statistiques, gère les véhicules, les chauffeurs et les itinéraires.
- **Chauffeur :** Signale la position du véhicule et met à jour l'état du voyage.

### 2.2 Stack Technique
- **Frontend Web (Admin / Guichet) :** React.js / Vue.js
- **Frontend Mobile (Clients) :** Flutter / React Native
- **Backend / API :** Node.js (Express) / Python (FastAPI)
- **Intelligence Artificielle :** Python (Scikit-learn, Pandas, XGBoost / Prophet)
- **Base de données :** PostgreSQL avec extension PostGIS (ou MongoDB)
- **Paiement Mobile :** API MVola / Orange Money / Airtel Money

---

## 🛠️ 3. Spécifications Fonctionnelles

### Module 1 : Gestion de la Coopérative (Web Admin)
- **Gestion du parc automobile :** Ajout/Modification de véhicules, nombre de places, état technique.
- **Gestion des lignes et itinéraires :** Trajets, arrêts intermédiaires, tarifs par siège.
- **Gestion du personnel :** Profils des chauffeurs et affectation aux véhicules.
- **Tableau de bord financier :** Rapport quotidien des recettes, taux de remplissage.

### Module 2 : Réservation et Billetique (Mobile Client & Web Guichet)
- **Recherche de trajets :** Par date, ville de départ/arrivée et nombre de passagers.
- **Sélection dynamique des sièges :** Plan visuel du bus/véhicule (choix de la place exacte).
- **Paiement :** Intégration du paiement mobile local avec émission d'un e-billet QR Code.
- **Mode Hors-Ligne (Offline-First) :** Pour les guichetiers dans les zones à faible connectivité.

### Module 3 : Tracking & GPS en Temps Réel
- **Géolocalisation :** Envoi des coordonnées GPS du véhicule vers le serveur.
- **Suivi usager :** Affichage de la position estimée du bus sur une carte.

### Module 4 : Moteur d'IA (Prédiction et Optimisation)
- **Prédiction de la demande :** Analyse des données historiques croisées avec les événements locaux (saisons des pluies, vacances, fêtes, jours de paye).
- **Estimation du temps d'arrivée (ETA) :** Calcul affiné du temps de trajet en fonction de l'état des routes nationales.

---

## 🎯 4. Livrables Attendus
1. **Cahier des Charges & Spécifications UML/Merise** (MCD/MLD, Diagrammes de cas d'utilisation).
2. **Code Source complet** documenté sur ce dépôt.
3. **Application Web Fonctionnelle** (Admin & Guichet).
4. **Application Mobile (APK)**.
5. **Modèle IA opérationnel** (Notebook Jupyter / Scripts d'API REST).
6. **Rapport de Fin d'Études & Présentation Slide**.
