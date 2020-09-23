# Colmap conda recipe

The main point of this repo is to provide a way to install COLMAP
without requiring sudo privileges to run it through the gui or the command
line interface.

Note that I am *not* a conda expert, there are therefore likely:
- unnecessary build dependencies
- over-strict pinning
- other traces of bad practices

# Building and installing colmap using anaconda

This builds and installs colmap **without** GPU support

```sh
conda build recipe -c conda-forge -c anaconda
conda create -n colmap_local -c conda-forge -c anaconda
conda activate colmap_local
conda install --use-local colmap -c conda-forge -c anaconda
```

# Launch 

## GUI

```sh
colmap gui
```

## CLI

```sh
colmap -h
```
