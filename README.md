# Projet CV avec Next.js et Docker
## Phase de développement
1.  Clonage du repository à l'aide de la commande suivante :
```bash
   git clone https://github.com/AmirJaba/cvamir.git
   cd cvamir
```
3. Construire l'image Docker, exécutez la commande suivante à la racine du projet:

 ```bash
docker build -t cvamir .
 ```
3. Une fois l'image Docker construite, lancez le conteneur avec la commande:

```bash
docker run -p 3000:3000 cvamir
 ```
4. Vous serez maintenant à l'intérieur du conteneur, où vous pouvez effectuer vos tâches de développement. Accédez à http://localhost:3000 dans votre navigateur pour visualiser les résultats. Pour débuter l'édition, modifiez le fichier pages/index.js. La page se mettra à jour automatiquement à mesure que vous apportez des modifications au fichier.

5. Lorsque vous avez terminé le développement, quittez le conteneur en tapant "exit". Le conteneur sera automatiquement supprimé.

6. Quelques commandes utiles pendant le développement sont:

Pour lister tous les conteneurs en cours d'exécution:
```bash
docker ps
```
Pour lister tous les conteneurs (y compris ceux arrêtés):
```bash
docker ps -a
```
Pour arrêter un conteneur en cours d'exécution, utilisez:
```bash
docker stop <ID_DU_CONTENEUR>
```
Assurez-vous que le port nécessaire au développement est exposé dans le Dockerfile. Vous pouvez ajuster les configurations spécifiques au développement dans le Dockerfile selon vos besoins.
