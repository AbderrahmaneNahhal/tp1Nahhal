# Utilisation de l’IA — TP1

Abderrahmane Nahhal — Groupe 1, n° 17

## 1. Configuration du projet

- **Problème :** Configurer la clé Gemini et créer le projet TP1.
- **Pourquoi l’IA :** Avoir les étapes à suivre dans Windows et IntelliJ.
- **Prompts utilisés :** « Que dois-je faire après avoir copié la clé API ? » et « Peux-tu me guider étape par étape ? »
- **Aide reçue :** Enregistrer la clé dans `GEMINI_KEY` et créer un projet séparé du TP0.
- **Ce que j’ai appris :** Java lit la clé avec `System.getenv()` sans qu’elle soit écrite dans le code.

## 2. Mode debug et connexion à Gemini

- **Problème :** Adapter `Bb.java` et corriger une erreur de compilation dans le client Gemini.
- **Pourquoi l’IA :** Savoir où modifier le code et comprendre le rôle de chaque classe.
- **Prompts utilisés :** « Voici mon code actuel. Que dois-je modifier et pourquoi ? » J’ai aussi partagé une capture de l’erreur de compilation.
- **Aide reçue :** Ajouter les propriétés du mode debug, injecter l’adaptateur dans `Bb` et corriger le constructeur du client.
- **Ce que j’ai appris :** `Bb` gère l’affichage, l’adaptateur prépare le JSON et le client envoie la requête HTTP.

## 3. Lecture du JSON et tests d’erreur

- **Problème :** Comprendre l’historique JSON et distinguer les deux erreurs `400`.
- **Pourquoi l’IA :** Interpréter les résultats de mes tests.
- **Prompts utilisés :** « Peux-tu m’expliquer les résultats que je t’ai copiés ? » et « Quelle est la différence avec l’erreur précédente ? »
- **Aide reçue :** Examiner le tableau `contents` et lire `error.message` pour identifier la cause de chaque erreur.
- **Ce que j’ai appris :** L’adaptateur renvoie les échanges précédents avec la nouvelle question. Deux erreurs peuvent avoir le même code HTTP mais des causes différentes.

## 4. Rôle personnalisé et erreur 503

- **Problème :** Choisir un rôle personnalisé et terminer son test malgré les erreurs `503`.
- **Pourquoi l’IA :** Trouver un rôle lié au data engineering et comprendre l’échec des appels.
- **Prompt utilisé :** « J’obtiens toujours la même erreur, même après avoir attendu quelques minutes. »
- **Aide reçue :** Proposer le rôle « Coach qualité des données » et lister les modèles Gemini disponibles pour en essayer un autre.
- **Ce que j’ai appris :** Le message `503` signalait une surcharge du modèle. J’ai validé le rôle dans un nouveau chat avec exactement deux échanges.