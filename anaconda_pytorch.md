1. **Anaconda install**

download anaconda (.sh file) from the web set and then install it using the following code
```
sh filename.sh

source ~/.bashrc

conda create -n deep python=3.6 pandas numpy matplotlib jupyter notebook   #set virtual environment name and load some packages
```
```
source activate deep   # active deep 

deactivate deep

```
2. cuda and cudnn instation in virtual env using anaconda

```
conda install -c anaconda cudatoolkit = 8

conda install -c anaconda cudnn = 6
```



3. **Pytorch install**
```
conda install pytorch=0.3 -c soumith
conda install torchvision
conda install tqdm
```
4. **bashrc set**
```
export PATH="/your anaconda local path/bin:$PATH"

alias py2 ="/usr/bin/python2.7"
alias py3 ="/usr/bin/python3.5"
alias pya ="~/anaconda3/bin/python3.6"
```
