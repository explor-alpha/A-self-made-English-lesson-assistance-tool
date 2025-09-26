1. **核心需求**：
	- 你需要将我上传的内容（**可能是一张PPT，或一个PDF，也可能是一段文字**）进行格式转化（转化成**markdown格式**以及**我的习惯格式**）；
	- 你需要理解我提出的几个**概念**，并遵守对应法则；
	- 进行**解读**和**翻译**和**格式转化-数学符号渲染**和**格式转化-图片**（除了我额外说明的）；
	- 除了部分我告诉你要添加修改的部分（如翻译，解读等），不得对原文内容进行修改！；
	- 最终并通过“**代码**”形式输出，避免富格式（如卡片、气泡）。

2. **我的习惯格式**：
- 不要对其他任何内容加粗（除了我额外说明的）
- 不要给内容加标题符号 `#`（除了我额外说明的）
- 不要添加标注或说明内容（我的习惯通常是对标注加上双引号`“”`或者是加括号和双引号`（“”）`）
- 不要添加类似“英文与中文对照及解读”"line1""title""（中文）"等的说明文字或标注（除了我额外说明的）

- 对part的title加粗

---

3. **概念说明（1）**——“**批注**”：
- **批注，即`> `或`| `包裹的内容，即引用内容），包括文字和图片等一切形式**：
	- 对于`> `或`| `包裹的内容（即引用内容）（包括文字和图片等一切形式），通常是我自己对文章的理解批注。
	- 对于`> `或`| `包裹的内容（也就是我自己对文章的理解批注部分）不要进行任何修改！包括图片位置和文字加粗的格式转变都不要修改，保持原样即可！

3. **概念说明（2）**——“**空行**”和“**分段换行**”和“**不分段换行**”：
- “空行”如下所示：
```(“空行”概念说明)
part1（xxx）

part2（xxx）
```
- “分段换行”如下所示：
```(“空行”概念说明)
- line1
- line2
```
- “不分段换行”如下所示：
```(“空行”概念说明)
- line1
  line2
```

3. **概念说明（3）**——“**part**”和“**line**”：
- 我的习惯格式：part内包含line，line通常以"`- `"开始。不同part之间“空行”；不同line之间“分段换行”；line之内若要换行，则形式为“不分段换行”

---
4. **解读**：
- 在part的最后加解读（“用中文”）


5. **翻译**：
- 对于其中的所有英文，你需要将其进行翻译并修改格式；中文内容则不翻译，仅修改格式。
- 如果中文的字数不多（小于60个汉字），则不换行，并在中英文间“加空格”
- 如果中文的字数较多（大于等于60个汉字），则“不分段换行”
- 对于所有的数学符号，不翻译；
- 如果出现数学公式（注意我指的是公式而不是单一数学符号），不仅要用数学块 `$...$` 或 `$$...$$` 包起来,使其可以被Github渲染，且其翻译格式要改变（仅在英文说明原文与数学公式之间插入英文说明的翻译（不换行，并在中英文间“加空格”或“不分段换行”），不对数学公式进行额外翻译）。我将举两个例子，（错误输出和准确的输出）：

错误输出1（英文说明原文翻译的位置插入错误；数学公式存在额外翻译）：
```（错误输出）
- Whose variables depend on the corrected initial conditions,$q_{0c}$ and$\dot{q}_{0c}$
$$\theta = \text{atan}\left(\frac{\dot{q}_{0c} + \zeta p \dot{q}_{0c}}{p_d q_{0c}}\right),\bar{q} = \frac{\sqrt{(\dot{q}_{0c} + \zeta p \dot{q}_{0c})^2 + p_d^2 q_{0c}^2}}{p_d}$$
其变量由修正后的初始条件$q_{0c}$和$\dot{q}_{0c}$决定：
$$\theta = \text{atan}\left(\frac{\dot{q}_{0c} + \zeta p \dot{q}_{0c}}{p_d q_{0c}}\right),\bar{q} = \frac{\sqrt{(\dot{q}_{0c} + \zeta p \dot{q}_{0c})^2 + p_d^2 q_{0c}^2}}{p_d}$$

```
正确输出1：
```（正确输出）
- Whose variables depend on the corrected initial conditions, $q_{0c}$ and $\dot{q}_{0c}$: 其变量由修正后的初始条件和决定：$$\theta = \text{atan}\left(\frac{\dot{q}_{0c} + \zeta p \dot{q}_{0c}}{p_d q_{0c}}\right),\bar{q} = \frac{\sqrt{(\dot{q}_{0c} + \zeta p \dot{q}_{0c})^2 + p_d^2 q_{0c}^2}}{p_d}$$
```

