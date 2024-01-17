> 基于[katex](https://katex.org/docs/support_table)
> 使用 `Markdown` 编写数学公式比较麻烦 可选择在线数学公式编辑 [Equation Editor](https://editor.codecogs.com/?lang=zh-cn)
> 在线编辑完成后可复制到本文件中展示

### 行内与独行

#### 行内公式

> 将公式插入到本行内，符号：`$公式内容$`

```
$f(x)=2x^2+3x+5$
```

_效果：_
$f(x)=2x^2+3x+5$

#### 独行公式

> 将公式插入到新的一行内，并且居中，符号：`$$公式内容$$`

```
$$x_{1,2} = {-b\pm\sqrt{b^2 - 4ac} \over 2a}.$$
```

_效果：_
$$x_{1,2} = {-b\pm\sqrt{b^2 - 4ac} \over 2a}.$$

### 上标、下标与组合

| 描述     | 符合 | 示例                  |        效果         |
| :------- | :--: | :-------------------- | :-----------------: |
| 上标符号 | `^`  | `$x^4$`               |        $x^4$        |
| 下标符号 | `_`  | `$x_1$`               |        $x_1$        |
| 组合符号 | `{}` | `${16}_{8}O{2+}_{2}$` | ${16}_{8}O{2+}_{2}$ |

### 汉字、字体与格式

| 描述       |              符合              | 示例                                                 |                        效果                        |
| :--------- | :----------------------------: | :--------------------------------------------------- | :------------------------------------------------: |
| 汉字形式   |           `\mbox{}`            | `$V_{\mbox{初始}}$`                                  |                 $V_{\mbox{初始}}$                  |
| 字体控制   |        `\displaystyle`         | `$\displaystyle \frac{x+y}{y+z}$`                    |          $\displaystyle \frac{x+y}{y+z}$           |
| 下划线符号 |          `\underline`          | `$\underline{x+y}$`                                  |                 $\underline{x+y}$                  |
| 标签       |          `\tag{数字}`          | `$\tag{11}$`                                         |                     $\tag{11}$                     |
| 上大括号   |       `\overbrace{算式}`       | `$\overbrace{a+b+c+d}^{2.0}$`                        |            $\overbrace{a+b+c+d}^{2.0}$             |
| 下大括号   |      `\underbrace{算式}`       | `$a+\underbrace{b+c}_{1.0}+d$`                       |            $a+\underbrace{b+c}_{1.0}+d$            |
| 上位符号   | `\stacrel{上位符号}{基位符号}` | `$\vec{x}\stackrel{\mathrm{def}}{=}{x_1,\dots,x_n}$` | $\vec{x}\stackrel{\mathrm{def}}{=}{x_1,\dots,x_n}$ |

### 占位符

| 描述           |   符合   | 示例           |     效果     |
| :------------- | :------: | :------------- | :----------: |
| 两个 quad 空格 | `\qquad` | `$x \qquad y$` | $x \qquad y$ |
| quad 空格      | `\quad`  | `$x \quad y$`  | $x \quad y$  |
| 大空格         |   `\`    | `$x \ y$`      |   $x \ y$    |
| 中空格         |   `\:`   | `$x \: y$`     |   $x \: y$   |
| 小空格         |   `\,`   | `$x \, y$`     |   $x \, y$   |
| 紧贴           |   `\!`   | `$x \! y$`     |   $x \! y$   |

### 定界符与组合

| 描述       |                         符合                          | 示例                                                                   |                                 效果                                 |
| :--------- | :---------------------------------------------------: | :--------------------------------------------------------------------- | :------------------------------------------------------------------: |
| 括号       | `（）\big(\big) \Big(\Big) \bigg(\bigg) \Bigg(\Bigg)` | `$（）\big(\big) \Big(\Big) \bigg(\bigg) \Bigg(\Bigg)$`                |        $（）\big(\big) \Big(\Big) \bigg(\bigg) \Bigg(\Bigg)$         |
| 中括号     |                         `[]`                          | `$[x+y]$`                                                              |                               $[x+y]$                                |
| 大括号     |                        `\{ \}`                        | `${x+y}$`                                                              |                               ${x+y}$                                |
| 自适应括号 |                    `\left \right`                     | `$\left(x\right)$，$\left(x{yz}\right)$`                               |                $\left(x\right)$，$\left(x{yz}\right)$                |
| 组合公式   |             `{上位公式 \choose 下位公式}`             | `${n+1 \choose k}={n \choose k}+{n \choose k-1}$`                      |           ${n+1 \choose k}={n \choose k}+{n \choose k-1}$            |
| 组合公式   |              `{上位公式 \atop 下位公式}`              | `$\sum_{k_0,k_1,\ldots>0 \atop k_0+k_1+\cdots=n}A_{k_0}A_{k_1}\cdots$` | $\sum_{k_0,k_1,\ldots>0 \atop k_0+k_1+\cdots=n}A_{k_0}A_{k_1}\cdots$ |

### 四则运算

| 描述       |         符合          | 示例                  |        效果         |
| :--------- | :-------------------: | :-------------------- | :-----------------: |
| 加法运算   |          `+`          | `$x+y=z$`             |       $x+y=z$       |
| 减法运算   |          `-`          | `$x-y=z$`             |       $x-y=z$       |
| 加减运算   |         `\pm`         | `$x \pm y=z$`         |     $x \pm y=z$     |
| 减加运算   |         `\mp`         | `$x \mp y=z$`         |     $x \mp y=z$     |
| 乘法运算   |       `\times`        | `$x \times y=z$`      |   $x \times y=z$    |
| 点乘运算   |        `\cdot`        | `$x \cdot y=z$`       |    $x \cdot y=z$    |
| 星乘运算   |        `\ast`         | `$x \ast y=z$`        |    $x \ast y=z$     |
| 除法运算   |        `\div`         | `$x \div y=z$`        |    $x \div y=z$     |
| 斜法运算   |          `/`          | `$x/y=z$`             |       $x/y=z$       |
| 分式表示   |  `\frac{分子}{分母}`  | `$\frac{x+y}{y+z}$`   |  $\frac{x+y}{y+z}$  |
| 分式表示   | `{分子} \voer {分母}` | `${x+y} \over {y+z}$` | ${x+y} \over {y+z}$ |
| 绝对值表示 |        `\|\|`         | `$\|x+y\|$`           |      $\|x+y\|$      |

> 注:绝对值 `｜｜` 进行了转义`\|`否则无法展示

### 高级运算

| 描述         |             符合              | 示例                                                                                                                            |                                                             效果                                                              |
| :----------- | :---------------------------: | :------------------------------------------------------------------------------------------------------------------------------ | :---------------------------------------------------------------------------------------------------------------------------: |
| 平均数运算   |       `\overline{算式}`       | `$\overline{xyz}$`                                                                                                              |                                                       $\overline{xyz}$                                                        |
| 开二次方运算 |            `\sqrt`            | `$\sqrt x$`                                                                                                                     |                                                           $\sqrt x$                                                           |
| 开方运算     |   `\sqrt[开方数]{被开方数}`   | `$\sqrt[3]{x+y}$`                                                                                                               |                                                        $\sqrt[3]{x+y}$                                                        |
| 对数运算     |            `\log`             | `$\log(x)$`                                                                                                                     |                                                           $\log(x)$                                                           |
| 极限运算     |            `\lim`             | `$\lim^{x \to \infty}_{y \to 0}{\frac{x}{y}}$`                                                                                  |                                         $\lim^{x \to \infty}_{y \to 0}{\frac{x}{y}}$                                          |
| 极限运算     |     `\displaystyle \lim`      | `$\displaystyle \lim^{x \to \infty}_{y \to 0}{\frac{x}{y}}$`                                                                    |                                  $\displaystyle \lim^{x \to \infty}_{y \to 0}{\frac{x}{y}}$                                   |
| 求和运算     |            `\sum`             | `$\sum^{x \to \infty}_{y \to 0}{\frac{x}{y}}$`                                                                                  |                                         $\sum^{x \to \infty}_{y \to 0}{\frac{x}{y}}$                                          |
| 求和运算     |     `\displaystyle \sum`      | `$\displaystyle \sum^{x \to \infty}_{y \to 0}{\frac{x}{y}}$`                                                                    |                                  $\displaystyle \sum^{x \to \infty}_{y \to 0}{\frac{x}{y}}$                                   |
| 积分运算     |            `\int`             | `$\int^{\infty}_{0}{xdx}$`                                                                                                      |                                                   $\int^{\infty}_{0}{xdx}$                                                    |
| 积分运算     |     `\displaystyle \int`      | `$\displaystyle \int^{\infty}_{0}{xdx}$`                                                                                        |                                            $\displaystyle \int^{\infty}_{0}{xdx}$                                             |
| 微分运算     |          `\partial`           | `$\frac{\partial x}{\partial y}$`                                                                                               |                                                $\frac{\partial x}{\partial y}$                                                |
| 矩阵表示     | `\begin{matrix} \end{matrix}` | `$\left[ \begin{matrix} 1 &2 &\cdots &4\5 &6 &\cdots &8\\vdots &\vdots &\ddots &\vdots\13 &14 &\cdots &16\end{matrix} \right]$` | $\left[ \begin{matrix} 1 &2 &\cdots &4\5 &6 &\cdots &8\\vdots &\vdots &\ddots &\vdots\13 &14 &\cdots &16\end{matrix} \right]$ |

### 逻辑运算

| 描述           |    符合    | 示例               |       效果       |
| :------------- | :--------: | :----------------- | :--------------: |
| 等于运算       |    `=`     | `$x+y=z$`          |     $x+y=z$      |
| 大于运算       |    `>`     | `$x+y>z$`          |     $x+y>z$      |
| 小于运算       |    `<`     | `$x+y<z$`          |     $x+y<z$      |
| 大于等于运算   |   `\geq`   | `$x+y \geq z$`     |   $x+y \geq z$   |
| 小于等于运算   |   `\leq`   | `$x+y \leq z$`     |   $x+y \leq z$   |
| 不等于运算     |   `\neq`   | `$x+y \neq z$`     |   $x+y \neq z$   |
| 不大于等于运算 |  `\ngeq`   | `$x+y \ngeq z$`    |  $x+y \ngeq z$   |
| 不大于等于运算 | `\not\geq` | `$x+y \not\geq z$` | $x+y \not\geq z$ |
| 不小于等于运算 |  `\nleq`   | `$x+y \nleq z$`    |  $x+y \nleq z$   |
| 不小于等于运算 | `\not\leq` | `$x+y \not\leq z$` | $x+y \not\leq z$ |
| 约等于运算     | `\approx`  | `$x+y \approx z$`  | $x+y \approx z$  |
| 恒定等于运算   |  `\equiv`  | `$x+y \equiv z$`   |  $x+y \equiv z$  |

### 集合运算

| 描述         |     符合      | 示例                |       效果        |
| :----------- | :-----------: | :------------------ | :---------------: |
| 属于运算     |     `\in`     | `$x \in y$`         |     $x \in y$     |
| 不属于运算   |   `\notin`    | `$x \notin y$`      |   $x \notin y$    |
| 不属于运算   |   `\not\in`   | `$x \not\in y$`     |   $x \not\in y$   |
| 子集运算     |   `\subset`   | `$x \subset y$`     |   $x \subset y$   |
| 真子集运算   |  `\subseteq`  | `$x \subseteq y$`   |  $x \subseteq y$  |
| 非真子集运算 | `\subsetneq`  | `$x \subsetneq y$`  | $x \subsetneq y$  |
| 非子集运算   | `\not\supset` | `$x \not\supset y$` | $x \not\supset y$ |
| 并集运算     |    `\cup`     | `$x \cup y$`        |    $x \cup y$     |
| 交集运算     |    `\cap`     | `$x \cap y$`        |    $x \cap y$     |
| 差集运算     |  `\setminus`  | `$x \setminus y$`   |  $x \setminus y$  |
| 同或运算     |  `\bigodot`   | `$x \bigodot y$`    |  $x \bigodot y$   |
| 同与运算     | `\bigotimes`  | `$x \bigotimes y$`  | $x \bigotimes y$  |
| 实数集合     | `\mathbb{R}`  | `\mathbb{R}`        |   $\mathbb{R}$    |
| 自然数集合   | `\mathbb{Z}`  | `\mathbb{Z}`        |   $\mathbb{Z}$    |
| 空集         |  `\emptyset`  | `$\emptyset$`       |                   |

### 数学符号

| 描述             |      符合      | 示例                               |               效果               |
| :--------------- | :------------: | :--------------------------------- | :------------------------------: |
| 无穷             |    `\infty`    | `$\infty$`                         |             $\infty$             |
| 虚数             |    `\imath`    | `$\imath$`                         |             $\imath$             |
| 虚数             |    `\jmath`    | `$\jmath$`                         |             $\jmath$             |
| 数学符号         |   `\hat{a}`    | `$\hat{a}$`                        |            $\hat{a}$             |
| 数学符号         |  `\check{a}`   | `$\check{a}$`                      |           $\check{a}$            |
| 数学符号         |  `\breve{a}`   | `$\breve{a}$`                      |           $\breve{a}$            |
| 数学符号         |  `\tilde{a}`   | `$\tilde{a}$`                      |           $\tilde{a}$            |
| 数学符号         |   `\bar{a}`    | `$\bar{a}$`                        |            $\bar{a}$             |
| 矢量符号         |   `\vec{a}`    | `$\vec{a}$`                        |            $\vec{a}$             |
| 数学符号         |  `\acute{a}`   | `$\acute{a}$`                      |           $\acute{a}$            |
| 数学符号         |  `\grave{a}`   | `$\grave{a}$`                      |           $\grave{a}$            |
| 数学符号         | `\mathring{a}` | `$\mathring{a}$`                   |          $\mathring{a}$          |
| 一阶导数符号     |   `\dot{a}`    | `$\dot{a}$`                        |            $\dot{a}$             |
| 二阶导数符号     |   `\ddot{a}`   | `$\ddot{a}$`                       |            $\ddot{a}$            |
| 上箭头           |   `\uparrow`   | `$\uparrow$`                       |            $\uparrow$            |
| 上箭头           |   `\Uparrow`   | `$\Uparrow$`                       |            $\Uparrow$            |
| 下箭头           |  `\downarrow`  | `$\downarrow$`                     |           $\downarrow$           |
| 下箭头           |  `\Downarrow`  | `$\Downarrow$`                     |           $\Downarrow$           |
| 左箭头           |  `\leftarrow`  | `$\leftarrow$`                     |           $\leftarrow$           |
| 左箭头           |  `\Leftarrow`  | `$\Leftarrow$`                     |           $\Leftarrow$           |
| 右箭头           | `\rightarrow`  | `$\rightarrow$`                    |          $\rightarrow$           |
| 右箭头           | `\Rightarrow`  | `$\Rightarrow$`                    |          $\Rightarrow$           |
| 底端对齐的省略号 |    `\ldots`    | `$1,2,\ldots,n$`                   |          $1,2,\ldots,n$          |
| 中线对齐的省略号 |    `\cdots`    | `$x_1^2 + x_2^2 + \cdots + x_n^2$` | $x_1^2 + x_2^2 + \cdots + x_n^2$ |
| 竖直对齐的省略号 |    `\vdots`    | `$\vdots$`                         |             $\vdots$             |
| 斜对齐的省略号   |    `\ddots`    | `$\ddots$`                         |             $\ddots$             |

### 希腊字母

| 大写字母 |    效果    |    符合    | -   | 小写字母 |            效果            |           符合            |
| :------: | :--------: | :--------: | --- | :------: | :------------------------: | :-----------------------: |
|    A     |  $\Alpha$  |  `\Alpha`  |     |    α     |          $\alpha$          |         `\alpha`          |
|    B     |  $\Beta$   |  `\Beta`   |     |    β     |          $\beta$           |          `\beta`          |
|    Γ     |  $\Gamma$  |  `\Gamma`  |     |    γ     |          $\gamma$          |         `\gamma`          |
|    Δ     |  $\Delta$  |  `\Delta`  |     |    δ     |          $\delta$          |         `\delta`          |
|    E     | $\Epsilon$ | `\Epsilon` |     |    ϵ     | $\epsilon$ ｜$\varepsilon$ | `\epsilon`｜`\varepsilon` |
|    Z     |  $\Zeta$   |  `\Zeta`   |     |    ζ     |          $\zeta$           |          `\zeta`          |
|    H     |   $\Eta$   |   `\Eta`   |     |    η     |           $\eta$           |          `\eta`           |
|    Θ     |  $\Theta$  |  `\Theta`  |     |    θ     |   $\theta$｜$\vartheta$    |   `\theta`｜`\vartheta`   |
|    I     |  $\Iota$   |  `\Iota`   |     |    ι     |          $\iota$           |          `\iota`          |
|    K     |  $\Kappa$  |  `\Kappa`  |     |    κ     |          $\kappa$          |         `\kappa`          |
|    Λ     | $\Lambda$  | `\Lambda`  |     |    λ     |         $\lambda$          |         `\lambda`         |
|    M     |   $\Mu$    |   `\Mu`    |     |    μ     |           $\mu$            |           `\mu`           |
|    N     |   $\Nu$    |   `\Nu`    |     |    ν     |           $\nu$            |           `\nu`           |
|    Ξ     |   $\Xi$    |   `\Xi`    |     |    ξ     |           $\xi$            |           `\xi`           |
|    O     | $\Omicron$ | `\Omicron` |     |    ο     |         $\omicron$         |        `\omicron`         |
|    Π     |   $\Pi$    |   `\Pi`    |     |    π     |      $\pi$ ｜$\varpi$      |     `\pi` ｜`\varpi`      |
|    P     |   $\Rho$   |   `\Rho`   |     |    ρ     |     $\rho$ ｜$\varrho$     |     `\rho`｜`\varrho`     |
|    Σ     |  $\Sigma$  |  `\Sigma`  |     |    σ     |  $\sigma$ ｜ $\varsigma$   |  `\sigma` ｜`\varsigma`   |
|    T     |   $\Tau$   |   `\Tau`   |     |    τ     |           $\tau$           |          `\tau`           |
|    Υ     | $\Upsilon$ | `\Upsilon` |     |    υ     |         $\upsilon$         |        `\upsilon`         |
|    Φ     |   $\Phi$   |   `\Phi`   |     |    ϕ     |     $\phi$ ｜$\varphi$     |    `\phi` ｜ `\varphi`    |
|    X     |   $\Chi$   |   `\Chi`   |     |    χ     |           $\chi$           |          `\chi`           |
|    Ψ     |   $\Psi$   |   `\Psi`   |     |    ψ     |           $\psi$           |          `\psi`           |
|    Ω     |  $\Omega$  |  `\Omega`  |     |    ω     |          $\omega$          |         `\omega`          |

> 大写空心粗体字母

```
$\mathbb{A}$
```

_效果：_
$\mathbb{A}$
