L'API est un service fourni pour les développeurs qui souhaiteraient créer des modules basés sur Bank Tycoon.

Chaque serveur de jeu à son API accessible sur l'url [http://banktycoon.com/](http://banktycoon.com/){serveur}/api

Ainsi vous pouvez accéder à la liste des alliances d'un serveur en appelant la page [http://banktycoon.com/s3/api/alliancesList.json](http://banktycoon.com/s3/api/alliancesList.json)

Elle comporte 3 services :


*  **/agencesPays/agences{Code lettre pays}.json **:
      * Retourne un tableau JSON contenant toutes les agences d'un pays :
        * region : l'id de la region de l'alliance
        * id :l'identifiant du propriétaire de l'agence
        * colonie : l'identifiant du joueur contrôlant l'agence (pour plus d'info voir [Prise de contrôle](/Prise de contrôle))
        * alliance : l'identifiant de l'alliance du joueur contrôlant l'agence.
      * Ce tableau est mis à jour toutes les heures.

*  **/alliancesList.json **:
      * Retourne la liste des alliances d'un serveur, leur identifiant, leur nom, leur sigle, leur nombre de membre.
      * Est mis à jour toute les 2 heures.

*  **/utilisateursList.json :**
      * **​**  Retourne la liste des joueurs d'un serveur, leur identifiant, leur nom de banque et leur alliance.
      * Est mis à jour toute les heures

