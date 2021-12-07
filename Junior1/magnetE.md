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

#### 矢量分析
散度：源  
无源：闭合曲线  （恒定电流只能在闭合曲线中通过）
旋度：环流
1. $\oint_{S} \vec{A} \cdot \mathrm{d} \vec{S} = \int_{\Omega}(\nabla \cdot \vec{A}) \mathrm{d} V$
2. $\oint_{l} \vec{A} \cdot \mathrm{d} \vec{l}=\int(\nabla \times \vec{A}) \cdot \mathrm{d} \vec{S}$
3. $\nabla^{2} \vec{A}=\nabla(\nabla \cdot \vec{A})-\nabla \times(\nabla \times \vec{A})$
4. . 任意标量场梯度的旋度为0：$\nabla \times(\nabla f)=0$
5. . 任意矢量场旋度的散度为0：$\nabla \cdot(\nabla \times \vec{f})=0$

感应电场有旋，静电场无旋
##### 确定一个矢量场
1. 旋度
2. 散度

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

#### 3.静磁场
静电场：有源无旋----无旋--标势
静磁场：有旋无源----无源--矢势
$\left\{\begin{array}{l}
\nabla \times \vec{H}=\vec J \\
\nabla  \cdot \vec{B}=0
\end{array}\right.$

若$\nabla  \cdot \vec{B}=0$，则$\vec{B}=\nabla \times \vec{A}$
对于这样的定义，由$\vec{A}$不能完全确定$\vec{B}$