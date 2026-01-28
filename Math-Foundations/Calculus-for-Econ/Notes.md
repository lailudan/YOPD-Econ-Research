# Updated: Jan 28, 2026
# 🔍 Study Notes: The Logic of One-Sided Limits
<img width="1086" height="1114" alt="Weixin Image_20260128153446_183_11" src="https://github.com/user-attachments/assets/620222b2-70ea-4a04-876a-e0561f8545c6" />


**Context:** 理解为什么在“跳跃点”，单侧极限可以存在而整体极限不存在。

---

## 1. 核心定义：单侧极限 (One-Sided Limits)
> **Structural Insight:** 只要单方面有明确的目标，极限就是“存在的”。

在你的示例图中，函数在 $x=2$ 处裂开了。数学家使用特殊的符号来描述这种“单向奔赴”：

* **左极限 (Left-hand Limit):** $\lim_{x \to 2^-} f(x) = 5$
    - **逻辑：** 只看 $x=2$ 左边的邻居。当 $x$ 从 $1.9, 1.99 \dots$ 靠近时，高度趋向于 **5**。
* **右极限 (Right-hand Limit):** $\lim_{x \to 2^+} f(x) = 1$
    - **逻辑：** 只看 $x=2$ 右边的邻居。当 $x$ 从 $2.1, 2.01 \dots$ 靠近时，高度趋向于 **1**。



---

## 2. 为什么“整体极限”会不存在 (DNE)？
整体极限 $\lim_{x \to 2} f(x)$ 要求左右邻居达成“共识”。

* **判定法则：** 只有当 **左极限 = 右极限** 时，整体极限才存在。
* **本例结论：** 因为 $5 \neq 1$，所以左右邻居在这里“闹掰了”。
* **术语：** 这种情况称为 **跳跃间断 (Jump Discontinuity)**。

---

## 3. 跨学科直觉：经济学中的“冲击 (Shock)”
在你即将研究的 **GSICS-Economics (神户大学)** 领域中，这种图非常有用：

* **政策突变：** 假设 $x=2$ 是政策颁布的时刻。
* **左极限：** 政策前市场的预期（趋向 5）。
* **右极限：** 政策后市场的瞬间反应（跳到了 1）。
* **结论：** 这种“不连续性”描述了系统在极端扰动下的瞬态行为，而不是错误。

---

