### Telecharger une image
```bash
docker pull mongo
```

### Afficher les images
```bash
docker images
```

### Exécuter un conteneur MongoDB
```bash
docker run -d -p 27017:27017 --name mongo-example mongo:latest
```
- Cette commande lance un conteneur MongoDB en arrière-plan (`-d`) avec le port local 27017 mappé sur le port du conteneur 27017. Le nom du conteneur est défini comme "mongo-example" en utilisant l'image MongoDB la plus récente (`mongo:latest`).

### Entrer dans le conteneur MongoDB
```bash
docker exec -it mongo-example mongosh
```
- Cette commande permet d'entrer dans le conteneur en cours d'exécution et d'ouvrir l'interpréteur de commandes MongoDB (`mongo`).

### Afficher les conteneurs en cours d'exécution
```bash
docker ps
```
- Cette commande affiche la liste des conteneurs en cours d'exécution avec des détails tels que l'ID du conteneur, le nom, l'image utilisée, le statut, les ports mappés, etc.

Bien sûr, continuons avec quelques étapes supplémentaires pour explorer davantage Docker :

### Afficher toutes les images (y compris celles intermédiaires)
```bash
docker images -a
```
- Cette commande affiche toutes les images, y compris celles qui sont intermédiaires. Parfois, des images intermédiaires sont créées lors de la construction d'une image Docker.

### Afficher tous les conteneurs (y compris ceux arrêtés)
```bash
docker ps -a
```
- Cette commande affiche tous les conteneurs, qu'ils soient en cours d'exécution ou arrêtés. Elle fournit des détails tels que l'ID du conteneur, le nom, l'image utilisée, le statut, les ports mappés, etc.

### Arrêter un conteneur en cours d'exécution
```bash
docker stop mongo-example
```
- Cette commande arrête le conteneur spécifié (`mongo-example` dans cet exemple).

### Supprimer un conteneur arrêté
```bash
docker rm mongo-example
```
- Cette commande supprime le conteneur spécifié qui a été arrêté (`mongo-example` dans cet exemple).

### Supprimer une image Docker
```bash
docker rmi nom_de_l_image
```
- Cette commande supprime l'image Docker spécifiée.

N'oubliez pas de remplacer "nom_de_l_image" par le nom ou l'ID réel de l'image que vous souhaitez supprimer.

