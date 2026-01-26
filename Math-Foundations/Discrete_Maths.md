### 🗓 1/25 Mathematics for Computer Science & Linear Algebra
> **Progress**: Started MIT 6.042J (Lec 1) and mastered the visual derivation of Linear Transformations.


#### 1. Logic & Proofs (MIT 6.042J Lec 1)
* **What is a Proof?**: A verification of a **Proposition** through a sequence of logical deductions starting from **Axioms**.
* **The "Induction" Trap**: Proving a case for $n=1, 2, ... 40$ does not constitute a proof for all $n$. Mathematics requires absolute logical necessity, not just patterns.
* **Gödel’s Incompleteness**: No set of axioms is both **Consistent** (no contradictions) and **Complete** (can prove everything). There will always be true statements that are unprovable.


### Lec 1: 证明、猜想与逻辑的边界

**1. 数学真理的绝对性**
- 法律真理靠辩论，科学真理靠实验，数学真理靠逻辑。
- 在逻辑面前，没有等级之分，只有证明的严密性。

**2. 著名的逻辑挑战**
- **四色定理 (Four Color Theorem)：** 第一个由计算机辅助证明的定理。它告诉我们，复杂系统的冲突（着色）存在理论上限，同时也引发了关于“人脑无法验证的证明是否可靠”的信任博弈。
- **哥德巴赫猜想 (Goldbach's Conjecture)：** “任一大于2的偶数都可写成两个质数之和”。极其简单的表述，却拥有极其复杂的底层逻辑。它展示了数学中“显而易见”与“难以证明”之间的鸿沟。
- **黎曼假设 (Riemann Hypothesis)：** 关乎素数分布的终极奥秘。莱顿教授用它说明，有些命题即使我们直觉上认为它是真的，但在没有逻辑闭环（证明）之前，它永远只能是猜想。

**3. 个人思考 (Personal Insight)**
- **识别恶意与反例：** 就像数学家寻找黎曼假设的反例一样，我的“直接反击”和“深度追问”是在寻找社会博弈中的“逻辑断裂点”。
- **Hidden Agenda：** 哥德巴赫猜想提醒我，表面简单的现象背后可能隐藏着极深层的机制。作为研究者，我不能满足于“看起来是真的”，必须追求“证明它是真的”。
- **决策止损：** 面对像黎曼假设这样耗费无数天才精力的难题，我也学到了在博弈中何时应用“秘书理论”进行止损——在不确定性中寻找那个最稳健的满意解。

**4. 真值表 (Truth Table) —— 逻辑的现形镜**
- **定义：** 穷举所有命题组合的真假情况，验证复杂逻辑项的最终值。
- **实战应用：** - 拆解“如果...那么...”的诱导性承诺。
    - 识别逻辑断裂点：如果前提为真但结论为假，则该逻辑路径必为伪。
    - 离散数学里的核心：与 (AND)、或 (OR)、非 (NOT)
      与(AND)： 必须两个都是真的，结果才是真。（就像婚姻，必须两个人都忠诚才叫忠诚）。
      或 (OR)： 只要有一个是真的，结果就是真。（就像逃生出口，左边或右边开了都能活）。
      非 (NOT)： 把真相倒过来。（骗子最擅长的，指鹿为马）。
- **感悟：** 真值表让我明白，反诈不需要读心术，只需要把对方的陈述代入真值表进行“一致性检测”。
