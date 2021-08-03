# 线性代数练习题

1. 求各排列(35214, 34251, 25431)的逆序数t

<details>
    <summary>解</summary>

排列(35214)的逆序有：(32, 31, 52, 51, 54, 21)，所以t(35214)=6

排列(34251)的逆序有：(34, 32, 31, 42, 41, 51)，所以t(34251)=6

排列(25431)的逆序有：(21, 54, 53, 51, 43, 41, 31)，所以t(25431)=7

</details>

2. 已知行列式$\left|\begin{array}{}3&-5&2\\1&1&3\\-1&3&-4\end{array}\right|$, 计算余子式$M_{23}$, $M_{32}$, $M_{33}$

<details>
    <summary>解</summary>

$M_{23}=\left|\begin{array}{}3&-5\\-1&3\end{array}\right|=3*3-(-5)*(-1)=4$

$M_{32}=\left|\begin{array}{}3&2\\1&3\end{array}\right|=3*3-2*1=7$

$M_{33}=\left|\begin{array}{}3&-5\\1&1\end{array}\right|=3*1-(-5)*1=8$

</details>

3. 已知行列式$\left|\begin{array}{}3&-5&2\\1&1&3\\-1&3&-4\end{array}\right|$, 计算代数余子式$A_{12}$, $A_{22}$, $A_{13}$

<details>
    <summary>解</summary>

代数余子式定义：$A_{ij}=(-1)^{i+j}M_{ij}$

$A_{12}=(-1)^{1+2}\left|\begin{array}{}1&3\\-1&-4\end{array}\right|=(-1)^{1+2}*(1*(-4)-3*(-1))=1$

$A_{22}=(-1)^{1+2}\left|\begin{array}{}3&2\\-1&-4\end{array}\right|=(-1)^{2+2}*(3*(-4)-2*(-1))=-10$

$A_{13}=(-1)^{1+2}\left|\begin{array}{}1&1\\-1&3\end{array}\right|=(-1)^{1+3}*(1*3-(-1)*1)=4$

</details>

4. 计算三阶行列式：$\left|\begin{array}{}a&0&0\\0&b&0\\0&0&c\end{array}\right|$, $\left|\begin{array}{}0&0&a\\0&b&0\\c&0&0\end{array}\right|$, $\left|\begin{array}{}a&0&0\\d&b&0\\e&f&c\end{array}\right|$

<details>
    <summary>解</summary>

$\left|\begin{array}{}a&0&0\\0&b&0\\0&0&c\end{array}\right|=a*A_{11}+0*A_{12}+0*A_{13}=abc$

$\left|\begin{array}{}0&0&a\\0&b&0\\c&0&0\end{array}\right|=0*A_{11}+0*A_{12}+a*A_{13}=-abc$

$\left|\begin{array}{}a&0&0\\d&b&0\\e&f&c\end{array}\right|=a*A_{11}+0*A_{12}+0*A_{13}=a*(bc-0)=abc$

</details>

5. 已知三阶行列式$\left|\begin{array}{}2&1&k\\0&2&4\\k&1&0\end{array}\right|=-8$, 求k

<details>
    <summary>解</summary>

$\left|\begin{array}{}2&1&k\\0&2&4\\k&1&0\end{array}\right|$

$=2*\left|\begin{array}{}2&4\\1&0\end{array}\right| - 1*\left|\begin{array}{}0&4\\k&0\end{array}\right| + k*\left|\begin{array}{}0&2\\k&1\end{array}\right|$

$= 2*(2-4) - 1*(0-4k) + k*(0-2k)$

$= -2k^2 + 4k - 4 = -4$

$k(k-2)=0$

$k=0, 2$

</details>

6. 已知方程组

$
\begin{cases}
 kx_1 - x_2 = 1\\
 3x_1 + 2x_2 = 5\\
\end{cases}
$

求行列式D；若当方程组有唯一解，求D，k

<details>
    <summary>解</summary>

$D = \left|\begin{array}{}k&-1\\3&2\end{array}\right|= 2k + 3$

若方程组有唯一解

$D = 2k + 3 \neq 0$

$k \neq -3/2$

</details>

7. 已知矩阵

$A = \left[\begin{matrix}x\\y\end{matrix}\right]$

$B = \left[\begin{matrix}a&b\\b&c\end{matrix}\right]$

求$A^T$, $A^TB$, $A^TBA$

<details>
    <summary>解</summary>

$A^T = \left[\begin{matrix}x&y\end{matrix}\right]$

$A^TB = \left[\begin{matrix}x&y\end{matrix}\right]*\left[\begin{matrix}a&b\\b&c\end{matrix}\right] = \left[\begin{matrix}ax+by&bx+cy\end{matrix}\right]$

