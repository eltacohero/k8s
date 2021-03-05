# k8s
## Producteur
1. Créer un daemonSet nommé producteur basé sur l'image alpine
2. Créer un volume
3. Monter le volume sur le conteneur
4. Ecrire dans le fichier index.html le nom du hostname et la date toutes les 60 secondes

## Consommateur
1. Créer un déploiement nommé web avec 3 replicas basé sur l'image httpd
2. Monter le volume créé précédemment sur le chemin htdocs du serveur Apache

## Service NodePort
1. Créer un service nommé web de type NodePort qui rassemble les pods du déploiement web

## Utilisation
1. Depuis le poste de travail, exécuter toutes les minutes la commande "curl node1:30000"
