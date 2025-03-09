## **Poetry**

### Deux fichiers :
* pyproject.toml, composé de :
  * tool.poetry : les "meta données du projet"
  * tool.poetry.dependencies : les dépendances du côté utilisateur
  * tool.poetry.dev-dependencies : les dépendances du côté dev

<span style="color: #F00">Mais alors, pourquoi utiliser différentier les dépendances utilisateurs des dépendances développeur ?</span>

Le fait de différentier les dépendances permet aux développeurs d'utiliser d'autres dépendances, afin de tester de nouvelles fonctionnalités sans forcément avoir à les implémenter aux utilisateurs.

* poetry.lock : Définit et fige les versions des dépendances avec lesquelles le projet fonctionne afin d'éviter des conflits de versions en cas d'updates.

### Des commandes :

*Pour créer / activer un environnement :*
* poetry_shell

*Pour pouvoir visualiser les différentes dépendances sous forme "d'arbre" :*
* poetry_show --tree

*Pour installer les dépendances :*
* poetry_install

*Pour build son application :*
* poetry_build : génère deux fichiers représentant le projet sous forme de livrables

*Pour publier son application (dans un repository préalablement configuré) :*
* poetry_publish -r mon-depository

*Pour exécuter du code python :*
* poetry_run python le_script.py


---

[La source](https://www.hymaia.com/blog/poetry-enfin-loutil-pour-charmer-python)