$A^TBA = \left[\begin{matrix}ax+by&bx+cy\end{matrix}\right]*\left[\begin{matrix}x\\y\end{matrix}\right]=(ax+by)x+(bx+cy)y=ax^2+2bxy+cy^2$

</details>

8. 已知二阶方阵$A=\left[\begin{matrix}a&1\\0&a\end{matrix}\right]$, 求$A^2$, $A^3$, $A^n$

<details>
    <summary>解</summary>

$A^2=\left[\begin{matrix}a&1\\0&a\end{matrix}\right]*\left[\begin{matrix}a&1\\0&a\end{matrix}\right]=\left[\begin{matrix}a*a+1*0&a*1+1*a\\0*a+a*0&0*1+a*a\end{matrix}\right]=\left[\begin{matrix}a^2&2a\\0&a^2\end{matrix}\right]$

$A^3=\left[\begin{matrix}a^2&2a\\0&a^2\end{matrix}\right]*\left[\begin{matrix}a&1\\0&a\end{matrix}\right]=\left[\begin{matrix}a^3&3a^2\\0&a^3\end{matrix}\right]$

$A^n=\left[\begin{matrix}a^n&na^{n-1}\\0&a^n\end{matrix}\right]$

</details>

9. 已知三阶方阵A, B, |A|=-3, |B|=2, 求|2A|, |3B|, |2AB|

<details>
    <summary>解</summary>

$|2A|=\left|2*\left[\begin{matrix}a&b&c\\d&e&f\\h&i&j\end{matrix}\right]\right|=\left|\left[\begin{matrix}2a&2b&2c\\2d&2e&2f\\2h&2i&2j\end{matrix}\right]\right|=2*\left|\left[\begin{matrix}a&b&c\\2d&2e&2f\\2h&2i&2j\end{matrix}\right]\right|=2*2*\left|\left[\begin{matrix}a&b&c\\d&e&f\\2h&2i&2j\end{matrix}\right]\right|=2*2*2*\left|\left[\begin{matrix}a&b&c\\d&e&f\\h&i&j\end{matrix}\right]\right|=2*2*2*(-3)=-24$

$|3B|=3*3*3*2=54$

设$A=\left[\begin{matrix}a&0&0\\0&b&0\\0&0&c\end{matrix}\right]$, $B=\left[\begin{matrix}d&0&0\\0&e&0\\0&0&f\end{matrix}\right]$, 则$AB=\left[\begin{matrix}ad&0&0\\0&be&0\\0&0&cf\end{matrix}\right]$

$|A|=abc$, $|B|=def$, 

$|AB|=ad*be*cf=abc*def=|A|*|B|$

$|2AB|=2*2*2*|AB|=2*2*2*(-3)*2=-48$

</details>

10. $A=\left[\begin{matrix}1&-1&-1\\2&-1&-3\\3&2&-5\end{matrix}\right]$, $B=\left[\begin{matrix}2\\1\\0\end{matrix}\right]$

求二项式|A|, 伴随矩阵$A^*$, 逆矩阵$A^{-1}$

求解矩阵方程AX=B

<details>
    <summary>解</summary>

用$a_{ij}$表示A矩阵的i行j列

用$A_{ij}$表示A矩阵的i行j列的代数余子式

用$M_{ij}$表示A矩阵的i行j列的余子式，是A矩阵消去i行j列后余下的部分

$A_{ij}=(-1)^{i+j}M_{ij}$

$|A|=\sum_{1}^na_{1j}A_{1j}$

$A^*=\left[A_{ij}\right]^T=\left[\begin{matrix}{A_{11}}&{a_{21}}&{\cdots}&{a_{n1}}\\{a_{12}}&{a_{22}}&{\cdots}&{a_{n2}}\\{\vdots}&{\vdots}&{\ddots}&{\vdots}\\{a_{1m}}&{a_{2m}}&{\cdots}&{a_{nm}}\end{matrix}\right]$

$A^{-1}=\frac{1}{|A|}A^*$

$AX=B$

$A^{-1}AX=A^{-1}B$

$X=A^{-1}B$

</details>

11. $A=\left[\begin{matrix}3&2&-1\\2&-1&3\\7&0&5\end{matrix}\right]$

求|A|, R(A), 一个最高阶非零子式

<details>
    <summary>解</summary>

矩阵的初等变换可以用矩阵乘法来表示

$\left[\begin{matrix}1&0&0\\1&2&0\\1&2&-1\end{matrix}\right]*\left[\begin{matrix}3&2&-1\\2&-1&3\\7&0&5\end{matrix}\right]=\left[\begin{matrix}3&2&-1\\7&0&5\\0&0&0\end{matrix}\right]$

