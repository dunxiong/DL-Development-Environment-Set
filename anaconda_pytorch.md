1. **Anaconda install**

download anaconda (.sh file) from the web set and then install it using the following code
```
sh filename.sh

source ~/.bashrc
```
2. **Pytorch install**
```
conda install pytorch=0.3 -c soumith
conda install torchvision
conda install tqdm
```
3. **bashrc set**
```
export PATH="/your anaconda local path/bin:$PATH"

alias py2 ="/usr/bin/python2.7"
alias py3 ="/usr/bin/python3.5"
alias pya ="~/anaconda3/bin/python3.6"
```