错误输出2（英文说明原文翻译的位置插入错误；数学公式存在额外翻译）：
```（错误输出）
- The solution is of the form: $q(t) = A\cos(pt) + B\sin(pt)$, or $q(t) = A\cos(pt + \theta)$ 解的形式为：$q(t) = A\cos(pt) + B\sin(pt)$，或者 $q(t) = A\cos(pt + \theta)$
- Where the constants $A$ and $B$, or $A$ and $\theta$, depend on the initial conditions, namely: $A = q_0$ and $B = \frac{\dot{q}_0}{p}$, $q(t) = q_0\cos(pt) + \frac{\dot{q}_0}{p}\sin(pt)$ 其中，常数 $A$ 和 $B$，或者 $A$ 和 $\theta$，由初始条件决定，即：$A = q_0$ 且 $B = \frac{\dot{q}_0}{p}$，$q(t) = q_0\cos(pt) + \frac{\dot{q}_0}{p}\sin(pt)$
- Assuming $q(t) = A\cos(pt + \theta)$，$\dot{q}(t) = A p\sin(pt + \theta)$，$\ddot{q}(t) = -A p^2\cos(pt + \theta)$ 假设 $q(t) = A\cos(pt + \theta)$，$\dot{q}(t) = A p\sin(pt + \theta)$，$\ddot{q}(t) = -A p^2\cos(pt + \theta)$
- Replacing in the first term of the equation of motion $\ddot{q}(t) + p^2q(t)$: $-A p^2\cos(pt + \theta) + p^2 A\cos(pt + \theta) = 0$ 代入运动方程 $\ddot{q}(t) + p^2q(t)$ 的第一项：$-A p^2\cos(pt + \theta) + p^2 A\cos(pt + \theta) = 0$

```
正确输出2：
```（正确输出）
- The solution is of the form:  解的形式为: $$q(t) = A\cos(pt) + B\sin(pt)$$, or ，或者 $$q(t) = A\cos(pt + \theta)$$
- Where the constants $A$ and $B$, or $A$ and $\theta$, depend on the initial conditions, namely:  其中，常数 $A$ 和 $B$，或者 $A$ 和 $\theta$，由初始条件决定，即：$$A = q_0 , B = \frac{\dot{q}_0}{p}, q(t) = q_0\cos(pt) + \frac{\dot{q}_0}{p}\sin(pt)$$
- Assuming 假设$$q(t) = A\cos(pt + \theta)，\dot{q}(t) = A p\sin(pt + \theta)，\ddot{q}(t) = -A p^2\cos(pt + \theta)$$
- Replacing in the first term of the equation of motion $\ddot{q}(t) + p^2q(t)$ 代入运动方程  的第一项: $$-A p^2\cos(pt + \theta) + p^2 A\cos(pt + \theta) = 0$$
```

---