$\left[\begin{matrix}3&2&-1\\7&0&5\\0&0&0\end{matrix}\right]*\left[\begin{matrix}0&1&0\\1&0&0\\0&0&1\end{matrix}\right]=\left[\begin{matrix}2&3&-1\\0&7&5\\0&0&0\end{matrix}\right]$

矩阵A通过初等变换化为$\left[\begin{matrix}2&3&-1\\0&7&5\\0&0&0\end{matrix}\right]$

非零子式的最高阶为2，所以R(A)=2

</details>

12. 已知A为n阶方阵，$|A|=n^n$，求$R(A)$, $|A^{-1}|$, $|nA^{-1}|$

<details>
    <summary>解</summary>

$|A|=n^n\neq0$, $R(A)=n$

$|A^{-1}|*|A|=1$, $|A|=n^n$, $|A^{-1}|=\frac{1}{n^n}$

A是n阶方阵，$|nA^{-1}|=n^n|A^{-1}|=n^n * \frac{1}{n^n}=1$

</details>

13. 已知A为3阶矩阵，$|A|=\frac{1}{2}$, 求$R(A)$, $|A^{-1}|$, $|A^*|$

<details>
    <summary>解</summary>

$|A|=\frac{1}{2}\neq0$, $R(A)=n$

$|A^{-1}|*|A|=1$, $|A|=\frac{1}{2}$, $|A^{-1}|=2$

A是n阶方阵，$A^{-1}=\frac{1}{|A|}A^*$

$|A^{-1}|=|\frac{1}{|A|}A^*|$

$|A^{-1}|=\frac{1}{|A|}=\frac{1}{|A|^n}|A^*|$

$|A^*|=|A|^{n-1}$

</details>

14. n元线性方程组$Ax=b$的解判定

<details>
    <summary>解</summary>

无解的充要条件：$R(A)<R(A,b)$

唯一解充要条件：$R(A)=R(A,b)=n$

无限解充要条件：$R(A)=R(A,b)<n$

n元齐次线性方程组$Ax=0$有非零解充要条件：$R(A)<n$

线性方程组$Ax=b$有解充要条件：$R(A)=R(A,b)$

矩阵方程$AX=B$有解充要条件：$R(A)=R(A,B)$

</details>

15. 

$
\begin{cases}
 3x_1 + kx_2 + x_3 = 0\\
 4x_2 + x_3 = 0\\
 kx_1 + 4x_2 = 0
\end{cases}
$

求系数行列式D，若方程组有非零解，求k

<details>
    <summary>解</summary>

当系数行列式D=0，方程组有非零解

</details>

16. 

$
\begin{cases}
 (1-a)x_1 + x_2 = 1\\
 x_1 + (1-a)x_2 + x_3 = 2\\
 3x_2 + (1-a)x_3= 3
\end{cases}
$

若方程组有唯一解，求a

<details>
    <summary>解</summary>

系数行列式$D\neq0$

$D=(1-a)(3-a)(1+a)\neq0$

</details>

17. 

$
\begin{cases}
 ax_1 + x_2 + x_3 = 1\\
 x_1 + ax_2 + x_3 = a\\
 x_1 + x_2 + ax_3= a^2
\end{cases}
$

求增广矩阵

增广矩阵的阶梯型

方程组无解，求a

方程组有无限解，求a和通解

<details>
    <summary>解</summary>

增广矩阵

$\left[\begin{matrix}a&1&1&1\\1&a&1&a\\1&1&a&a^2\end{matrix}\right]$

增广矩阵的阶梯型

$\left[\begin{matrix}
1&0&1+a&a(1+a)\\
0&1&-1&-a\\
0&0&(1+a)(2+a)&(1-a)(1+a)^2
\end{matrix}\right]$

无解

$
\begin{cases}
 (1+a)(2+a) = 0\\
 (1-a)(1+a)^2 \neq 0
\end{cases}
$

唯一解

$(1+a)(2+a) \neq 0$

无限解

$
\begin{cases}
 (1+a)(2+a) = 0\\
 (1-a)(1+a)^2 = 0
\end{cases}
$

通解$x = \left[\begin{matrix}x1\\x2\\x3\end{matrix}\right] = x_p + x_n$

当$a = -1$

增广矩阵为

$\left[\begin{matrix}
1&0&0&0\\
0&1&-1&1\\
0&0&0&0
\end{matrix}\right]$

增广矩阵每行第一个系数不为0的变量，叫做独立变量，$x_1$, $x_2$

其余的变量为自由变量：$x_3$

$x_p$是$Ax=b$在自由变量$x_3=0$的特解，

