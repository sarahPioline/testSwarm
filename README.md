# TP - Docker Swarm
Contributeur : Greg, Sarah, Thomas, Clément, Valentin (Presque tout les ancien B3)

## schéma
<img src="./schema-docker-swarm.png" alt="">

## Initialisation
Démarrer vos VMs et installer docker sur chacun.

Sur la VM 'manager' exécuter les lignes suivantes dans le terminal :

    $ sudo docker swarm init

    $ docker swarm join --token SWMTKN-1-1jyx1grn9l5ru7oh2hxlquioccoasrxcstqwr9c511gwzah98y-ac0ulnp1e1sey7ntyumidqtu0 X.X.X.X:2377


Maintenant, ajouter des workers :

    $ sudo docker swarm join --token SWMTKN-1-1jyx1grn9l5ru7oh2hxlquioccoasrxcstqwr9c511gwzah98y-ac0ulnp1e1sey7ntyumidqtu0 X.X.X.X:2377

Deployer la stack :

    $ sudo docker stack deploy --compose-file docker-compose.yaml tpdocker

## Les liens :

Traefik : https://traefik.uwu

Wordpress : https://wordpress.uwu

ps : Sur Linux, ils faut préciser l'adresse IP du worker dans le fichier de conf host sinon le DNS fonctionne pas et pas de '.uwu'.

## Enjoy !
