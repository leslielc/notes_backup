https://docs.python.org/3/library/functions.html#enumerate

没事就看看

https://book.douban.com/subject/25779298/



# 超算

ssh 1801110215@162.105.133.134

module load anaconda/3.7.1



conda create -n myenv python=3.7

scp

scp -r ./Project 1801110215@162.105.133.134:~

sbatch





$\begin{equation*} P(r, \vec{n}_i) dr = \rho_i \frac{\hat{N}_i}{\sqrt{2\pi}\hat{\sigma}_i} \text{exp} \left[-\frac{(r-\hat{\mu}_i)^2}{2\hat{\sigma}_i^2} \right] r^2 dr \end{equation*}$



# 安装

Pip list所有包

 pip list --outdated 

*#更新某个包*

 pip install --upgrade <packages-name>

pip install numpy=1.2.3

pip install --upgrade lalsuite pycbc

#### Conda install 的官网



# Healpy

https://github.com/gw-odw/odw-2018/blob/master/skymaps/Intro_to_Skymaps.ipynb

https://github.com/kadrlica/skymap/tree/master/tutorial healpy和skymap联动

```
Coordinate must be a string (G[alactic], E[cliptic], C[elestial] or Equatorial=Celestial)
```

theta从天顶算

phi从中间往左

## SKY MAP

https://dcc.ligo.org/public/0157/P1800381/006/plot_GWTC-1_skymaps.py

https://dcc.ligo.org/LIGO-P1800381/public



## 求导和差值

splrep splev https://docs.scipy.org/doc/scipy/reference/generated/scipy.interpolate.splev.html https://docs.scipy.org/doc/scipy/reference/generated/scipy.interpolate.splrep.html splprep



## 计时

```python
import time
time_start = time.time() #开始
```

```python
time_end = time.time()
print('time: ', (time_end - time_start)/60,np.mod(time_end - time_start, 60)) # 以秒为单位  
```

