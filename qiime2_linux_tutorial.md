## Installing QIIME2 on linux and using jupyter notebook for analysis

### conda
open a shell and run these three commands
```
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh -b
~/miniconda3/bin/conda init
```
exit and reopen shell 
```
conda update conda -y
wget https://data.qiime2.org/distro/core/qiime2-2020.2-py36-linux-conda.yml
conda env create -n qiime2-2020.2 --file qiime2-2020.2-py36-linux-conda.yml
rm rm qiime2-2020.2-py36-linux-conda.yml
source activate qiime2-2020.2
qiime --help
```

### moving pictures tutorial
https://docs.qiime2.org/2020.2/tutorials/moving-pictures/
```
wget https://github.com/voidlogic/QIIME2_jupyter_tutorials/blob/master/QIIME2_MovingPicturesTutorial.ipynb
jupyter notebook QIIME2_MovingPicturesTutorial.ipynb
```
