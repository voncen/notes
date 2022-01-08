<div style='display: none'>
考完试再来看这个实在是写得太幼稚了，也不想整理了，就这样封存起来吧
</div>
[https://zhuanlan.zhihu.com/p/58808753]()
$\nabla$ 只对$r$ 作用，视$r'$ 为常数，故$\nabla r'=0$

$$
\begin{array}{l|l}
\nabla \cdot \vec{E}=\frac{\rho}{\varepsilon_{0}} & \nabla \cdot \vec{D}=\rho_{f} \\
\nabla \times \vec{E}=-\frac{\partial \vec{B}}{\partial t} & \nabla \times \vec{E}=-\frac{\partial \vec{B}}{\partial t} \\
\nabla \cdot \vec{B}=0 & \nabla \cdot \vec{B}=0 \\
\nabla \times \vec{B}=\mu_{0} \vec{J}+\mu_{0} \varepsilon_{0} \frac{\partial \vec{E}}{\partial t} & \nabla \times \vec{H}=\vec{J}_{f}+\frac{\partial \vec{D}}{\partial t} \quad \star[i]
\end{array}
$$
左边就是一个最原始的通用方程,在任何时候都是成立的.右边是为了方便运算人为制造了一些辅助矢量使得方程组形式更优美/处理介质影响更方便罢了.
#### 基本

任何情况都成立：$\nabla \cdot \vec{B}=0$  
恒定磁场：$\nabla \times\ \vec{B}=\mu_0\vec{J}$  恒定磁场总是无源的（因为磁荷不存在）：$\nabla  \cdot  \vec{B}=0$
电流连续性方程：电荷守恒定律的微分形式：$\nabla\cdot\vec{J}+\frac{\partial\rho}{\partial t}=0$   
高斯定理：$\oint_{S} \vec{E} \cdot \mathrm{d} \vec{S} = \frac{\sum Q_i}{\epsilon_0}$ 微分形式 $\nabla\cdot\vec{E}=\frac{\rho}{\epsilon_0}$  

##### 符号
$\sigma$：电导率
$\epsilon$：电容率
$\chi_e$：介质极化率
$\vec{P}$：总电偶极矩
$w(x,t)$：能量密度：场内单位体积的能量    
$\vec{S}：$能流密度，坡印廷矢量：$\vec{S}=\vec{E} \times \vec{H}$   
$\vec{J}_M$：宏观磁化电流密度
$\vec{J}_D$：位移电流：和电流合起来形成闭合的量，实质上是电场的变化率（电生磁）---为了满足电荷守恒定律的修正
$\vec{M}$：磁化强度
$\rho_m$：假象磁荷密度
$\vec{B},\,\vec{M},\,\vec{H}$方向相同
#### 数学处理
$$
\frac{\vec{r} \, \mathrm{d}S}{r^3}=\mathrm{d }\,\Omega
$$

$\vec{R}/R^3$的无旋性
#### 矢量分析
散度：源  
无源：闭合曲线  （恒定电流只能在闭合曲线中通过）
旋度：环流

散度：面积分到体积分
旋度：线积分到面积分

1. $\oint_{S} \vec{A} \cdot \mathrm{d} \vec{S} = \int_{\Omega}(\nabla \cdot \vec{A}) \mathrm{d} V$
2. $\oint_{l} \vec{A} \cdot \mathrm{d} \vec{l}=\int(\nabla \times \vec{A}) \cdot \mathrm{d} \vec{S}$
3. $\nabla^{2} \vec{A}=\nabla(\nabla \cdot \vec{A})-\nabla \times(\nabla \times \vec{A})$
4. . 任意标量场梯度的旋度为0：$\nabla \times(\nabla f)=0$
5. . 任意矢量场旋度的散度为0：$\nabla \cdot(\nabla \times \vec{f})=0$

感应电场有旋，静电场无旋
##### 确定一个矢量场
1. 旋度
2. 散度
   

亥姆霍兹定理：在有限的区域内，任意矢量场由该矢量场的旋度、散度和边界条件唯一确定
根据亥姆霍兹分解定理，仅当矢量场在无穷远处趋于零时，散度和旋度才能唯一确定这个矢量场
#### 1.普遍规律
积分形式：不连续分布的电荷电流
微分形式：传递关系
##### 电磁场能量的传输
1. 电子运动的动能
2. 导线周围空间中传输的电磁场能量

在电路的载流导线中，电流（电场）方向和其产生的磁场方向相互垂直，其叉积之后得到的能流方向与电流的方向垂直，并且指向导线的截面中心。因此，电子运动的能量并不是供给负载上消耗的能量。在负载上以及在导线上消耗的功率完全是在场中传输的。导线上的电流和周围空间或介质内的电磁场相互制约，使电磁能量在导线附近的电磁场中沿一定方向传输。

#### 2.静电场
$\left\{\begin{array}{l}
\nabla \cdot \vec{D}=\rho \\
\nabla \times \vec{E}=0
\end{array}\right.$

1. 无旋---标势
2. 电势差---电场强度的线积分
$$
\nabla \cdot(-\epsilon\nabla\varphi)=\rho
$$

##### 静电场能量
线性介质：$W=\frac{1}{2} \int_{\infty} \vec{E} \cdot \vec{D} \mathrm{~d} V$
电势表示：$W=\frac{1}{2} \int_{V} \rho \varphi \mathrm{d} V$

为什么电势是一个标量，却能求得电场强度？
因为由于$\nabla \times \vec{E}=0$（静电场的无旋性），他的各个分量不是独立的

$\frac{\partial E_{x}}{\partial y}=\frac{\partial E_{y}}{\partial x}, \frac{\partial E_{z}}{\partial y}=\frac{\partial E_{y}}{\partial z}, \frac{\partial E_{x}}{\partial z}=\frac{\partial E_{z}}{\partial x}$

$\vec{S}=\vec{E} \times \vec{H}$
真空中能量密度：$w=\frac{1}{2}\left(\varepsilon_{0} E^{2}+\frac{1}{\mu_{0}} B^{2}\right)$
线性介质中能量密度：$w=\frac{1}{2}(\vec{E} \cdot \vec{D}+\vec{H} \cdot \vec{B})$
一般介质：$\delta w=\vec{E} \cdot \delta \vec{D}+\vec{H} \cdot \delta \vec{B}$

##### 边界条件
因为在边界处微分不存在（突变） 只能用用积分形式的麦克斯韦方程组
散度做一个上下底面平行于界面的小盒子推出垂直于界面的边界条件
旋度做一个上下边平行于界面的长方形回路推出平行的

##### 电偶极子

$$
\varphi=\frac{\vec{p}\cdot\vec{R}}{4\pi\epsilon_0R^3a                   }
$$
非均匀介质：整个内部
均匀介质的束缚电荷：
1. 自由电荷附近
2. 介质界面处

#### 3.静磁场
静电场：有源无旋----无旋--标势
静磁场：有旋无源----无源--矢势
无源场必可表示为另一矢量的旋度

$\left\{\begin{array}{l}
\nabla \times \vec{H}=\vec J \\
\nabla  \cdot \vec{B}=0
\end{array}\right.$

若$\nabla  \cdot \vec{B}=0$，则$\vec{B}=\nabla \times \vec{A}$，对于这样的定义，由$\vec{A}$不能完全确定$\vec{B}$
$
\begin{aligned}
\vec{B} &=\nabla \times \vec{A}+\nabla \times(\nabla \varphi) \\
&=\nabla \times(\vec{A}+\nabla \varphi) \\
&=\nabla \times \vec{A}^{\prime}
\end{aligned}
$

$\vec{A}$是它沿任一闭合回路的环量代表通过以该回路为边界的任意曲面的磁通量。只有$\vec{A}$的环量才有物理意义，每点上$\vec{A}$的值没有直接的物理意义。
##### 磁矢势
###### 静磁场的库伦规范


$$
\begin{array}{l}
\nabla \cdot \vec{A}=0 \\
\nabla^{2} \vec{A}=-\mu \vec{J}
\end{array}
$$
分量：
$
\left\{\begin{array}{l}
\nabla^{2} A_{x}=-\mu J_{x} \\
\nabla^{2} A_{y}=-\mu J_{y} \\
\nabla^{2} A_{z}=-\mu J_{z}
\end{array}\right.
$

$$
\vec{A}(\vec{x})=\frac{\mu}{4 \pi} \int_{V} \frac{\vec{J}\left(\vec{x}^{\prime}\right) \mathrm{d} V^{\prime}}{r}
$$

$$
\begin{aligned}
\vec{B} &=\nabla \times \vec{A} \\
&=\frac{\mu}{4 \pi} \nabla \times \int_{V} \frac{\vec{J}(\vec{x}) \mathrm{d} V^{\prime}}{r} \\
&=\frac{\mu}{4 \pi} \int_{V}\left(\nabla \frac{1}{r}\right) \times \vec{J}\left(\vec{x}^{\prime}\right) \mathrm{d} V^{\prime} \\
&=\frac{\mu}{4 \pi} \int_{V} \frac{\vec{J} \times \vec{r}}{r^{3}} \mathrm{~d} V^{\prime}
\end{aligned}
$$

把体电流换成线电流，$\vec{J} \mathrm{~d} V^{\prime}=I \mathrm{~d} \vec{l}$
$$
\vec{B}=\frac{\mu}{4 \pi} \oint_{L} \frac{I \mathrm{~d} \vec{l} \times \vec{r}}{r^{3}}
$$

###### 静磁场的能量
$W =\frac{1}{2}\int B\cdot H\,dV$
$W =\frac{1}{2}\int A\cdot J\,dV$

$\frac{1}{2}  A\cdot J$不能看作是能量密度，因为能量分布于磁场内，而不是由电流存在的地方。
$A_e$：外磁场的矢势
$J_e$：产生外磁场的电流分布
$J+J_e$：总电流分布
$A+A_e$：总磁场矢势

磁场总能量
$$
W=\frac{1}{2}\int (J+J_e)\cdot(A+A_e) \, d\,V
$$
电流$J$在外场$A_e$中的相互作用能量为
$$
W_i=\int_V J\cdot A_e\, d\,V
$$

##### 磁标势
1. 电流区域去掉
2. 电流围着的面去掉

分子电流---一对假想磁荷组成的磁偶极子
$\vec{J}=\mu_0\vec{M}$

#### 4.电磁波的传播
##### 波动方程
无源  $\rho=0,\vec{J}=0$
$c=\frac{1}{\sqrt{\mu_0\epsilon_0}}$
$$
\left\{\begin{array}{l}
\nabla^{2} \vec{E}-\frac{1}{c^{2}} \frac{\partial^{2} \vec{E}}{\partial t^{2}}=0 \\
\nabla^{2} \vec{B}-\frac{1}{c^{2}} \frac{\partial^{2} \vec{B}}{\partial t^{2}}=0
\end{array}\right.
$$

束缚电荷以相同频率做正弦振动

介质的色散：
$$
\epsilon=\epsilon(w),\mu=\mu(w)
$$
因此只考虑一定频率的电磁波

##### 时谐电磁波
$$
\left\{\begin{array}{l}
\vec{E}(\vec{x}, t)=\vec{E}(\vec{x}) e^{-i \omega t} \\
\vec{B}(\vec{x}, t)=\vec{B}(\vec{x}) e^{-i \omega t}
\end{array}\right.
$$

$$
\left\{\begin{array}{l}
\nabla \times \vec{E}=i \omega \mu \vec{H} \\
\nabla \times \vec{H}=-i \omega \varepsilon \vec{E}
\end{array}\right.\\ 
\nabla \cdot \vec{E}=0 \\
\nabla \cdot \vec{H}=0 \\
$$

###### 亥姆霍兹方程$k=w\sqrt{\mu\epsilon}$
$$
\nabla^2\vec{E}+k^2\vec{E}=0
$$
隐含条件
$\nabla\cdot\vec{E}=0$
亥姆霍兹方程每一个满足$\nabla\cdot\vec{E}=0$的解都代表一种可能存在的波模



##### 平面电磁波

$\vec{E}=\vec{E}_{0} e^{i(k z-\omega t)}$

相速度：$v_{p}=\frac{\mathrm{d} z}{\mathrm{~d} t}=\frac{\omega}{k}=\frac{1}{\sqrt{\mu\epsilon}}=\frac{1}{\mu\mu_0\epsilon\epsilon_0}=\frac{c}{n}$

$\vec{E}$的取向为电磁波的偏振方向
$$
\vec{k}\cdot\vec{E}=0\\
\vec{B}=\sqrt{\mu\epsilon}\vec{e_k}\times\vec{E}\\
\vec{k}\cdot\vec{B}=0
$$
于是
$$
|\frac{\vec{E}}{\vec{B}}|=\frac{1}{\sqrt{\mu\epsilon}}=v
$$

##### 波导
不同的模式可能具有相同的截止波长（简并）。
只有传输条件得到满足时，模才能传输。
对于给定的波导，如果有 [公式] 个波导满足传输条件，则这 [公式] 个模可以同时在该波导中传输（多模传输）。
#### 5.电磁波的辐射
