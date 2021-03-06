# wgconf : Gestion serveur et clients Wireguard

Ce script bash a pour objet de configurer et de gérer les clients Wireguard sur un serveur Linux.

Voir les articles correspondants sur https://www.mikmer.fr :

[Installer Wireguard sur un Raspberry sous Raspbian](https://www.mikmer.fr/?p=148)

[Installer Wireguard sur un serveur Linux](https://www.mikmer.fr/?p=95#paqcomp)

## Pré-requis
Il faut :
- disposer d'un petit serveur Linux et d'un accès fibre optique : c'est indispensable pour avoir un débit correct.
- avoir une adresse IPv4 fixe
- avoir un accès root
- ouvrir le port Wireguard sur votre box (par défaut 51820) pour le rediriger vers le serveur Linux qui héberge Wireguard

## Utilisation
Voir le mode d'emploi sur le wiki :
[wgconf : script de configuration du serveur et de gestion des clients Wireguard](https://github.com/mikmer62/wgconf/wiki/wgconf-:-script-de-configuration-du-serveur-et-de-gestion-des-clients-Wireguard)

## Compatibilité
| Système                      | ? |
| ---------------------------- | - |
| Ubuntu 16.04                 | :question: |
| Ubuntu 18.04                 | :question: |
| Ubuntu 20.04 (Focal Fossa    | :white_check_mark: |
| Raspbian 10 (Buster)         | :white_check_mark: |

## A faire
- [ ] Support IPv6
- [ ] Vérification avec un firewall
- [ ] Vérification et support autres OS

## Auteur
Michel MERCIER

## Licence
Distribution open source mise à disposition sous licence MIT.
https://github.com/mikmer62/wgconf

[Voir la licence](Licence.md)
