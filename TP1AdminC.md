# Questions Préparatoires

## `addition.py`

Ce code définit une fonction `add(x, y)` qui prend en entrée deux nombres et retourne leur somme.
Si le script est exécuté directement (`__name__ == '__main__'`), il demande deux nombres à l'utilisateur, les additionne et affiche le résultat.

## Questions

1. **À quoi sert `requirements.txt` ?**  
   Il contient la liste des dépendances nécessaires pour exécuter un projet Python. Il permet d'installer toutes les bibliothèques requises avec `pip install -r requirements.txt`.  
   **Source:** [FreeCodeCamp](https://www.freecodecamp.org/news/python-requirementstxt-explained/)

2. **À quoi ressemble un module en Python ?**  
   Un module est simplement un fichier Python (`.py`) contenant des fonctions ou des classes réutilisables. Exemple :
   ```python
   # module: addition.py
   def add(x, y):
       return x + y
   ```

3. **À quoi ressemble un package ?**  
   Un package est un dossier contenant un ou plusieurs modules et un fichier `__init__.py`. Exemple :
   ```
   my_package/
   ├── __init__.py
   ├── addition.py
   ├── multiplication.py
   ```
   **Source:** [Python Doctor](https://python.doctor/page-python-modules-package-module-cours-debutants-informatique-programmation)

4. **Créer un code Python utilisant `addition.py` sous forme de module**
   ```python
   import addition
   
   x = 30
   y = 11
   res = addition.add(x, y)
   print(res)
   ```

5. **À quoi sert `pip` ?**  
   `pip` est le gestionnaire de paquets de Python. Il permet d’installer, mettre à jour et supprimer des bibliothèques.

6. **À quoi sert `PYTHONPATH` ?**  
   `PYTHONPATH` est une variable d’environnement qui indique à Python où chercher les modules et packages lorsqu'ils sont importés.

7. **Où sont stockés les paquets installés par `pip` ?**  
   Ils sont stockés dans le dossier `site-packages` de l’environnement Python utilisé.
   - Sous Linux/macOS : `~/.local/lib/pythonX.X/site-packages/`
   - Sous Windows : `C:\Users\<nom_utilisateur>\AppData\Local\Programs\Python\PythonXX\Lib\site-packages\`

8. **À quoi sert `pip install --user` ?**  
   Il installe les paquets uniquement pour l’utilisateur courant, sans nécessiter de privilèges administratifs.

9. **À quoi sert `venv` ?**  
   `venv` permet de créer un environnement virtuel isolé pour installer des paquets sans affecter le système global.

10. **Comment utiliser `venv` ?**  
    ```bash
    python -m venv mon_env
    source mon_env/bin/activate  # Linux/macOS
    mon_env\Scripts\activate  # Windows
    ```

11. **À quoi sert Docker ?**  
    Docker permet de créer, déployer et exécuter des applications dans des conteneurs isolés.

12. **Comment utiliser Docker ?**  
    ```bash
    docker pull python
    docker run -it python
    ```

Sources interessantes:

**Python Unittest (Tests unitaires)**  
   [https://docs.python.org/3/library/unittest.html](https://docs.python.org/3/library/unittest.html)  

**PEP 8 – Guide de style Python**  
   [https://peps.python.org/pep-0008/](https://peps.python.org/pep-0008/)  

**Python Packaging (Créer et publier un package sur PyPI)**  
   [https://packaging.python.org/en/latest/tutorials/packaging-projects/](https://packaging.python.org/en/latest/tutorials/packaging-projects/)  

**Python Logging (Gestion des logs en Python)**  
   [https://docs.python.org/3/library/logging.html](https://docs.python.org/3/library/logging.html)  

**Pytest (Alternative plus avancée à Unittest)**  
   [https://docs.pytest.org/en/latest/](https://docs.pytest.org/en/latest/)  

**Gestion des environnements virtuels avec `venv`**  
   [https://docs.python.org/3/library/venv.html](https://docs.python.org/3/library/venv.html)

# Exercices

**Ex.3**
Utilisation de black.
Mon fichier a ete corrige pour remplacer les tabs par 4 espaces (d'apres Pep8), 
et egalement placer un espace a chaque second element d'un tuple (a, b).