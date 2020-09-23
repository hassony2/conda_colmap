# Instructions for local build of colmap using anaconda

```sh
conda build recipe -c conda-forge -c anaconda
conda create -n colmap_local -c conda-forge -c anaconda
conda activate colmap_local
conda install --use-local colmap -c conda-forge -c anaconda
```
