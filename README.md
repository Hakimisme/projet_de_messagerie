# 📧 Projet Messagerie avec RabbitMQ et Python

Bienvenue dans le projet de messagerie instantanée utilisant RabbitMQ et une interface graphique Python ! Ce guide vous aidera à configurer et lancer l'application étape par étape.

## 🚀 Étapes d'installation

1. **Lancer Docker**

   Assurez-vous d'avoir Docker installé sur votre machine. Si ce n'est pas le cas, vous pouvez le télécharger et l'installer depuis Docker.

   ```bash
   docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3.13-management
   ```

2. **Démarrer le serveur RabbitMQ**

   Utilisez la commande ci-dessous pour lancer un conteneur Docker avec RabbitMQ :

   ```bash
   docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3.13-management
   ```

3. **Créer les utilisateurs sur RabbitMQ**

   Ouvrez votre navigateur et allez à l'adresse : http://localhost:15672/.
   Connectez-vous avec les identifiants par défaut :
   - Utilisateur : guest
   - Mot de passe : guest

   Allez dans l'onglet Admin et cliquez sur Add User. Ajoutez de nouveaux utilisateurs avec les permissions nécessaires.

4. **Installer les packages nécessaires**

   Avant de lancer les scripts, installez les dépendances requises. Utilisez la commande suivante :

   ```bash
   pip install pika customtkinter requests
   ```

5. **Lancer les scripts**

   Pour démarrer l'application de messagerie, exécutez les scripts `log.py` et `client.py` :

   ```bash
   python log.py
   python client.py
   ```

## 🎉 Et voilà !

L'application de messagerie instantanée est maintenant prête à l'emploi. Vous pouvez commencer à envoyer et recevoir des messages via l'interface graphique.
