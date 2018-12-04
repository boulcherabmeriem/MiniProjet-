## MiniProjet #

## Réaliser par: #

*Chaachoua Anis*

*Boulcherab Meriem*

## Objectif: #

<p> Le but de ce projet est de permettre une approche globale de la matière Cloud Computing.
  Il s'agit de développer une application prète pour le cloud (cloud-ready or cloud-native application)
  de conversion de document proposant plusieur types de conversion pour les clients.
</p>

## Fonctionnement général: #

+ Une page d'accueil spécifier pour le client, dépose son document et choisie les convertions a realisé parmi elle disponibles et un e-mail de contact.
+ Une fois la demande enregistrée, l'application envoie un message (e-mail) confirmant que l'opération est en cours,
et un lien vers une page résumant le statut de chaque conversion (en attente, en cours , terminé)
*pour chaque statut le temp passé dans l'état courant est connaie.*
+ Lorsqu'un document est converti, un lien est mis a disposition depuis la page de statut permettant de le télécharger.
+ L'utilisateur dispose alors 5 minutes pour le télécharger après quoi ie sera supprimé.
+ Quand le document a été converti, un message est envoyé a l'utilisateur avec le lien.
+ Pour chaque utilisateur, il est possible de réaliser seulement 2 conversions a la fois.

## Particularités pour le projet: #

+ L'architecture de l'application est spécifiquement pou la plate forme Cloud.
+ L'application est d'une forme Services-Web.
+ Il n y a pas une interface pour l'application.
+ Synchronisation de plusieurs demandes,utulise les threads.
+ 2 Type de conversions.
+ Langage utilisé est java avec la plateforme J2EE.

##  L'Arcchitecture globale de l'application: #

 1)- *Plateforme utilisé est J2EE (Enterprise Edition):*
 
<p> J2EE est une spécification pour la plate-forme Java d'Oracle, destinée aux applications d'entreprise2. 
  La plate-forme étend Java Platform, Standard Edition (Java SE) en fournissant une API de mapping objet-relationnel, des architectures distribuées et multitiers, et des services web3. La plate-forme se fonde principalement sur des composants modulaires exécutés sur un serveur d'applications. </p>
  
  Pour ce faire, Java EE définit les éléments suivants :
  
   + Une plate-forme (Java EE Platform), pour héberger et exécuter les applications, incluant outre Java SE des bibliothèques logicielles additionnelles du Java Development Kit (JDK).
   + Une suite de tests (Java EE Compatibility Test Suite) pour vérifier la compatibilité.
   + Une réalisation de référence (Java EE Reference Implementation), dénommée GlassFish.
   + Un catalogue de bonnes pratiques (Java EE BluePrints).
   + Un code script. 
   
   ![java_platforms](https://user-images.githubusercontent.com/44198183/49477991-dfaa7e00-f81e-11e8-9a16-fa9a2c79ba04.PNG)
   
   
   
   
 <p> Il exist des ensemble des framework j2ee donc ensemble des bibliothèques qui sont structuré en MVC par exemple on a
  JSF,STRUTS,SPRING,HIBERNAT.</p>
  dans ce mini projet on va utilise le Spring. 
  
 2)- *MVC (Modèle-vue-contrôleur):*
 <p> est un motif d'architecture logicielle destiné aux interfaces graphiques lancé en 1978 et très populaire pour les applications web. Le motif est composé de trois types de modules ayant trois responsabilités différentes : les modèles, les vues et les contrôleurs.</p>
 
 ![modelemvc](https://user-images.githubusercontent.com/44198183/49478412-00270800-f820-11e8-80cd-1fbf50b40f99.png)
 
+ Description:

 <p> Une application conforme au motif MVC comporte trois types de modules : les modèles, les vues et les contrôleurs.
  
le visiteur qui envoi sa requéte HTTP transmie a le serveur application qui lui va transmie directement a la partie code,
 donc le contrôleur est une partie de code qui se compter de faire l'aiguillage de l'information c'est a dire le routage de l'information, il va décidée qui va récupirer l'information et ensuit la traitée.
 en général le contrôleur va appelé le modèle qui contient les informations strécturée de ne donnée qui va notament fais des calcules, se modèle peut envoyer les informations au contrôleur qui peut en suit générer une page web donc une vue.
 la vue représente en réalité a ce que le visiteur on va voir en final, et c bien la vue qui va envoyer a le visiteur.
</p>
  
  ![capture2](https://user-images.githubusercontent.com/44198183/49478285-a7576f80-f81f-11e8-8578-e17990440d85.PNG)
  
  ## Modèle:  #
 
 <p> Élément qui contient les données ainsi que de la logique en rapport avec les données: validation, lecture et enregistrement.
  on appel les objet java, peut etre a communicer a une base de donnée pour stocker les informations et garder en mémoire le plus tempe possible. </p>
  
 ## Contrôleur:  #
 <p> Module qui traite les actions de l'utilisateur, modifie les données du modèle et de la vue.
donc en va appelé une servlet.
</p>

## vue:  #
<p> Partie visible d'une interface graphique,  Une vue contient des éléments visuels ainsi que la logique nécessaire pour afficher les données provenant du modèle.
  on appel les pages JSP qui on en réalité des pages qui uilisé le code HTML et du code spécifique en générale en java,
  cette vue et donc retournée par le controleur au visiteur. </p>

 
3)- * Apache-Tomcat:*
<p> Est un conteneur web libre de servlets et JSP Java EE. Issu du projet Jakarta, c'est un des nombreux projets de l’Apache Software Foundation. Il implémente les spécifications des servlets et des JSP du Java Community Process6, est paramétrable par des fichiers XML et des propriétés, et inclut des outils pour la configuration et la gestion. Il comporte également un serveur HTTP.</p>



