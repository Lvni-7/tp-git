# tp-bachelor

J'ai cloné le dépot
git clone https://github.com/cecilev-axe/tp-bachelor.git

ensuite je me déplace a l'intérieur du dossier
cd tp-bachelor

j'ai supprimé l'ancien origin
git remote remove origin

j'ai créer un repo sur github

j'ai ajouté mon repo github comme origin
git remote add origin https://github.com/Lvni-7/tp-git.git

j'ai verifié que ca avais marché
git remote -v

Ensuite j'ai ajouté une nouvelle image et un dot dans le index.html

J'ai enregistré les changements avec :
git add .
git commit -m"ajout photo et dot"

J'ai envoyé sur mon repo distant
git push -u origin main

J'ai modifié la taille des dot de 15px a 20px puis commit("Increase size of dot elements in style.css 15px -> 20px") directement sur github

Puis en local de 15px a 25px
git add .
git commit -m"img size 15px -> 25px"

Ensuite quand j'ai fait un git pull un conflit est apparu car la taille des dots
avait été modifiée différemment sur github (20px) et en local (25px)

J'ai ouvert le fichier en conflit et j'ai choisi la version locale en 25px
en supprimant les lignes de conflit ajoutées par git

Puis j'ai enregistré avec :
git add .
git commit -m"img size 15px -> 25px version finale 2.0"

Enfin j'ai envoyé la version finale sur mon repo github
git push
