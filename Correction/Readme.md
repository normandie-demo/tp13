# Correction TP 13


## Créer un fichier vault *mysql.yaml* contenant les mots de passe root *old_pass* et *new_pass*

```Shell
ansible-vault create mysql.yaml
```

Copier le contenu:

```
old_pass: testPASS123
new_pass: testPASS456
```

## Créer un Playbook *rotate.yaml*

```Shell
vi rotate.yaml
```

## Exécuter le Playbook

```Shell
ansible-playbook -i inventory rotate.yaml --ask-vault-pass
```
