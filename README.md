# Projet CV avec Next.js et Docker
## Phase de développement
1. Clonez le repository :
   ```bash
   git clone https://github.com/AmirJaba/cvamir.git
   cd cvamir

2. Construction de l'Image Docker 
Construisez l'image Docker en exécutant la commande suivante à la racine du projet :
docker build -t cvamir .
3. Lancement du Conteneur Docker
docker run -p 3000:3000 cvamir

4. Développement dans le Conteneur
Vous êtes maintenant à l'intérieur du conteneur. Effectuez vos tâches de développement normalement.
Ouvrez [http://localhost:3000](http://localhost:3000) avec votre navigateur pour voir le résultat.
Vous pouvez commencer à éditer la page en modifiant `pages/index.js`. La page se met à jour automatiquement au fur et à mesure que vous modifiez le fichier.
5. Arrêt du Conteneur
Lorsque vous avez terminé, vous pouvez quitter le conteneur en tapant exit. Le conteneur sera automatiquement supprimé.

6. Autres Commandes Utiles
Pour lister tous les conteneurs en cours d'exécution : docker ps
Pour lister tous les conteneurs (y compris ceux arrêtés) : docker ps -a
Pour arrêter un conteneur en cours d'exécution : docker stop <ID_DU_CONTENEUR>
Notes Supplémentaires
Assurez-vous que le port nécessaire pour le développement est exposé dans le Dockerfile.
Les configurations spécifiques au développement peuvent être ajustées dans le Dockerfile selon les besoins.
