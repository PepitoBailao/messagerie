# Application messagerie en Java
## Description
Ce projet étudiant consiste à développer une application de chat interne en Java permettant à des employés de communiquer en temps réel. Chaque utilisateur peut poster des messages visibles par tous, et un système de likes permet de mettre en avant les messages populaires. Un score d'actualité est calculé pour chaque message en fonction de son âge et du nombre de likes.

## Fonctionnalités
- **Chat en temps réel** : Envoi et réception de messages instantanés via une interface console ou graphique (Java Swing, JavaFX, etc.). 
- **Système de likes** : Les utilisateurs peuvent liker les messages, ce qui influe sur leur position dans le fil de discussion. 
- **Calcul du score d'actualité** : Le score d’actualité des messages est calculé avec la formule suivante : `ω = (30 - δ) × α`, où \( δ \) est l’âge du message (en jours) et \( α \) le nombre de likes.

## Prérequis
- **Java Development Kit (JDK)** version 11 ou supérieure 
- **IDE** comme IntelliJ IDEA, Eclipse ou NetBeans 
- **Maven** ou **Gradle** pour la gestion des dépendances

## Installation
### Étapes pour exécuter le projet
1. Clonez ce dépôt : `git clone https://github.com/username/chat-stream-java.git` 
2. Ouvrez le projet dans votre IDE préféré (IntelliJ, Eclipse, etc.). 
3. Compilez le projet avec Maven ou Gradle : `mvn clean install` ou `gradle build` 
4. Exécutez l'application principale : `java -jar target/chat-stream-app.jar` 
5. L’application sera lancée et vous pourrez interagir via l'interface utilisateur (console ou GUI).

## Structure du projet
Le projet est structuré en différents packages pour organiser les fonctionnalités :
- `model` : Contient les classes de données (Message, Utilisateur). 
- `service` : Contient la logique métier (gestion des messages, calcul du score). 
- `ui` : Interface utilisateur (JavaFX/Swing). 
- `test` : Contient les tests unitaires et d'intégration.

## Utilisation
### Ajouter un message
Lancez l'application, entrez votre message dans l'interface, puis envoyez-le pour qu'il apparaisse dans le fil de discussion.

### Liker un message
Cliquez sur le bouton "Like" ou utilisez la commande correspondante dans la console.

### Calcul du score
Le score des messages est mis à jour dynamiquement en fonction du nombre de likes et de l’âge du message.

## Tests
Pour exécuter les tests unitaires, utilisez la commande suivante : `mvn test` ou `gradle test`

## Contribution
Les contributions sont encouragées ! Voici comment vous pouvez participer :
1. **Fork** ce dépôt. 
2. Créez une branche avec votre fonctionnalité : `git checkout -b feature/nom-fonctionnalité` 
3. Faites vos modifications et commitez-les : `git commit -m "Ajout de fonctionnalité"` 
4. Poussez vos modifications vers votre fork : `git push origin feature/nom-fonctionnalité` 
5. Ouvrez une **Pull Request** pour que vos modifications soient examinées.

## License
Ce projet est sous licence MIT. Consultez le fichier `LICENSE` pour plus d'informations.
