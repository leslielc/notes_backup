# 超算

### Terminal连

ssh 1801110215@162.105.133.134



### 登录口运行

module load anaconda/3.7.1

source activate pycbc_env





sbatch - Submit a batch script to Slurm.

1.单个运行没有问题，2.标明你要导出储存的具体数据，3. 多线程运行的参数空间

收费标准：http://hpc.pku.edu.cn/guide_6.html

指南：http://hpc.pku.edu.cn/_book/guide/slurm/slurm.html

### 在teminal里输入（http://hpc.pku.edu.cn/_book/guide/soft_env/python.html）

module load anaconda/3.7.1



conda create -n pycbc_env python=3.7



source activate pycbc_env



conda install pip



pip install lalsuite pycbc



### 在文件夹的run.sh输入：

\#!/bin/bash

\#SBATCH --qos=low

\#SBATCH -p C032M0128G

\#SBATCH -A hpc1806187115

\#SBATCH -J Multi

\#SBATCH --get-user-env

\#SBATCH --nodes=1

\#SBATCH --ntasks-per-node=32

\#SBATCH --mail-type=END,FAIL

\#SBATCH --mail-user=1801110215@pku.edu.cn

\#SBATCH --time=24:00:00



module load anaconda/3.7.1

source activate pycbc_env

python main.py

### 之后去文件夹里

sbatch run.sh

### 之后看看是不是在排队

squeue -u 1801110215



### 从远程下下来

scp 1801110215@162.105.133.134:~/multi/data.hdf5 .

以下scp粘到本地还是远程忘记了

scp -r ./Project 1801110215@162.105.133.134:~

### 网页版

wpn.pku.edu.cn

ssh

学号@162.105.133.134

