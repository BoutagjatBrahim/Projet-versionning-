# Projet-versionning 

## Table des matières
* [Infos générales](#infos-générales)
* [Statut](#status)
* [Technologies](#technologies)
* [Organisation](#organisation)
* [Fonctionnalités](#fonctionnalités)
* [Chambre des améliorations](#chambre-des-améliorations)
* [Les acquis](#les-acquis)
* [Remerciement](#remerciement)
* [Contact](#contact)

## Informations générales
  - Ce projet est simplement la refonte d'un ancien site de vente de voiture.
  - Ce projet intervient notamment dans le cadre de la manipulation et la familiarisation avec les commandes git.
  - Le but de ce projet est d'apprendre à utiliser git en travaillant de manière collective sur des taches différents. Ces dernières vont etre assembler pour donner un rendu complet qui donnera suite au déploiment sur internet. 


## Status
  complet

## Les technologies
  Le projet est créé avec :
  * HTML
  * CSS
  * JAVASCRIPT

## Organisation
  * Ancien projet
  - Sur le plan organisationnel, nous avons eu quelques problèmes mineurs, où la répartition des tâches fonctionnait très bien sauf que nous avons finalement réalisé une erreur majeure.
Le principal défaut est la création de tags + pull requests lorsque la continuité des tâches réalisées est mesurée.
Mais à part cela, nous sommes organisés au niveau de l'équipe car nous avons des réunions régulières au cours desquelles nous évaluons ce qui doit être fait et ce qui ne l'est pas.

  * Nouveau projet
  - C'est donc pourquoi à la des tache terminé on a décider de recréer un repos git dans le quel ona défini une autre 


## Fonctionnalité
  ### Créer une clé ssh :
    ** Pour connecter GitHub à notre machine locale ** 
    - Profile > settings > SSH and GPG keys > generating a new SSH key and adding it to the ssh-agent 
    - Profile > settings > SSH and GPG keys > New SSH key 
    
  ### Création de repo du projet : 
    ** création du repository sur GitHub ** 
    - New repository 
    ** copy du projet en locale **
    - "git clone <fichier https du projet >"
    - "git commit"
    - "git push" __dans le repo git__ 
    
  ### Création des branches : 
    ** Après organisation des tâches, nous avons créer des branches respectives pour développer nos modifications avant 
    de les merge dans la branche dev **
    - "git branch <nom de la branche>"
    - "git checkout <nom de la branche>" pour switcher de branche 
   
  ### Création de pull request :
    ** Indique aux autres que la tâche est fini et merge les commits sur la branche sélectionnés **
  
  ### Création des tags :
    ** Les tags sont utilisés pour créer (des points de sauvegardes) ou point de version ** 
    - "git tag <identifiant de la version>" 
    - "git push origin <nom de la version>" 
  
  ###  Synchronisation du dépot distant en local :
    - git pull 
  
  ###  Déploiement du projet sur Netlify : 
    ** installation de netlify en locale ** 
    - "npm install netlify-cli -g" 
    - "netlify login" __pour connecter notre machine à notre compte netifly__
    - "ntl init" __pour créer notre projet netlify__ 
    - case à valider 1 : create & configure a new site
    - case à valider 2 : select netlify team 
    - case à valider 3 : choose name for application 
    - case à valider 4 : your build command ? Tap enter 
    - case à valider 5 : directory to deploy ? Tap enter 
    - case à valider 6 : Netifly function folder ? Tap enter 
    - case à valider 7 : create netlify.toml ? yes 
    - "git add." 
    - " git commit -m 'configuration du projet netlify'"
    - "git push" 
    
    ** Création des clés ** 
    - création de la clé d'authentification netlify NETLIFY_AUTH_TOKEN
    - Dans Netlify > profil > user settings > applications > New oath app > copy __secret__
    - Dans github > setting > secrets > actions > new repository secrets > NETLIFY_AUTH_TOKEN > paste __secret__ 
    - création de la clé build netlify NETLIFY_HOOK_ID
    - Dans Netlify > Team overview > sites > netlify projet > site settings > Build & Deploy > Build hooks 
      > select last number 
    - Dans github > setting > secrets > actions > new repository secrets > NETLIFY_HOOKS_ID > paste CODE 
    
    ** Création github action workflows ** 
    - Dans github > actions > new workflow 
    - git commit 
    
    ** Modification fichier netlify.toml **
    - Ajout de la section Build 
    
    ** Modifications du site settings dans Netlify **
    - Build & Deploy > Build Settings > publish directory (ProjetVersionning/garage). 
    
    
## Chambre des améliorations



## Les acquis


## Remerciement

## Contact
Created by 
* Brahim Boutagjat
* Michael yaromishyan
* Frédéric Zai
* Amine