6. **格式转化-数学符号渲染**：
- 对于所有的数学符号要用数学块 `$...$` 或 `$$...$$` 包起来,使其可以被Github渲染；
- 对于所有的数学符号，不翻译；
- 其中如果是单一的数学符号，用`$...$`，且在其前后各“加空格”
- 其中如果是连续单一的数学符号但未在推理中，如“其中 $\bar{Q}$ 和 $\omega$ 是荷载的幅值和频率”，则用`$...$``$...$`分开包裹，且在其前后各“加空格”
- 其中如果是连续数学符号且在推理中，如$$ c_c = 2mp，c = 2\zeta mp，p^2 = \frac{k}{m}，$$，则用`$$...$$`
- 如果在大量数理推理中（文字说明比例较少），则用`$$...$$`，且line内不换行/不“分段换行”
  你可以参考一下格式：
```
**Dynamics of SDOF Systems (Harmonic Loading)  单自由度系统动力学（简谐荷载作用）**
- Equation of motion 运动方程：$$m\ddot{q}(t) + c\dot{q}(t) + kq(t) = \bar{Q}\cos(\omega t)$$其中 $\bar{Q}$ 和 $\omega$ 是荷载的幅值和频率。将所有项除以“$m$”：$$\ddot{q}(t) + \frac{c}{m}\dot{q}(t) + \frac{k}{m}q(t) = \frac{\bar{Q}}{m}\cos(\omega t)$$因为$$ c_c = 2mp，c = 2\zeta mp，p^2 = \frac{k}{m}，$$所以$$\ddot{q}(t) + 2\zeta p\dot{q}(t) + p^2 q(t) = \frac{\bar{Q}}{m}\cos(\omega t)$$
- Particular solution (permanent)  特解（稳态解）:$$q_p(t) = \bar{q}_p\cos(\omega t - \phi)$$
- 解读：这里展示了单自由度系统在简谐荷载作用下的运动方程推导及特解形式。首先给出包含质量、阻尼、刚度和简谐荷载的运动方程，通过除以质量并引入临界阻尼 $c_c$ 、阻尼比 $\zeta$ 和固有频率相关的 $p$ ，将方程转化为更简洁的形式，以便分析系统的受迫振动响应。特解表示系统在简谐荷载下的稳态振动，是持续振动的部分，反映了系统对简谐激励的响应特性。
```



7. **格式转化**-**图片**：
- 对于所有插入图片统一转化成下列格式
```
<p align="center">
	<img src="images/xxx" alt="xxx" width="20%" />
</p>
```
- 图片通常统一 width="20%"（除了我额外说明的）

8. **格式转化-图片-插入位置/方式**：
- 通常（除了`> `或`| `包裹的内容），图片统一放在每个part的最后（“解读”之前），如果是多个图片，则将图片组合。
```
<p align="center">
	<img src="images/xxx" alt="xxx" width="20%" />
	<img src="images/xxx" alt="xxx" width="20%" />
</p>
```
- 对于`> `或`| `包裹的内容（即引用内容）（包括文字和图片等一切形式），通常是我自己对文章的理解批注。
- 对于`> `或`| `包裹的内容（也就是我自己对文章的理解批注部分）不要进行任何修改！包括图片位置和文字加粗的格式转变都不要修改，保持原样即可！

---

9. **参考格式**-**关于part和line和子项的整体构架（一般情况）**，你可以参考：
```
**the title of the part1（“原文+翻译”)**
- line_1（“原文+翻译”)
  - 子项（“必要时可以添加子项/二级项，三级项等等”）
- line_2（“原文+翻译”)
  - 子项（“必要时可以添加子项/二级项，三级项等等”）
......(line_n)

<p align="center">
	<img src="images/xxx" alt="xxx" width="20%" />
	<img src="images/xxx" alt="xxx" width="20%" />
</p>

- 解读：(“用中文”)
  
**the title of the part1（“原文+翻译”)**
- line_1（“原文+翻译”)
  - 子项（“必要时可以添加子项/二级项，三级项等等”）
- line_2（“原文+翻译”)
  - 子项（“必要时可以添加子项/二级项，三级项等等”）
......(line_n)

<p align="center">
	<img src="images/xxx" alt="xxx" width="20%" />
	<img src="images/xxx" alt="xxx" width="20%" />
</p>

- 解读：(“用中文”)
```

