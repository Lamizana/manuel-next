# NEXT Mode d'emploi

Pour une documentation complète, visitez [mkdocs.org](https://www.mkdocs.org).

## Commandes

* `mkdocs new [nom-dossier]` - Créez un nouveau projet.
* `mkdocs serve` - Démarrez le serveur de documentation avec rechargement en direct.
* `mkdocs build` - Générez le site de documentation.
* `mkdocs -h` - Affichez le message d'aide et quittez.

```bash
> mkdocs serve --dev-addr=127.0.0.1:8001    # Lance le serveur.
> mkdocs build                              # Génére le site de documentation.
```

## Structure du projet

```text
    mkdocs.yml    # Le fichier de configuration.
    docs/
        index.md  # La page d'accueil de la documentation.
        ...       # Autres pages markdown, images et autres fichiers.
```

Voici la liste des thèmes disponibles par défaut avec MkDocs :

```text
    mkdocs (thème par défaut)
    readthedocs
    material (nécessite une installation supplémentaire)
    windmill
    slate
    cyborg
    simplex
    superhero
    united
    cosmo
    yeti
    cerulean
    flatly
    journal
    lumen
    paper
    sandstone
    spacelab
```
