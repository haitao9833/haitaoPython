# Jupyter Notebook & 深度学习 & 快速上手使用教程

<img src="https://img.shields.io/badge/Jupyter Notebook-基础语法-ff5722.svg?colorA=FFFAF0&colorB=ff69b4&logo=jupyter" />
<img src="https://img.shields.io/badge/Jupyter Notebook-数据处理 | Txt | Excel | Json -ff5722.svg?colorA=FFFAF0&colorB=ff69b4&logo=databricks" />
<img src="https://img.shields.io/badge/Jupyter Notebook-数据可视化-ff5722.svg?colorA=FFFAF0&colorB=ff69b4&logo=simpleanalytics" />
<img src="https://img.shields.io/badge/Jupyter Notebook-预训练语言模型-ff5722.svg?colorA=FFFAF0&colorB=ff69b4&logo=pytorch" />

# 环境

```
pip install numpy                 -i https://pypi.tuna.tsinghua.edu.cn/simple 
pip install pandas                -i https://pypi.tuna.tsinghua.edu.cn/simple 
pip install sentence-transformers -i https://pypi.tuna.tsinghua.edu.cn/simple/
pip install sklearn               -i https://pypi.tuna.tsinghua.edu.cn/simple/
pip install scikit-learn          -i https://pypi.tuna.tsinghua.edu.cn/simple/
pip install matplotlib            -i https://pypi.tuna.tsinghua.edu.cn/simple/
pip install openpyxl              -i https://pypi.tuna.tsinghua.edu.cn/simple/
pip install jieba                 -i https://pypi.tuna.tsinghua.edu.cn/simple/
pip install plotly                -i https://pypi.tuna.tsinghua.edu.cn/simple/
pip install pythonds              -i https://pypi.tuna.tsinghua.edu.cn/simple/
pip install stanfordcorenlp       -i https://pypi.tuna.tsinghua.edu.cn/simple/
pip install sklearn.mainfold      -i https://pypi.tuna.tsinghua.edu.cn/simple/
pip install pyecharts -U          -i https://pypi.tuna.tsinghua.edu.cn/simple/

conda install pytorch torchvision torchaudio cudatoolkit=11.6 -c pytorch -c conda-forge
conda install transformers
```
# 数据可视化

<div align="center" style="display:flex">
	<img hspace="0px" width="1200px" height="401px" src="/echarts1.png" title="鼠标停留" alt="加载失败" />
</div>

<div align="center" style="display:flex">
	<img hspace="0px" width="1200px" height="401px" src="/echarts2.png" title="鼠标停留" alt="加载失败" />
</div>

<div align="center" style="display:flex">
	<img hspace="0px" width="1200px" height="401px" src="/echarts3.png" title="鼠标停留" alt="加载失败" />
</div>

<div align="center" style="display:flex">
	<img hspace="0px" width="1200px" height="401px" src="/echarts4.png" title="鼠标停留" alt="加载失败" />
</div>

<div align="center" style="display:flex">
	<img hspace="0px" width="1200px" height="401px" src="/echarts5.png" title="鼠标停留" alt="加载失败" />
</div>

<div align="center" style="display:flex">
	<img hspace="0px" width="1200px" height="401px" src="/echarts6.png" title="鼠标停留" alt="加载失败" />
</div>

<div align="center" style="display:flex">
	<img hspace="0px" width="1200px" height="401px" src="/echarts7.png" title="鼠标停留" alt="加载失败" />
</div>

<div align="center" style="display:flex">
	<img hspace="0px" width="1200px" height="401px" src="/echarts8.png" title="鼠标停留" alt="加载失败" />
</div>

<div align="center" style="display:flex">
	<img hspace="0px" width="1200px" height="401px" src="/echarts9.png" title="鼠标停留" alt="加载失败" />
</div>
# 概率论基础

# 科学计数法

> - `E` 代表的是 `exponent` 指数
> - `E` 表示的是乘以 $10^n$ 次方

# 统计概率

> - 概率 `==` 面积

## 事件

> - 并事件 `==` 和事件：$A\cup B\ =\ A+B$（至少有一个发生）
> - 交事件 `==` 积事件：$A\cap B\ =\ A\ \cdot\ B$（同时发生） 
> - 互斥事件：$P(A_1\ \cup\ A_2\ \cup\ \ldots\ \cup\ A_n)=P(A_1)\ +\ P(A_2)\ +\ \ldots\ +\ P(A_n)$ （不能同时发生）
> - 非互斥情况：$P(A\ \cup\ B)\ =\ P(A)\ +\ P(B)\ -\ P(A\ \cap\ B)$  （即减去重复的面积）

## 三概率

> - 联合概率：$P(A\cap B)=\frac{A\cap B\ 交集面积}{\Omega\ 全面积}$   
> - 边缘概率：$P(A)=\frac{A\ 面积}{\Omega\ 全面积}$   
> - 条件概率：$P(B| A)=\frac{A\cap B\ 交集面积}{A\ 面积}$   
>
> $$
> P(B|A)\ =\ \frac{P(A\ \cap\ B)}{P(A)}\ =\ \frac{P(B|A)\cdot P(A)}{P(A)}\ =\ \frac{P(A|B)\cdot P(B)}{P(A)}
> $$

## 乘法法则

