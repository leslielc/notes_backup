https://docs.python.org/3/library/functions.html#enumerate

没事就看看

https://book.douban.com/subject/25779298/



# 安装

Pip list所有包

 pip list --outdated 

*#更新某个包*

 pip install --upgrade <packages-name>

pip install numpy=1.2.3

pip install --upgrade lalsuite pycbc

LALSimInspiral.h里有每个波形的说明



# Profiling

https://stackoverflow.com/questions/38358881/how-to-profile-multiple-subprocesses-using-python-multiprocessing-and-memory-pro

```sh
e.g.1 不需要在程序里面写什么
mprof run -M --include-children python main.py
%显示子进程和总内存占用
mprof run -M python main.py
%显示子进程和main（不加子进程）
mprof plot
%最后画一下刚刚生成的文件
```

```
e.g.2 写在程序里可以看每一行的占用：（我还没看）
```

https://www.cnblogs.com/kaituorensheng/p/5669861.html

# Healpy

https://github.com/gw-odw/odw-2018/blob/master/skymaps/Intro_to_Skymaps.ipynb

https://github.com/kadrlica/skymap/tree/master/tutorial healpy和skymap联动

```python
# Coordinate must be a string (G[alactic], E[cliptic], C[elestial] or Equatorial=Celestial)
```

theta从天顶算

phi从中间往左

## SKY MAP

https://dcc.ligo.org/public/0157/P1800381/006/plot_GWTC-1_skymaps.py

https://dcc.ligo.org/LIGO-P1800381/public

skymap https://github.com/kadrlica/skymap/tree/master/tutorial

healpy https://healpy.readthedocs.io/en/latest/tutorial.html   



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

