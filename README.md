# Projet : Installation et Configuration des Services Réseau

## Description
L’objectif de ce projet est d’installer et de configurer les services suivants sur des serveurs Windows 2016 :  
- DNS  
- Accès à distance  
- Messagerie  

Le projet est réalisé dans le cadre du cours de réseau et systèmes distribués, avec pour objectif de mettre en pratique la gestion de services critiques sur un réseau d’entreprise simulé.

---

## 1️⃣ Objectifs

### 1.1 Service DNS
- Acheter un domaine auprès du « registrar » représenté par l’enseignant.  
- Gérer un sous-domaine du TLD privé `.tp`.  
- Configurer un serveur DNS **primaire** sur Windows Server 2016 :  
  - Nom du serveur : `R303_B9_1`  
  - Ce nom sera utilisé comme nom de VM et nom système.  
- Configurer un serveur DNS **secondaire** pour assurer la redondance :  
  - Nom du serveur : `R303_B9_2`  
- Créer deux sous-domaines dans la zone principale :  
  - Déléguer la gestion d’un des sous-domaines à un troisième serveur :  
    - Nom : `R303_B9_3`  

---

### 1.2 Service d’accès à distance
- Configurer le serveur `R303_<groupe>_3` pour autoriser plus de deux connexions simultanées.  
- Les utilisateurs du domaine `peda.rt.local` doivent pouvoir accéder à distance aux applications :  
  - Thunderbird (client de messagerie)  
  - Wireshark  
- L’accès doit se faire via **Remote Desktop Web**.

---

### 1.3 Service de messagerie
- Installer un serveur de messagerie sur un **quatrième serveur** :  
  - OS : Windows Server 2016  
  - Nom : `R303_B9_4`  
  - Logiciel : `hMailServer`  
- Services à configurer : IMAP, POP et SMTP.  
- Créer **deux comptes utilisateurs** pour tester la messagerie.  
- Configurer les clients de messagerie pour vérifier le fonctionnement :  
  - Un compte utilisant le service **POP**  
  - Un compte utilisant le service **IMAP**  
- Le serveur doit pouvoir transférer les mails vers des domaines extérieurs (par exemple ceux des camarades).  
- Un serveur de test géré par l’enseignant est disponible pour l’envoi des mails :  
  - Compte : `maurice@tp.r`  

---