> - 分解联合概率，用面积理解，即所有事件的**<u>交集面积</u>**   
>
> $$
> P(A\ \cap\ B\ \cap\ C\ \cap\ \ldots\ \cap\ N)\ =\ P(A)\ \cdot\ P(B|A)\ \cdot\ P(C|A\cap B)\ \ldots
> $$

## 两公式

> - 设：$B$ 为结果
> - 设：$\{A_1\ ,\ A_2\ ,\ \ldots\ ,\ A_n\}$ 两两互斥且 $A_1\ \cup\ A_2\ \cup\ \ldots\ \cup\ A_n\ =\ \Omega$ 为所有原因
> - 全概率公式：$P(B)\ =\ \sum联合概率\ =\ 即\ B\ 与所有原因\ \{A_1\ ,\ A_2\ ,\ \ldots\ ,\ A_n\}\ 的交集面积总和=\frac{B\ 面积}{\Omega\ 全面积}$   
> - 贝叶斯公式：$\frac{P(B\ \cap\ A_i)}{P(B)}=\frac{B\ 与某个原因\ A_i\ 的交集面积}{B\ 与所有原因\ \{A_1\ ,\ A_2\ ,\ \ldots\ ,\ A_n\}\ 的交集面积总和}$   

## 排列组合

> $$
> C_n^m\ =\ \frac{A_n^m}{A_m^m}\ =\ \frac{\frac{n!}{(n-m)!}}{m!}
> $$
>
> - 5 名游客，到 3 个景点游览，每个景点至少 1 人，至多 2 人 $\Rightarrow\ C_5^1\cdot C_4^2\cdot C_2^2\cdot \frac{A_3^3}{A_2^2}$（因为有两组 `2` 人组无差别游览）
> - 5 名游客，到 4 个景点游览，每个景点至少 1 人，至多 2 人 $\Rightarrow\ C_5^1\cdot C_4^1\cdot C_3^1\cdot C_2^2\cdot \frac{A_4^4}{A_3^3}$（因为有三组 `1` 人组无差别游览）
> - 12 个球放入 3 个盒子，允许有空盒 $\Rightarrow$ 15 个球放入 3 个盒子，不允许有空盒 $\Rightarrow \ C_{14}^2$ （`x + y + z = 12` 的非负整数解）

## 贝叶斯

> - [贝叶斯更新：前一次贝叶斯更新中计算出的后验概率，会在下一次贝叶斯更新中作为先验概率](https://blog.csdn.net/weixin_48978134/article/details/126750571)   
> - 检验信念的标准是它们解释世界的能力
> - 数据影响信念，关注那些改变信念的数据
> - 条件独立性假设
>
> $$
> P(X_1\ ,\ X_2\ ,\ \ldots\ ,\ X_n\ |\ Y)\ =\ P(X_1\ |\ Y)\ \cdot\ P(X_2\ |\ Y)\ \cdot\ \ldots\ \cdot\ P(X_n\ |\ Y)
> $$
>
> - 即给定事件 $Y$ 发生的情况下，事件 $X_1\ ,\ X_2\ ,\ \ldots\ ,\ X_n$ 之间相互独立
> - [概率图模型之贝叶斯网络----------](https://zhuanlan.zhihu.com/p/30139208)   

## 独立性

> - **<u>概率与条件无关，添加或删除条件不影响概率</u>** 
> - $三个（或以上）个事件之间相互独立\Leftrightarrow\left\{\begin{aligned}&两两独立\Leftrightarrow\left\{\begin{aligned}&A\ 与\ B\ 独立\Leftrightarrow P(AB)=P(A)\cdot P(B)\\&A\ 与\ C\ 独立\Leftrightarrow P(AC)=P(A)\cdot P(C)\\&B\ 与\ C\ 独立\Leftrightarrow P(BC)=P(B)\cdot P(C)\end{aligned}\right.\\&组合独立\Leftrightarrow\left\{\begin{aligned}&A\ 与\ BC\ 独立\\&B\ 与\ AC\ 独立\\&C\ 与\ AB\ 独立\end{aligned}\right.\left\}\begin{aligned}&\\&\\&\end{aligned}\right.\leftrightharpoons P(ABC)=P(A)\cdot P(B)\cdot P(C)\end{aligned}\right.$   
> - $\leftrightharpoons$ 表示左右两边需要搭配两两独立条件才能相互推出
>
> $$
> \begin{aligned}
> P(ABC)&=P(A)\cdot P(B)\cdot P(C)\\
> &=P(A)\cdot P(B|A)\cdot P(C|AB)\\
> &=P(B)\cdot P(C|B)\cdot P(A|BC)\\
> &=P(C)\cdot P(A|C)\cdot P(B|AC)
> \end{aligned}
> $$

## 最大似然估计

# 基础语法

## `base_`

- List
- Tuple
- String
- Dictionary
- for 循环

## `base_Numpy`

- 创建
- 属性
- 变维
- 运算
- 比较
- 切片 & 访问
- 副本 & 视图
- 缺省值 `np.nan`
- 一维 `ndarray` 的拼接
- 二维 `ndarray` 的拼接
- 扁平化
- 降维

## `base_Pandas`

- Index
- Series
- DataFrame（内容较多）

# 数据处理
> `data_`

## `data_Use`

- 路径
- 通用函数
- 正则表达式

## `data_Test`

- 使用 `data_Tool.ipynb` 进行数据处理的案例

# 预训练语言模型
> `pre_`
