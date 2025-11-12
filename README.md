⚠️ Instructions pour exécuter le projet

Créer une base PostgreSQL locale :

Nom : postgres

Laisser la configuration par défaut (ou adapter le .env)

Créer un fichier .env à la racine du projet :
Exemple :

DATABASE_URL=postgresql://postgres:password@localhost:5432/postgres


Lancer le serveur WebSocket :

cargo run


Ouvrir le tableau de bord :

Ouvrir le fichier client.html dans un navigateur

Le dashboard se connecte automatiquement au WebSocket et affiche les prix en temps réel.

Résumé :

Serveur WebSocket en Rust (tokio, tokio-tungstenite)

Lecture des derniers prix via PostgreSQL (sqlx)

Diffusion temps réel à tous les clients (broadcast::channel)

Dashboard web simple en HTML, avec mise à jour automatique
