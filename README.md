# NEXT Mode d'emploi

---

## Commandes

* `mkdocs new [nom-dossier]` - Créez un nouveau projet.
* `mkdocs serve` - Démarrez le serveur de documentation avec rechargement en direct.
* `mkdocs build` - Générez le site de documentation.
* `mkdocs -h` - Affichez le message d'aide et quittez.

```bash
> mkdocs serve --dev-addr=127.0.0.1:8001    # Lance le serveur.
> mkdocs build                              # Génére le site de documentation.

```

---

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

---

## Déploiement

```bash
mkdocs gh-deploy --clean
```

Le site est actuellement sur : <https://lamizana.github.io/manuel-next/>.

---

## Personnaliser le footer Mkdocs

1. Crée un dossier **overrides/** à la racine de ton projet

  ```bash
  mkdir overrides
  ```

1. Dans ce dossier, crée le chemin

  ```bash
  overrides/main.html
  ```

1. Ajoute ce contenu dans overrides/main.html

  ```html
  {% extends "base.html" %}

  {% block footer %}
  <!-- Footer désactivé -->
  {% endblock %}
  ```

1. Dans ton mkdocs.yml, indique l’override

  ```yaml
  theme:
    name: mkdocs  # ou readthedocs
    custom_dir: overrides
  ```
