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

<details open>
    <summary>解</summary>

$\left[\begin{matrix}1&0&0\\1&2&0\\1&2&-1\end{matrix}\right]*\left[\begin{matrix}3&2&-1\\2&-1&3\\7&0&5\end{matrix}\right]=\left[\begin{matrix}3&2&-1\\7&0&5\\0&0&0\end{matrix}\right]$

$\left[\begin{matrix}3&2&-1\\7&0&5\\0&0&0\end{matrix}\right]*\left[\begin{matrix}0&1&0\\1&0&0\\0&0&1\end{matrix}\right]=\left[\begin{matrix}2&3&-1\\0&7&5\\0&0&0\end{matrix}\right]$

</details>
