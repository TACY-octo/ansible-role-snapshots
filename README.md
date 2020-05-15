# Information 

Ce rôle à le statut "Développement". 
Certaines fonctionnalités ne peuvent peut-être pas fonctionner ou sont en cours d'amélioration. 
Vous pouvez contribuer à améliorer ce contenu en proposant vos modifications à partir d'un pull request. 

| Version | Statut | 
| ------- | ------------- | 
| 0.0.1   | Développement |


# Objectifs 

- [ ] Créer un snapshots 
- [ ] Supprimer un ou plusieurs snapshots
- [ ] Appliquer un snapshots (retour arrière)

# Variable 

```yml
# vars/main.yml
---
snapshots_esxi: ""
snapshots_user: ""
snapshots_password: ""
snapshots_datacenter: ""

```

# Utilisation 

Exemple de playbook : 

```yml 
# playbooks/main.yml
---
- hosts: all
  roles:
    - ansible-role-snapshots

```

# Requirement
- Installer le module ```pyvmomi``` sur le controlleur Ansible
```shell 
python -m pip install pyvmomi
```

# Supports 
- cyril.tavian@acensi.fr

# Nommage
Les variables ont en prefix le nom du rôle. ```snapshots_```
