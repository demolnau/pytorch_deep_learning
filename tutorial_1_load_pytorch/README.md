# Tutorial #1
1. Install mamba using [miniforge3](https://github.com/conda-forge/miniforge?tab=readme-ov-file)

2. initiate mamba:
```
mamba init bash
```

3. Create a virtual environment using mamba
```
mamba create -n li-tutorial
mamba activate li-tutorial
mamba install pytorch::pytorch
mamba update -all
mamba install anaconda::jupyter
mamba install anaconda::numpy
mamba install -c anaconda ipykernel
mamba install -y -c conda-forge cudatoolkit
mamba install -c anaconda tensorflow-gpu keras-gpu
python -m ipykernel install --user --name=li-tutorial
```