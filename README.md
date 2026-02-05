🇫🇷 Présentation

ENT Scrapper est une application Node.js qui se connecte à un ENT compatible Scolengo afin de récupérer et afficher :

📅 Emploi du temps de la semaine

📊 Notes et moyennes (générale + par matière)

📝 Devoirs à faire (avec gestion urgent / fait)

Les données sont synchronisées automatiquement et affichées dans une interface web moderne et responsive.

🇬🇧 Overview

ENT Scrapper is a Node.js application that connects to a Scolengo-compatible ENT to fetch and display:

📅 Weekly timetable

📊 Grades and averages (global & per subject)

📝 Homework assignments (with urgent / done status)

Data is automatically synchronized and displayed in a clean web dashboard.

✨ Fonctionnalités / Features

🔐 Authentification via token Scolengo

🔄 Synchronisation automatique toutes les 20 minutes

💾 Cache local (data/cache.json)

✅ Marquer les devoirs comme faits

⚠ Détection des devoirs urgents

🌙 Interface web moderne (dark mode)

🛠️ Technologies

Node.js

Express

scolengo-api

node-cron

HTML / CSS (vanilla)

🚀 Installation
1️⃣ Prérequis

Node.js ≥ 18

Un compte ENT utilisant Scolengo

2️⃣ Génération du token Scolengo

Lance scolengo-token

Connecte-toi à ton ENT

Télécharge le fichier JSON généré

Place-le à la racine du projet

Renomme-le en :

token.json

3️⃣ Installation des dépendances
npm install

4️⃣ Configuration

Crée un fichier .env (optionnel si tu modifies le code directement) et assure-toi que le chemin du token est correct :

TOKEN_PATH=./token.json


(par défaut le projet utilise ./token.json)

5️⃣ Lancement du serveur
npm start


Le serveur sera accessible sur :

http://localhost:3000

🔄 Synchronisation des données

Synchronisation automatique au démarrage

Puis toutes les 20 minutes

Les données sont stockées dans :

data/cache.json

🖥️ Interface Web

📅 Emploi du temps avec devoirs intégrés

📊 Notes + moyennes

📝 Liste complète des devoirs

✅ Case à cocher pour marquer un devoir comme fait

📂 Structure du projet
entscrapper/
├── data/
│   └── cache.json
├── services/
│   └── ent.js
├── server.js
├── token.json
├── package.json
└── README.md

⚠️ Avertissement

Ce projet est :

🔒 Personnel

🧪 Expérimental

❌ Non affilié officiellement à Scolengo ou à un ENT

Utilisation à vos propres risques.

📜 Licence

MIT – libre d’utilisation et de modification.

support = entscrapper@gmail.com
