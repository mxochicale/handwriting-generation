Dependencies
---


# Anaconda installation 

Check the lastest version of Anaconda at https://repo.anaconda.com/archive/ (See more [ [1] (sep2018) ](https://www.ceos3c.com/open-source/install-anaconda-ubuntu-18-04/), [ [2] ](https://linuxhint.com/install_anaconda_python_ubuntu_1804/)).

```
cd ~/Downloads
wget https://repo.anaconda.com/archive/Anaconda3-5.3.0-Linux-x86_64.sh #04 November 2018 ## Length: 667822837 (637M) 
md5sum Anaconda3*.sh
bash Anaconda3*.sh #ENTER/yes/yes/no
source ~/.bashrc
#rm Anaconda3*.sh #don't delete in case of reinstallation
```


# Setting up virtual environment

* create conda virtual environment
```
cd
conda create -n hwgo python=3.6 pip numpy #remember to initialize the env with pip here.
```

* activate the virtual environment and install dependencies
```
conda activate hwgo
conda install -c conda-forge matplotlib 
conda install lxml #for `import xml.etree.cElementTree as ElementTree`

##installing tensorflow
conda install -c anaconda tensorflow-gpu


#seaborn #--is a Python visualization library based on matplotlib. 
#It provides a high-level interface for drawing attractive statistical graphics.
conda install -c anaconda seaborn 

##installing jupyter
#conda install nb_conda #install nb_conda for easily managing/switching notebook kernel
#conda install -c conda-forge jupyter #running: jupyter notebook
```


* deactivate your tensorflow conda env 
```
conda deactivate
conda deactivate
```



# References
Anaconda [:link:](https://www.anaconda.com/).


