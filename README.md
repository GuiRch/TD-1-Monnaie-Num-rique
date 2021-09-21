# TD 1 Monnaie Numérique

## Setting up SSH properly

Dans un premier temps on crée une clé publique et un clé privée RSA sur notre machine avec les outils Putty (dans le cas d'une machine sous windows).
![putty gen](https://user-images.githubusercontent.com/62909821/134141715-b77ce04a-485c-4f60-96de-7b0138d46616.PNG)
On stocke ensuite les clés privée et publique dans deux fichiers différents sur l'emplacement de notre choix. On pensera à bien sécuriser le fichier contenant la clé privée, qui est l'information sensible.
![fichiers clés](https://user-images.githubusercontent.com/62909821/134142125-5fe64430-4999-4d82-9730-5f697af94d3d.PNG)

On créer ensuite un dossier caché `.ssh` à la racine de la machine virtuelle. Dans ce dossier on crée un fichier `authorized_keys` dans lequel on colle la clé ssh. Une fois ce dossier sécurisé avec la commande `chmod -R 700 .ssh/` on peut se connecter via ssh depuis Putty en indiquant l'emplacement de la clé ssh sur notre machine physique.

Il est également possible de désactivé la connexion via mot de passe sur la machine virtuelle pour n'utiliser que la connexion via ssh sur la machine virtuelle. Il faut être prudent en réalisant cette opération et s'assurer que la connexion par ssh fonctionne bien avant de désactiver la connexion par mot de passe.

## Setting up UFW and Fail2Ban 

### UFW 
 
### Fail2Ban

Fail2ban permet de contrer les attaques par forces brute en bloquant les tentatives de connexion après un certain nombre tentatives de connexions avec un mot de passe éronné.
L'installation de fail2Ban se fait facilement avec la commande `sudo apt install fail2ban`, puis en utilisant la configuration par défault de fail2ban.

## Installing Bitcoind 

## Turning BitcoinD into a service 

## Creating a wallet and depositing tBTC in it 

## Installing LND

## Turning LND into a service

## Opening a lightning channel

## Setting up Tor

## Running your own BTC explorer
