# devops
Rendu du projet de devops

## Prérequis
- 2 machines sous Debian9, dans notre cas nous utilisons vagrant, mais il est possible d'utiliser un autre environnement de virtualisation, tel [AWS](https://aws.amazon.com/fr/).
- Ansible sous licence Linux

## Mise en place

Copiez collez cette ligne dans votre terminal:
```
ansible-playbook playbook_wordpress.yml -i config-ip
```
Ce script à pour but d'installer sur les machines distantes: MySQL, Wordpress, apache2, php5.

Modifiez le fichier **config-ip** avec les IPs de vos machines et l'utilisateur   
Dans notre exemple, nous utiliserons l'ip 10.33.10.1 ( pour la BDD ) et 10.33.10.2 ( pour le WEB Server ).   
Pour ce qui est de l'utilisateur changez celui par celui que vous utilisez ansible_user=vagrant   
