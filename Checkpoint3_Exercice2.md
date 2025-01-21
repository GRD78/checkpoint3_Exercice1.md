
**Q.2.1.1** Sur le serveur, créer un compte pour ton usage personnel.

![cap16](https://github.com/user-attachments/assets/5bfc7cd1-735b-43a3-8382-f4c30020abaf)



**Q.2.1.2** Quelles préconisations proposes-tu concernant ce compte ?

![cap1](https://github.com/user-attachments/assets/bbc14446-e83f-4dab-bba5-c485a387532f)


**Q.2.2.1** Désactiver complètement l'accès à distance de l'utilisateur root.

![cap4](https://github.com/user-attachments/assets/72a66c75-082f-4e3d-a963-aa5f2996683a)


**Q.2.2.2** Autoriser l'accès à distance à ton compte personnel uniquement.

![cap6,1](https://github.com/user-attachments/assets/7dda4efc-98a0-4ebd-aa57-1fde026fa3af)


**Q.2.2.3** Mettre en place une authentification par clé valide et désactiver l'authentification par mot de passe

![cap18](https://github.com/user-attachments/assets/53325095-e2c3-4187-831c-d480080dd38c)


![cap2](https://github.com/user-attachments/assets/140f83ae-dd0c-465e-9cfc-ceae9b7e3969)

![cap7](https://github.com/user-attachments/assets/321e18b8-faa5-41e3-9e2b-135f54c2074c)

![cap8](https://github.com/user-attachments/assets/a01e4b23-38fd-4a51-92d2-000e827cb5d0)


**Q.2.3.1** Quels sont les systèmes de fichiers actuellement montés ?

![cap9](https://github.com/user-attachments/assets/5653b5ad-e92e-4fe5-9a89-1e4f61449d0c)


**Q.2.3.2** Quel type de système de stockage ils utilisent ?

![cap10](https://github.com/user-attachments/assets/1f58983e-d031-494a-b072-f2d6125d09af)


**Q.2.3.3** Ajouter un nouveau disque de 8,00 Gio au serveur et réparer le volume RAID

![cap10,1](https://github.com/user-attachments/assets/ba7f998b-86d6-4982-9f80-e92fbe2fa3ce)

![cap11](https://github.com/user-attachments/assets/02193204-9f78-4d79-beaf-bbcdc6256541)

![cap12](https://github.com/user-attachments/assets/119086c8-06cc-4f50-8e0a-8f369757449d)


**Q.2.3.4** Ajouter un nouveau volume logique LVM de 2 Gio qui servira à héberger des sauvegardes. Ce volume doit être monté automatiquement à chaque démarrage dans l'emplacement par défaut : /var/lib/bareos/storage.

![cap20](https://github.com/user-attachments/assets/078d9ce0-cdd8-4cd8-a1b7-337802ed3374)



**Q.2.3.5** Combien d'espace disponible reste-t-il dans le groupe de volume ?



**Q.2.4.1** Expliquer succinctement les rôles respectifs des 3 composants bareos installés sur la VM.

bareos-sd (Storage Daemon) :

Gestion du stockage : Le Storage Daemon est responsable de la gestion physique du stockage des données de sauvegarde.

 bareos-fd (File Daemon) :

Agent sur les clients : Le File Daemon est installé sur les machines clientes dont les données doivent être sauvegardées.

 bareos-dir (Director) :

Le chef d'orchestre : Le Director est le cœur de Bareos. Il est responsable de la gestion et de la coordination de toutes les opérations de sauvegarde, de restauration, de vérification et d'archivage.


**Q.2.5.1** Quelles sont actuellement les règles appliquées sur Netfilter ?

![cap13](https://github.com/user-attachments/assets/02ead8ae-a6c1-4a58-bbc4-a88c597e649a)


**Q.2.5.2** Quels types de communications sont autorisées ?

Trafic provenant de la machine locale (interface `lo`).

Connexions SSH sur le port 22 TCP.

Pings et autres paquets ICMP pour IPv4 et IPv6.

Trafic établi ou en réponse à des connexions initiées par le serveur.


**Q.2.5.3** Quels types sont interdit ?

Les connexions entrantes non spécifiées (HTTP, FTP,).

Les paquets invalides ou mal formés.


**Q.2.5.4** Sur nftables, ajouter les règles nécessaires pour autoriser bareos à communiquer avec les clients bareos potentiellement présents sur l'ensemble des machines du réseau local sur lequel se trouve le serveur.

![cap14](https://github.com/user-attachments/assets/fdcb6b56-376a-4e9c-ad23-d593b249e54f)



**Q.2.6.1** Lister les 10 derniers échecs de connexion ayant eu lieu sur le serveur en indiquant pour chacun :

* La date et l'heure de la tentative  
* L'adresse IP de la machine ayant fait la tentative

![cap15](https://github.com/user-attachments/assets/5acc337d-edcc-444f-ac49-b20dda8ca573)


  
