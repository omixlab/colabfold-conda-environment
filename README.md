# Colabfold Conda Environment 

```yaml
name: colabfold
channels:
  - conda-forge
  - bioconda
dependencies:
  - python=3.7
  - pip
  - pip:
    - "colabfold[alphafold] @ git+https://github.com/sokrypton/ColabFold"
    - -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
  - kalign2=2.04
  - hhsuite=3.3.0
  - openmm=7.5.1
  - pdbfixer
```

Install the ["ColabFold"](https://github.com/sokrypton/ColabFold) Alphafold distribution locally using `conda`.

```bash
(base) $ git clone https://github.com/omixlab/colabfold-conda-environment
(base) $ cd colabfold-conda-environment
(base) $ conda env create
```

After installing, just activate the environment using the command `conda activate colabfold` and start modelling!
