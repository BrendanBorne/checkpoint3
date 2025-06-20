# Exercice 2 - Manipulations pratiques sur VM Linux

## Partie 1 - Gestion des utilisateurs

**Q2.1.1**

Connecté en root, lancer la commande :

```bash
adduser perso
```

Entrer un mot de passe, et les informations de l'utilisateur.

**Q2.1.2**

Il peut être intéressant d'ajouter l'utilisateur au groupe sudo :

```bash
usermod -aG sudo perso
```

## Partie 2 - Configuration de SSH

**Q2.2.1 à 2.2.3**

Modifier le fichier de configuration ssh :

```bash
nano /etc/ssh/sshd_config
```

Avec les lignes suivantes :

```bash
PermitRootLogin no
AllowUsers perso
PubkeyAuthentication yes
PasswordAuthentication no
```

## Partie 3 - Analyse du stockage

## Partie 4 - Sauvegardes

## Partie 5 - Filtrage et analyse réseau

## Partie 6 - Analyse de logs