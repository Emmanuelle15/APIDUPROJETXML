# API DU PROJET XML
Ceci est un projet à titre scolaire afin de consolider nos connaissances dans le domaine des web services. 

![image](https://github.com/Emmanuelle15/APIDUPROJETXML/blob/master/api.gif)

## Préréquis
- un serveur LAMP ou WAMP
- SoapUI ou POSTMAN


## Installation
- Télécharger le fichier zippé api_xml 
- Dézipper le fichier
- Déplacer le dossier dézippé dans le dossier www de Apache
- Ouvrir le fichier api_xml/src/configs/DBAccess.php
- Modifier les lignes 6, 7 et 8 du fichier par vos propres valeurs.
- Démarrer le serveur Apache
- Se connecter sur PhpMyAdmin
- Dans la base de données renseignée au niveau de la ligne 6 du fichier api_xml/src/configs/DBAccess.php, créer une table T_Users avec les champs 

      -> id
      -> nom
      -> numero
      -> adresse
      -> commentaire

 Si la base de données indiquée au niveau de la ligne 6 n'existe pas, vous la créez 
 
## Test avec SOAP UI
- Lancer SoapUI
- Dans l'onglet file, cliquer sur NEW REST project
- Entrer URI, ex: http://localhost/api_xml/public/
- Tester l'ajout d'utilisateur


      -> Method : POST
      -> Ressource : /api_xml/public/api/voisin
      -> Parametres : nom, numero, adresse, commentaire
      
    
    
- Cliquer sur le bouton play 

Vous recevrez un message de la forme 

     {
       "status" : "OK",
       "message" : "The neighbor has been added successfully."
     }



        
    
    
    
    
    
