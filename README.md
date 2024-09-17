<div align="center">

# Procédure pour causer un conflit de fusion

</div>

![image](https://github-production-user-asset-6210df.s3.amazonaws.com/133788665/341078991-e59b2850-64cf-49b9-be71-e0f98e98661e.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAVCODYLSA53PQK4ZA%2F20240911%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20240911T222202Z&X-Amz-Expires=300&X-Amz-Signature=583ad66ce7f83f248e2da78d39def6af271f0c586c031d454f5d57743a774b29&X-Amz-SignedHeaders=host&actor_id=133788665&key_id=0&repo_id=687440473)




Suivez les étapes ci-dessous une par une :

1. Clonez ce dépôt localement.
2. Dans le répertoire du dépôt local, créez un fichier `README2.md` contenant vos prédictions sur les finalistes de la Ligue des Champions.
3. Créez un commit initial sur la branche `main` et poussez-le sur GitHub.
4. Créez une branche `branche1` à partir de `main`.
5. Vérifiez que vous êtes bien sur la branche `branche1`.
6. Dans la branche `branche1`, modifiez le fichier `README2.md` avec vos nouvelles prédictions pour les finalistes. Créez un commit avec le message "modif finaliste 1" et poussez les modifications de `branche1` sur GitHub.
7. Revenez à la branche `main`.
8. Créez une branche `branche2` à partir de `main`.
9. Dans la branche `branche2`, modifiez également les noms des finalistes saisis à l'étape 6. Créez un commit avec le message "modif finaliste 2" et poussez les modifications de `branche2` sur GitHub.
10. Revenez à la branche `main`.
11. Fusionnez `branche1` dans `main`.
12. Poussez les modifications vers le dépôt distant.
13. Fusionnez `branche2` dans `main`.
14. Poussez les modifications vers le dépôt distant.
15. Résolvez le conflit de fusion localement, puis poussez les modifications résolues vers le dépôt distant.

Si vous avez suivi cette procédure correctement, vous devriez obtenir un conflit de fusion :

```
Auto-merging README2.md
CONFLICT (content): Merge conflict in README2.md
Automatic merge failed; fix conflicts and then commit the result.
```

La commande `git status` devrait afficher :

```
On branch main
You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Unmerged paths:
  (use "git add <file>..." to mark resolution)

        both modified:   README2.md
```

### Procédure pour résoudre un conflit de fusion

Pour résoudre ce conflit, suivez les étapes suivantes :

1. Ouvrez le fichier `README2.md` et résolvez les conflits en conservant les modifications souhaitées.
2. Ajoutez le fichier résolu avec la commande `git add README2.md`.
3. Créez un commit avec un message approprié pour indiquer la résolution du conflit.
4. Poussez les modifications résolues vers le dépôt distant.

Après avoir résolu le conflit de fusion, la commande `git status` devrait afficher :

```
On branch main
nothing to commit, working tree clean
```

Pour plus de détails sur la résolution des conflits, vous pouvez consulter la [ressource Classroom pour la résolution de conflit lors d'un merge](https://openclassrooms.com/fr/courses/7688581-devenez-un-expert-de-git-et-github/7851552-resolvez-les-conflits-avec-git).
