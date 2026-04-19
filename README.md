# 1. Initialisation
mkdir mon_projet && cd mon_projet
git init

# 2. Création fichiers
touch index.html style.css about.html script.js

# 3. Premier commit
git add .
git commit -m "Première version"

# 4. Lier GitHub
git remote add origin https://github.com/islemkhlifi031/mon_projet.git
git branch -M main
git push -u origin main

# 5. Modification
git add index.html
git commit -m "Ajout paragraphe"
git push origin main

# 6. Branche contact
git checkout -b ajout-contact
git add contact.html
git commit -m "Ajout formulaire contact"
git checkout main
git merge ajout-contact
git push origin main

# 7. .gitignore
git add .gitignore
git commit -m "Ajout .gitignore"
git push origin main

# 8. Pull
git pull origin main
