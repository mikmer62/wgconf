# wgconf
Gestion serveur et clients Wireguard

Ce script bash a pour objet de configurer et de gérer les clients Wireguard sur un serveur Linux.

Il requiert dans cette version un serveur avec une IPv4 fixe et fonctionne sous Ubuntu 18.04, mais peut être testé sous d'autres versions ou OS de Linux.

Le retour utilisateurs permettra de mettre à jour le tableau de compatibilité.

## Utilisation
Pour obtenir une aide sur les commandes, taper :

```
> wgconf ?
USAGE
    wgconf <option> [<byip>] [nom_du_client]
    Le nom du client  ne doit pas contenir d'espace
OPTIONS
    init                        : Initialise les paramètres du serveur VPN
    addcli nom_du_client        : Ajoute le client nom_du_client
    delcli nom_du_client        : Supprime le client nom_du_client
    listcli                     : Affiche la liste des clients
    listcli byip                : Affiche la liste des clients triée par IP VPN
    listkeys                    : Affiche la liste des clé publiques et privées
    showcli nom_du_client       : Affiche le fichier de configuration du client
    showqrcode nom_du_client    : Affiche le qrcode du client
    raz                         : Supprime tous les clients et la configuration
```
## Initialisation
Lors de la première utilisation, il faut initialiser le fichier de configuration.

La commande d'initialisation est : 
> wgconf init

Le fichier créé se nomme "wgconf.params" et se trouve dans /etc/wireguard.

**Il ne doit pas être supprimé ni modifié.**

3 répertoires seront également créés :
```
/etc/wireguard/conf : contient les fichiers de configuration clients
/etc/wireguard/keys : contient les clés privées et publiques du serveur (wgserver) et des clients
/etc/wireguard/qrcode : contient les qrcode des clients en format jpg
```
## Ajout d'un client

