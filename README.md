1 Lancer docker  
2 Lancer le serveur rabbitmq avec la commande ci-dessous:  
docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3.13-management  

3 Créer les utilisateurs sur rabbitmq  
4 lancer les scripts log.py et client.py  
