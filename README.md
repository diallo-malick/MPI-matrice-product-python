# MPI-matrice-product-python
Ce programme effectue le produit de matrices par blocs.

Pour l'utilisation du code vous avez besoin d'installer Python, numpy et MPI 
- ## Guide d'installation MPI sous window : 
1) Télécharger et installer MPI 10 pour Windows à l’adresse: [MPI](https://www.microsoft.com/en-us/download/details.aspx?id=57467)
2) Ouvrir une fenêtre PowerShell. Utiliser la recherche Windows pour trouver comment faire,  puis:
  - Entrer la commande python, ou python3, Windows ouvre directement la page Windows Store pour télécharger et installer la dernière version de python
  Une fois python installé, installer les modules numpy et mpi4py avec pip:
    - pip install numpy
    - ip install mpi4py
Les phases 1 et 2 sont indépendantes, vous pouvez les faire dans n’importe quel ordre. Ce n’est pas la peine de réinstaller le python3 de Microsoft si vous l’avez déjà fait. Il suffir d’installelr les modules manquants.

- ## Guide d'installation MPI sous Linux :
- 1) Il suffit juste de faire:
  - pip install numpy
  - ip install mpi4py
## Pour exécuter le programme avec 4 processeurs tapez:
mpiexec -n 6 python Produit_matrice_matrice.py
Par défaut la taille des matrices est 12x12, vous pouvez lancer le programme avec un argument qui vas sera la dimension de la matrice.
Par exemple pour initialiser une matrice de dimension 6x6 exécuter:
  mpiexec -n 6 python Produit_matrice_matrice.py 6
  
