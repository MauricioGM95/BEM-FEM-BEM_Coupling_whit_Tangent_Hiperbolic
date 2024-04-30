# BEM-FEM-BEM_Coupling_with_Tangent_Hiperbolic
An alternative to calculate the coupling of BEM-FEM-BEM with variable permittivity using the hyperbolic tangent as a model, applied for different types of solutes.

### File creation
To calculate the solvation or binding energy for each solute, you must first create the following files in this order:
- We first create the `.pqr` files for each solute, where the `Creation_of_PQR_files_General.ipynb` code is executed.
- After generating the `.pqr` files, the code `Creation_of_Surface_Meshes_General.ipynb` is used to generate the surface meshes of each solute.
- Then of generating the surface meshes, the code `Creation_of_Volumetric_Meshes_General.ipynb` is used to generate the volumetric meshes of each solute.
- Finally with the volumetric meshes, the code `Creation_Alpha_files_General.ipynb` must be executed to generate the text files of the alpha geometric parameter of each solute to work with the variable permittivity model.

### Calculation of solvation energy
To calculate the solvation energy of a particular solute, only the available codes are executed:
- `BEM_BEM_Coupling.ipynb`
- `BEM_BEM_BEM_Coupling.ipynb`
- `BEM_FEM_BEM_Coupling_(Variable_Permittivity).ipynb`
- `BEM_BEM_Coupling_(Cavity).ipynb`
- `BEM_FEM_BEM_Coupling_(Cavity)_(Variable_Permittivity).ipynb`

Additionally, the `Iterative_Code_HT_Mobley.py`, `Iterative_Code_HT_TanH_Sphere.py` and `Iterative_Code_HT_Binding_Energy.py` codes are an alternative to calculate the energy of each solute iteratively instead of individually.

### Calculation of Coulomb energy
In the `Addition_codes.ipynb` code, there is the information to calculate the coulomb energy of the ligand-proteins and then calculate the binding energy.

# Pendiente 
1. Corregir posibles detalles del README
2. Corroborar resultados de cavidad BFB en el paper
   
### Opcional
1. Excel
2. Caso de visualizacion de graficos del paper
3. Visualizacion corte BFB
