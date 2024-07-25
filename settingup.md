# Setting up software for the material from this i-CoMSE workshop:

### If you are participating in the workshop with Bridges2 on PSC
Running this command on Bridges2 will set up singularity images that can be used in jupyter notebooks through OnDemand:

```
bash /ocean/projects/see220002p/shared/icomse-setup.sh
```

### If you don't have an account on PSC
Most of the workshop functionality is provided through python libraries. If you wish to replicate the python environment from the container locally without gromacs use this [environment.yml](environment.yml):

```
conda env create -f environment.yml
conda activate icomseW23
```

And to get gromacs/plumed via conda:
```
	conda install --strict-channel-priority -c \
	    plumed/label/masterclass-2022 -c conda-forge plumed gromacs
```
