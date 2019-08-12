0. **nvidia driver**
```
sudo apt-get remove –purge nvidia*
sudo chmod a+x NVIDIA-Linux-x86_64-375.20.run

sudo ./NVIDIA-Linux-x86_64-375.20.run –no-x-check –no-nouveau-check –no-opengl-files
```
–no-x-check 安装驱动时关闭X服务
–no-nouveau-check 安装驱动时禁用nouveau
–no-opengl-files 只安装驱动文件，不安装OpenGL文件

安装CUDA时一定使用runfile文件，这样可以进行选择。不再选择安装驱动，以及在弹出xorg.conf时选择NO
不要使用ubuntu设置中附加驱动中驱动

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
**noticed the numpy version should use 1.14.5**


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
