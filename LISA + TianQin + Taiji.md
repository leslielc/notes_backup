#### To do list 2

# Joint Angular Resolution

#### 主要问题

1. 分类？1、2、3、4类？

monochromatic、BBH、**SMBHB**、EMRIs

2. 要不要对很多位置统计10000+ 太慢 —— 超算
3. sensitivity curve: LISA —— 还是想看TDI，不过老师说的$\frac{1}{s_{total}}=\frac{1}{s_{chnnel1}} + \frac{1}{s_{chnnel2}}$ 也挺有道理的——应该是对的，可是还相当于2个转了45度的LIGO吗？
4. LISA+TianQin比LISA/TianQin好多少，LISA+Taiji比LISA好多少



#### 次要问题

1. 都算什么？角分辨率（两个？、三个？；**固定20°？40°？**；按时间算？；画天区图？SNR和定位精度？）
2. 天琴只能3个月，适合持续时间短的源（SMBH）
3. 去看天琴3.54是不是可以再准确些
4. LISA和TAIJI反着怎么样哈哈？ 反正那个alph_0角的区别已经凉了，**一个探测器如果考虑两条臂在同一个平面内已经完备了，无论再怎么原地自转**（For a fixed detector plane, $A_1^2+A_2^2$ = Const, no matter the rotation angle of the detector）
5. f要不要截断？
6. 可以考虑+椭率——轨道椭率影响到达时间(多普勒)，和位置LISA-Taiji[12]
7. **还有那些导数项对角度求不求导？(TianQin求了一些)**
8. 编程的问题：【1】数值的那个我还没算对呢！！！！角度那个我也没算对呢！！！【2】6里求导的问题【3】class封装设计得好一些【4】+PN【5】+轨道椭率的问题【6】天区图 【7】然而class好像更慢，我也不知道我改的好不好，标准在哪里？class怎么区分【8】我想要个成品看一看



#### NOTE：

天琴3.65 一圈，实际3.65/4就是一个周期了





# LISA

Baseline: $2.5\times10^6 km$ [LISA 2017]







# TianQin

Baseline: $1.7\times10^5 km$ [ Xin-Chun Hu et al. 2018, Jun Luo et al 2016 ]

Geocentric distance:  $1 \times10^5 km$ 



stable Period : 3 moths $\times$ 2 because of sunlight





# Taiji

Baseline: $3\times10^6 km$ [Lisa 2017]

### sensitivity curve

算Taiji的

##### Taiji Program: Gravitational-Wave Sources

https://arxiv.org/pdf/1807.09495.pdf

用到:

##### The Gravitational Wave Observatory Designer: Sensitivity Limits of Spaceborne Detectors

https://arxiv.org/abs/1411.1260