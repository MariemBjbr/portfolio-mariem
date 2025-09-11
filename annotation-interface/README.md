Interface d’annotation OCT — 4 biomarqueurs (demo publique)

Projet PHP/MySQL pour faciliter le travail des médecins : annotation, tri et export d’images OCT pour 4 biomarqueurs (mode démo, sans données réelles).

✨ Fonctionnalités (démo)

Annotation binaire/mono-classe pour 4 biomarqueurs

Verrouillage d’image (éviter conflits)

Historique d’annotations (audit basique)

Export trié par biomarqueur (fichiers/dossiers)

Important : ce dépôt ne contient aucune donnée patient. Les captures/vidéos doivent utiliser des images factices.

🧰 Stack

PHP (procédural + quelques utilitaires)

MySQL (structure simple)

HTML/CSS/JS vanilla

🚀 Lancer en local (rapide)

Installe XAMPP/MAMP/WAMP (Apache + MySQL).

Clone le repo dans htdocs (ou équivalent).

Copie config.example.php → config.php, et ajuste les accès DB.

Crée une base vide (ex. oct_demo).

Lance Apache + MySQL, puis ouvre http://localhost/nom-du-repo.

La démo s’affiche, mais sans données. Tu peux ajouter quelques images factices (non médicales) dans un dossier public_demo/ pour illustrer le flux.
