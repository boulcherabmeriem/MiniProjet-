### MiniProjet #

### Réaliser par: #

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
  La plate-forme étend Java Platform, Standard Edition (Java SE) en fournissant une API de mapping objet-relationnel, des architectures distribuées et multitiers, et des services web3. La plate-forme se fonde principalement sur des composants modulaires exécutés sur un serveur d'applications. 
  Pour ce faire, Java EE définit les éléments suivants :
   + Une plate-forme (Java EE Platform), pour héberger et exécuter les applications, incluant outre Java SE des bibliothèques logicielles additionnelles du Java Development Kit (JDK) ;
   + Une suite de tests (Java EE Compatibility Test Suite) pour vérifier la compatibilité ;
   + Une réalisation de référence (Java EE Reference Implementation), dénommée GlassFish ;
   + Un catalogue de bonnes pratiques (Java EE BluePrints) ;
   + Un code script. </p>
  
  
 2)- *MVC utilisant des servlets.*
+ Serveur utilisé est Apache-Tomcat.


