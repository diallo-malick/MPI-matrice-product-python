# MPI-matrice-product-python
Ce programme a été réalisé dans le cadre de l'UE  MU5MAI06 - S2  Calcul parallèle de François-Xavier Roux. IL effectue le produit de matrices par blocs.

Pour l'utilisation du code vous avez besoin d'installer Python, numpy et MPI 
- ## Guide d'installation MPI sous window : 
1) Télécharger et installer MPI 10 pour Windows à l’adresse: [MPI](https://www.microsoft.com/en-us/download/details.aspx?id=57467)
2) Ouvrir une fenêtre PowerShell. Utiliser la recherche Windows pour trouver comment faire,  puis:
  - Entrer la commande python, ou python3, Windows ouvre directement la page Windows Store pour télécharger et installer la dernière version de python
  Une fois python installé, installer les modules numpy et mpi4py avec pip:
    - `pip install numpy`
    - `pip install mpi4py`
Les phases 1 et 2 sont indépendantes, vous pouvez les faire dans n’importe quel ordre. Ce n’est pas la peine de réinstaller le python3 de Microsoft si vous l’avez déjà fait. Il suffir d’installelr les modules manquants.

- ## Guide d'installation MPI sous Linux :
1) Il suffit d'ouvrir le terminal et installer les deux modules en tapant: 
  - `pip install numpy`
  - `pip install mpi4py`
#### Pour exécuter le programme avec 4 processeurs tapez:
`mpiexec -n 4 python Produit_matrice_matrice.py`
- Par défaut la taille des matrices est 12x12, vous pouvez lancer le programme avec un argument qui vas sera la dimension de la matrice.
Par exemple pour initialiser une matrice de dimension 6x6 exécuter:
  `mpiexec -n 4 python Produit_matrice_matrice.py 6`
  
