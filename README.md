templates/
├── base.html.twig        ← layout principal
├── home.html.twig        ← page d’accueil
├── covoiturage.html.twig ← page de recherche/annonce
├── security/
│   ├── login.html.twig       ← connexion
│   └── register.html.twig    ← inscription
├── dashboard/
│   ├── passager.html.twig
│   ├── conducteur.html.twig
│   └── passager_conducteur.html.twig

-------------------------------------------------------------------------
✍️ 2. Syntaxe Twig de base
Ce que tu veux faire	                    Syntaxe Twig
Afficher une variable	                    {{ variable }}
Condition if	                            {% if user %} Bonjour {{ user }} {% endif %}
Boucle for	                                {% for trajet in trajets %} ... {% endfor %}
Inclure un fichier	                        {% include 'partials/_header.html.twig' %}
Étendre un layout (héritage)	            {% extends 'base.html.twig' %}
Définir des blocs modifiables               {% block content %} ... {% endblock %}

--------------------------------------------------------------------------
🧩 Commande	            📌Définition
git init	            Initialise un nouveau dépôt Git dans le dossier courant.
git clone <url>	        Crée une copie locale d’un dépôt distant (GitHub, GitLab, etc.).
git status	            Affiche les fichiers modifiés, en attente, ou non suivis.
git add <fichier>	    Ajoute un fichier à l’index (zone de staging).
git add .	            Ajoute tous les fichiers modifiés à l’index.
git commit -m "message"	Sauvegarde les changements dans l’historique avec un message.
git push	            Envoie les commits locaux vers le dépôt distant.
git pull	            Récupère les changements du dépôt distant et fusionne localement.
git fetch	            Récupère les changements distants sans fusionner.
git merge <branche>	    Fusionne une branche dans la branche courante.
git branch	            Liste les branches locales.
git branch <nom>	    Crée une nouvelle branche.
git checkout <branche>	Change de branche.
git checkout -b <nom>	Crée et passe à une nouvelle branche.
git log	                Affiche l’historique des commits.
git diff	            Affiche les différences entre fichiers (non commités).
git reset	            Réinitialise l’index et le working directory.
git reset --hard	    Supprime tous les changements non commités.
git rm <fichier>	    Supprime un fichier du dépôt.
git mv <src> <dest>	    Renomme ou déplace un fichier.

🔧 Commandes avancées
🛠 Commande	                📌 Définition
git stash	                Sauvegarde temporairement les modifications non commités.
git stash pop	            Restaure les fichiers mis en stash.
git rebase <branche>	    Rejoue les commits sur une autre branche.
git remote	                Affiche les dépôts distants configurés.
git remote -v	            Liste les URL des dépôts distants.
git remote add origin <url>	Ajoute un dépôt distant.
git tag	                    Liste ou crée un tag (version).
git cherry-pick <commit>	Applique un commit précis d’une autre branche.
git revert <commit>	        Annule un commit en créant un nouveau commit inverse.
git config	                Configure Git (nom, email, éditeur, etc.).
git clean -fd	            Supprime les fichiers non suivis (⚠️ dangereux).

🛡️ Commandes de sécurité et dépannage
🔐 Commande	                📌 Définition
git blame <fichier>	            Montre ligne par ligne qui a modifié quoi.
git bisect	                    Aide à trouver un commit fautif par recherche binaire.
git reflog	                    Affiche l’historique local des HEAD (utile après reset).
git fsck	                    Vérifie l’intégrité du dépôt.

