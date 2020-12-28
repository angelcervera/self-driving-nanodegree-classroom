# Self-Driving Car Engineer
Nanodegree Program - Classroom

- [Lesson 4 notes](lesson4/README.md)



## Anaconda in Fish and ubuntu.
From: https://docs.anaconda.com/anaconda/install/linux/

1. Install required packages (Usually, it's installed)
   ```shell
    apt-get install libgl1-mesa-glx libegl1-mesa libxrandr2 libxrandr2 libxss1 libxcursor1 libxcomposite1 libasound2 libxi6 libxtst6
    ```
2. Add Anaconda binaries and scripts to the PATH:
    ```shell
    set -U fish_user_paths /home/angelcc/apps/anaconda3/bin $fish_user_paths
    ```
2. Update the `config.fish` file to prepare the environment at starting point:
    ```shell
    /home/angelcc/apps/anaconda3/bin/conda init fish
    ```
3. Restart the system.

## Anaconda basic commands.
Full documentation at https://conda.io/projects/conda/en/latest/commands.html
```shell
conda create -n ENV [python=X.X] [LIST_OF_PACKAGES]
conda env list
conda info --envs

conda activate ENV

conda list
conda search *SEARCH_TERM*
conda install PACKAGE_NAME
conda install PACKAGE_NAME==VERSION
conda update PACKAGE_NAME
conda update --all
conda remove PACKAGE_NAME

conda env export > environment.yaml

conda deactivate

conda list -n ENV

conda env create -f environment.yaml

conda env remove -n ENV
```

## Jupiter notes
Install `nb_conda` in the conda virtual environment to have the `Conda` tab.
```shell
conda install nb_conda
```

Links:
- List of [Jupyter built-in magic commands](https://ipython.readthedocs.io/en/stable/interactive/magics.html)
- [Examples](https://jupyter-notebook.readthedocs.io/en/stable/examples/Notebook/examples_index.html)
- [Kernels](https://github.com/jupyter/jupyter/wiki/Jupyter-kernels)

## pipenv Environment
Don't use it in this course. Anaconda is the recommended.

- [Pipenv: A Guide to the New Python Packaging Tool](https://realpython.com/pipenv-guide/)

```shell
sudo apt install python3-pip
pip3 install pipenv

pipenv shell
pipenv install matplotlib==3.3.3
pipenv install pytest --dev

python3 -m venv venv
source venv/bin/activate.fish
pip install pipenv
pipenv shell --fancy


```
