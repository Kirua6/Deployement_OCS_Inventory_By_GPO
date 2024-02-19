# Déploiement d'OCS Inventory via GPO

Ce tutoriel guide à travers les étapes nécessaires pour déployer OCS Inventory en utilisant les Group Policy Objects (GPO) sous Windows Server. C'est une méthode efficace pour automatiser le déploiement d'OCS Inventory sur plusieurs machines dans un réseau d'entreprise.

## Prérequis

Avant de commencer, assurez-vous de satisfaire aux exigences suivantes :

- **Windows Server 2019** : Le serveur doit avoir le rôle AD/DS installé.
- **Droits d'administrateur sur Active Directory** : Nécessaires pour effectuer les configurations de déploiement.
- **Serveur OCS** : Un serveur Debian ou Red Hat avec LAMP (Linux, Apache, MySQL, PHP) et OCS Inventory Server installés et configurés.

## Étapes du déploiement

### 1. Téléchargement des ressources

Téléchargez les ressources suivantes nécessaires au déploiement :

- OCS Packager
- OCS-Windows-Agent
- PsExec et PsExec64
- pscp et putty

### 2. Préparation et configuration des ressources

Préparez un dossier avec toutes les ressources téléchargées et configurez OCS Packager pour créer un package OCS à déployer. Suivez les instructions détaillées pour configurer correctement chaque composant.

### 3. Création et déploiement via GPO

Configurez une GPO pour permettre le déploiement automatique d'OCS sur les ordinateurs des utilisateurs. Ce processus implique la création d'une nouvelle politique de groupe et son association aux unités organisationnelles ciblées.

## Mise en garde

Il est fortement recommandé de tester ce déploiement dans un environnement de test avant de procéder à une mise en production. Cela permet d'éviter tout impact négatif potentiel sur l'infrastructure existante.