$x_p=\left[\begin{matrix}0\\1\\0\end{matrix}\right]$

$x_n$是$Ax=0$的基础解，设自由变量$x_3=1$求基础基

$x_n=c\left[\begin{matrix}0\\1\\1\end{matrix}\right]$

通解$x = x_p + x_n = \left[\begin{matrix}0\\1\\0\end{matrix}\right] + c\left[\begin{matrix}0\\1\\1\end{matrix}\right]$, $c\in{R}$

</details>

18. 

$
\begin{cases}
 x_1 + 2x_2 - x_3 + 3x_4 = 2\\
 2x_1 + 4x_2 - 2x_3 + 5x_4 = 1\\
 -x_1 - 2x_2 + x_3 - x_4 = 4
\end{cases}
$

求增广矩阵的秩

齐次线性方程组的特解

非齐次线性方程组的通解

<details>
    <summary>解</summary>

增广矩阵

$\left[\begin{matrix}
1&2&-1&3&2\\
2&4&-2&5&1\\
-1&-2&1&-1&4
\end{matrix}\right]$

经过初等变换为阶梯矩阵

$\left[\begin{matrix}
1&2&-1&3&2\\
0&0&0&1&3\\
0&0&0&0&0
\end{matrix}\right]$

非零子阵的最高阶为2，增广矩阵的秩为2

阶梯矩阵的每行第一个系数不为0的变量为独立变量$x_1$, $x_4$

其余的变量为自由变量$x_2$, $x_3$

设自由变量$x_2$, $x_3$为0，求出$Ax=b$的特解

$x_p=\left[\begin{matrix}-7\\0\\0\\3\end{matrix}\right]$

自由变量$x_2$, $x_3$分别设为1，代入齐次线性方程组$Ax=0$

$
\begin{cases}
 \left[\begin{matrix}1&2&-1&3\\0&0&0&1\\0&0&0&0\end{matrix}\right] * \left[\begin{matrix}x_1\\1\\0\\x_4\end{matrix}\right]= \left[\begin{matrix}0\\0\\0\\0\end{matrix}\right]\\
 \\
 \left[\begin{matrix}1&2&-1&3\\0&0&0&1\\0&0&0&0\end{matrix}\right] * \left[\begin{matrix}x_1\\0\\1\\x_4\end{matrix}\right]= \left[\begin{matrix}0\\0\\0\\0\end{matrix}\right]
\end{cases}
$

解出两个基础解

$\left[\begin{matrix}-2\\1\\0\\0\end{matrix}\right]$, $\left[\begin{matrix}1\\0\\1\\0\end{matrix}\right]$

基础解为

$a_1\left[\begin{matrix}-2\\1\\0\\0\end{matrix}\right] + a_2\left[\begin{matrix}1\\0\\1\\0\end{matrix}\right]$

$a_1, a_2 \in R$

</details>

19. 已知向量组A：$a_1=\left[\begin{matrix}1\\-3\end{matrix}\right]$, $a_2=\left[\begin{matrix}2\\\alpha\end{matrix}\right]$; 向量$b=\left[\begin{matrix}\beta\\3\end{matrix}\right]$

当b不能由A线性表示，求$\alpha$, $\beta$

当b可由A唯一线性表示，求$\alpha$

<details>
    <summary>解</summary>

b由A线性表示：

$b=x_1\left[\begin{matrix}1\\-3\end{matrix}\right] + x_2\left[\begin{matrix}2\\\alpha\end{matrix}\right]=\left[\begin{matrix}\beta\\3\end{matrix}\right]$

可以写成线性方程组：

$\left[\begin{matrix}1&2\\-3&\alpha\end{matrix}\right]\left[\begin{matrix}x_1\\x_2\end{matrix}\right]=\left[\begin{matrix}\beta\\3\end{matrix}\right]$

此方程组无解，则b不能由A线性表示

写成增广矩阵

$\left[\begin{matrix}1&2&\beta\\-3&\alpha&3\end{matrix}\right]$

通过初等变换，化为阶梯型

$\left[\begin{matrix}1&2&\beta\\0&6+\alpha&3\beta+3\end{matrix}\right]$

无解的条件为：

$
\begin{cases}
 6 + \alpha = 0\\
 3\beta+3 \neq 0
\end{cases}
$

有唯一解的条件为：

$
\begin{cases}
 6 + \alpha \neq 0\\
 3\beta+3 \neq 0
\end{cases}
$

</details>

20. 已知向量组

$A=(a_1,a_2,a_3)=\left[\begin{matrix}k&-1&1\\1&k&-1\\1&-1&k\end{matrix}\right]$

线性无关，求k

<details>
    <summary>解</summary>



</details>