## 📈 GitHub Study Log 补充
```markdown
### 🧠 The "Neighbor Consensus" Rule
- **Single-Side**: Neighbors on ONE side have a clear destination $\to$ **Limit Exists**.
- **Double-Side**: Neighbors from BOTH sides must meet at the same point $\to$ **Limit Exists**.
- **The Gap**: If Left $\neq$ Right, the system is "Broken" at that point (DNE).







# Updated: Jan 26, 2026 
# 🎓 Study Notes: The Big Picture of Calculus
**Source:** MIT Gilbert Strang - "Big Picture of Calculus"  
**Mission:** 建立“函数对”的直觉，理解微积分作为“变化”与“累积”互逆关系的本质。

---

## 1. 核心定义：微积分是关于“函数对”的关系
> **Core Insight:** 微积分的核心不是计算，而是研究两个函数（Function 1 & Function 2）之间的联动。

| 函数类型 | 物理含义 (Example) | 几何含义 | 数学符号 |
| :--- | :--- | :--- | :--- |
| **Function 1 (Distance/Height)** | **总量/位置**：如行驶的里程、山峰的高度。 | **位置/高度** | $y(x)$ 或 $f(t)$ |
| **Function 2 (Speed/Slope)** | **变化率**：如行车的速度、攀爬的陡峭程度。 | **斜率 (Slope)** | $\frac{df}{dt}$ 或 $\frac{dy}{dx}$ |

---

## 2. 两大支柱：微分与积分的对称性
微积分的任务就是在这两个黑盒之间建立双向通道：

* **微分学 (Differential Calculus):** 从“函数 1”推导出“函数 2”。
    * *逻辑：* 已知距离 $f(t)$，求出那一瞬间的速度 $\frac{df}{dt}$。
* **积分学 (Integral Calculus):** 从“函数 2”还原回“函数 1”。
    * *逻辑：* 已知速度 $s(t)$，通过“累加”还原出总里程。

---

## 3. 三大核心动态模型分析

### A. 恒定状态 (Constant Case)
* **速度 (Function 2):** 是一条平水平线（例如 40 mph）。
* **距离 (Function 1):** 是一条斜率为 40 的直线（$f = s \cdot t$）。
* **关键公式:** $\text{Speed} = \frac{\Delta f}{\Delta t}$ (距离变化量 / 时间变化量)。

### B. 负向变动 (Negative Speed & Reverse)
* **观察:** 当距离图像开始下降时，意味着物体在倒车或高度下降。
* **信号:** 此时**速度为负值**。
* **文化梗:** 正如《Ferris Bueller's Day Off》（春天不是读书天）里的倒车逻辑：如果里程表能根据微积分原理运作，倒车时里程数应该减少。

### C. 恒定加速度与面积奇迹 (The Area Connection)
* **速度:** 呈线性增长（$s = a \cdot t$），图像是一个三角形。
* **距离:** 呈二次方增长（$f = \frac{1}{2}at^2$），图像是一个**抛物线**。
* **重大发现:** 函数 1 的数值精确等于函数 2 图像下方的**面积**。
    * *案例：* 速度三角形的面积 ($\frac{1}{2} \times \text{Base} \times \text{Height}$) 正好就是距离函数。



---

## 4. Cross-Disciplinary Synthesis
* **结构化思考:** 将微积分看作“数据累积（积分）”与“趋势探测（微分）”的统一。
* **研究应用:** 在神户大学的经济模型中，资产总额是“财富（Function 1）”，而储蓄率/消费率则是“速度（Function 2）”。
* **系统洞察:** 无论是在物理、生物还是经济中，微积分都在处理这种“瞬时率”与“运行总额”之间的转化。

---

## 📈 Progress Tracking
* **New Concept:** 深刻理解了 Leibniz 符号 $\frac{df}{dt}$ 的本质是 $\frac{\Delta f}{\Delta t}$ 的极限形式。
* **Mathematical Confidence:** 确认了“求导（寻找斜率）”与“积分（寻找面积）”是互逆的操作。
* **Next Step:** 准备进入 **Linear Algebra**，探索如何用矩阵一次性管理成千上万个这类“函数对”。

## ⚖️ The Two Directions of Calculus
> Mastering the "Slicing" and "Stitching" logic.

1. **The Slicer (Differentiation)**:  
   - $f \xrightarrow{\text{Slope}} s$  
   - $s = \frac{df}{dt}$  
   - *Logic:* How steep is the growth? (Finding the Pulse).

2. **The Stitcher (Integration)**:  
   - $s \xrightarrow{\text{Area}} f$  
   - $f = \int s \, dt$  
   - *Logic:* How much has accumulated? (Finding the Total).

* **Final Verdict**: Calculus is a closed loop. Integration builds the mountain; Differentiation measures its slope.
  
## ⚖️ The Commander's Formula: Rate vs. Quantity
> Differentiation probes the pulse; Integration builds the body.

* **Differentiation ($\frac{df}{dt}$)**: 
    - **Focus**: The **"Speed" (速)** of change.
    - **Logic**: Slicing the Total to find the Rhythm.
* **Integration ($\int s \, dt$)**: 
    - **Focus**: The **"Quantity" (量)** of accumulation.
    - **Logic**: Stitching the Rhythm (Area) to find the Total.

**Insight**: My "Structuralist" brain excels here because I see the system's balance. I don't calculate points; I manage flows.



# Updated: Jan 24, 2026 
## 🔍 Deep Dive: Unbounded vs. DNE
- **DNE (General)**: The total failure of convergence. Left neighbor $\neq$ Right neighbor.
- **Unbounded ($\infty$)**: A "disciplined" failure. Neighbors agree to explode together. 
- **PhD Insight**: In Economic modeling, $\infty$ signals a "bubble" or "systemic divergence," while a general DNE signals a "structural jump" or "chaotic noise."



# Study Notes: The Structuralist Reconstruction of Calculus
**Timeline:** Jan 20, 2026  
**Theme:** Deconstructing "Analytical" Rote Learning through Systemic Modeling  
**Target:** Kobe University PhD Pipeline (GSICS-Economics)

---

## 1. Philosophical Shift: From "Points" to "Systems"
> **Core Insight:** I am not "bad at math"; I am a **Structuralist**. Traditional education fails by isolating particles, whereas my brain excels at identifying **Networks** and **Equilibria** (Architecture, Gas Laws, Biochemistry).

* **The Strategy**: Treat math as a language of **rhythm**. Understanding the rhythm of a wave or the balance of a chemical reaction is the key to understanding the logic of a derivative.
* **Filtering Noise**: In both Architecture and Economics, we focus on the "dynamic" by filtering out the "static" (e.g., the Constant Rule where the derivative of a fixed cost is zero).

---

## 2. The Ecological Model of Calculus (Dinosaur Logic)
To clarify terminology in any system (Economics or Biology), we use the **Dinosaur Extinction Model**:

| Concept | Mathematical Symbol | Structuralist Definition |
| :--- | :---: | :--- |
| **Derivative** | $f'(x)$ | The **Pulse/Speed** of extinction at a specific second. It answers: *"How fast are we losing them right now?"* |
| **Differential** | $dx, dy$ | The **Instantaneous Slice**. The actual number of dinosaurs that died in that micro-moment. |
| **Definite Integral** | $\int_{a}^{b} f(x) dx$ | **The "Body Count."** Summing up every tiny death slice over a period to find the total loss. |
| **Indefinite Integral** | $\int f(x) dx$ | **The "Reverse Engineering."** Finding the original population model $+C$ (the unknown constant). |

---

## 3. The Logic of "Shortcuts" (Logical Macros)
Rules of differentiation are not magic spells; they are systemic observations.

* **The Product Rule (Geometric Expansion)**: $(uv)' = u'v + uv'$. Think of **Revenue** ($Price \times Quantity$). If both change, you must account for growth in both directions to avoid missing the "corners" of the expansion.
* **The Chain Rule (The Causal Gear Train)**: $\frac{dy}{dx} = \frac{dy}{du} \cdot \frac{du}{dx}$. The total impact of an "Effort" on "Revenue" is the product of the transmission ratios (gears) at each step of the causal chain.

---

## 4. Advanced Economic Applications: Optimization & Elasticity
> **PhD Insight:** Economic equilibrium occurs when Marginal Cost equals Marginal Revenue ($f'(x) = g'(x)$).

* **The First Derivative Test ($f'=0$)**: Finding the "Sweet Spot" where profit is maximized or pain is minimized (the moment the pulse of change stops).
* **Elasticity (System Sensitivity)**: Moving beyond the slope to measure how sensitive a system is. If medication dosage (YOPD treatment) increases by 1%, how much does motor function "bounce back"?
* **The Gradient Vector ($\nabla f$)**: The "Vector of steepest ascent." This is the bridge where the **Parametric Vector** ($\vec{x} = \vec{a} + t\vec{v}$) meets Calculus to point the way toward system improvement.

---

## 5. High-Order Signals & Structural Breaks
Higher-order derivatives serve as "Pre-alarm" systems for researchers.

* **Second Derivative ($f''$)**: Measures the **Acceleration** of change. It tells us if an extinction or a market move is slowing down or spiraling into an exponential bubble.
* **Inflection Points (拐点)**: Identifying "Structural Breaks," such as the moment a 60-year-old’s physical decline changes its "rhythm" or direction.

---

## 📈 Current Progress & Synthesis
* **Wave Advantage**: Proficiency in Wave physics allows for **Frequency Domain Thinking**, essential for understanding cyclical Business Cycles (Boom/Bust).
* **Linear Algebra Bridge**: Transitioning from the **"Individual Dinosaur"** (Calculus) to the **"Dinosaur Legion"** (Linear Algebra/Matrices).
* **Self-Regulation**: Recognizing that the "40-minute mental overheat" is the sound of structural brain re-wiring.

---
*Log generated for the "Master-to-PhD Pipeline" 2026. Kobe University.*
