Virtual Environments 
==========

Anaconda
--------

Check Conda if conda is installed and added to Path: ``conda -V``

Check if Conda needs to be upadated: ``conda update conda``

Create Venv: ``conda create -n name python=x.x anaconda``

Active Venv: ``source activate yourenvname``

Install specific packages: ``conda install -n name [package]``

Deactivate Venv: ``source deactivate``

Remove Venv: ``conda remove -n yourenvname -all``

Rename virutal environment: not possible but you can crate a clone via ``conda create --name new_name --clone old_name``

Python Venv 
-----

Create dictionary and cd to it 

Run: ``python3 -m venv <name_of_virtualenv>```

Anaconda reinstall
--------

1. go to website, download (don't add to Path)

2. ``Strg + Shift + P`` --> selcet python interpreter conda 

3. restart terminal 