
Original Equation: $$y' - 2y = e^x y^3$$

This is a Bernoulli equation of the form: $$\Rightarrow y' + P(x)y = Q(x)y^n$$

Substitution: Let $v = y^{1-n} = y^{-2}$

Differentiating with respect to $x$: $$\frac{dv}{dx} = -2y^{-3} y'$$

Transformation: Multiply the original equation by $y^{-3}$: $$y^{-3} y' - 2y^{-2} = e^x$$

Substitute $v$ and $v'$ into the equation: $$\Rightarrow -\frac{1}{2} v' - 2v = e^x$$

Rearrange into standard linear form: $$v' + 4v = -2e^x$$

Integrating Factor: $$\mu = e^{\int 4 dx} = e^{4x}$$

Multiply the linear equation by the integrating factor: $$e^{4x} v' + 4e^{4x} v = -2e^{5x}$$ $$\frac{d}{dx}(e^{4x} v) = -2e^{5x}$$

Integration: $$e^{4x} v = \int -2e^{5x} dx = -\frac{2}{5} e^{5x} + C$$

Solve for $v$: $$v = -\frac{2}{5} e^x + Ce^{-4x}$$

Final Solution: Substitute back $v = y^{-2}$: $$y^{-2} = -\frac{2}{5} e^x + Ce^{-4x}$$

----

# Topic

y' - 2y = e^x y^3

---

y' + (-2)y = e^x y^3

- P(x) = -2
- Q(x) = e^x
- n = 3

---

## transfrom of variable

if
v = y^(1-n) = y^(-2)

⇒ dv/dx = -2y^(-3) y'

---

y^(-3)y' - 2y^(-2) = e^x

⇒ -1/2 v' - 2v = e^x

multiplication -2：

v' + 4v = -2e^x

---

μ = e^(∫4dx) = e^(4x)

⇒ d/dx (e^(4x)v) = -2e^(5x)

---

e^(4x)v = -2/5 e^(5x) + C

---

return 
v = y^(-2)

⇒ y^(-2) = -2/5 e^x + Ce^(-4x)

---

## Answear

y = 1 / √(-2/5 e^x + Ce^(-4x))

---

---

## 📌 題目二：二階線性非齊次微分方程

### 題目
y'' + y = x^2

---

### 解題步驟

#### 1️⃣ 齊次解
y'' + y = 0

特徵方程：
r^2 + 1 = 0  
⇒ r = ±i

⇒ y_h = C1 cos(x) + C2 sin(x)

---

#### 2️⃣ particular 解（待定係數法）
猜：
y_p = Ax^2 + Bx + C

---

#### 3️⃣ 計算導數
y_p' = 2Ax + B  
y_p'' = 2A  

---

#### 4️⃣ 代回原式
y'' + y = x^2

⇒ 2A + (Ax^2 + Bx + C) = x^2

⇒ Ax^2 + Bx + (C + 2A) = x^2

---

#### 5️⃣ 比較係數
A = 1  
B = 0  
C + 2A = 0 ⇒ C = -2  

---

#### 6️⃣ particular 解
y_p = x^2 - 2

---

### ✅ 最終解
y = C1 cos(x) + C2 sin(x) + x^2 - 2

---

## 🔥 總整理

### 題型判斷

- 題目1：Bernoulli（有 y^n）
- 題目2：二階常係數非齊次

---

### 解題套路

#### Bernoulli
1. 看出 y^n  
2. 設 v = y^(1-n)  
3. 轉線性  
4. 積分因子  

---

#### 二階非齊次
1. 解齊次（特徵方程）  
2. 猜 particular  
3. 代回比係數  

---