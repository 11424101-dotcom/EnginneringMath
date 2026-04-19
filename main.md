# 題目五：RLC 電路

## introdution
考慮 RLC 電路，其電流滿足以下微分方程（KVL）：

$$:contentReference[oaicite:0]{index=0}$$

給定輸入電壓：

$$
V(t) = \cos(t)
$$

求電流響應 $$\( i(t) \)$$。

---

## 二、idea with Enginnering Math

：
1. **Laplace transform**
2. equation $$\( I(s) \)$$
3. 做 **Post's inversion formula**


---

## 三、Laplace transform

first define：
$$\[
i(0)=0,\quad i'(0)=0
\]$$

Laplace transform for all equation：

$$\[
L[s^2 I(s)] + R[s I(s)] + \frac{1}{C} I(s) = \frac{s}{s^2+1}
\]$$


$$\[
I(s)\left( Ls^2 + Rs + \frac{1}{C} \right) = \frac{s}{s^2+1}
\]$$

---

## 四、answear $$\( I(s) \)$$

$$\[
I(s) = \frac{s}{(s^2+1)(Ls^2 + Rs + \frac{1}{C})}
\]$$

---

## 五、part of split

if ：

$$\[
I(s) = \frac{s}{(s^2+1)(Ls^2 + Rs + \frac{1}{C})}
\]$$

than：

$$\[
I(s) = \frac{As + B}{s^2+1} + \frac{Cs + D}{Ls^2 + Rs + \frac{1}{C}}
\]$$

than：

1. total amount
2. Comparison coefficient
3. to  A, B, C, D


---

## 六、Post's inversion formula

### first（forced response）

$$\[
\frac{As + B}{s^2+1}
\]$$

對應：

$$\[
A\cos(t) + B\sin(t)
\]$$

this is**orced response**

---

### two （natural response）

$$\[
\frac{Cs + D}{Ls^2 + Rs + \frac{1}{C}}
\]$$

feature ：

$$\[
Ls^2 + Rs + \frac{1}{C} = 0
\]$$

answear：

$$\[
s = \frac{-R \pm \sqrt{R^2 - 4L/C}}{2L}
\]$$

---

## 七、physical meaning

### 判斷是否震盪

看判別式：

$$\[
R^2 - 4L/C
\]$$

---

### 情況分析：

#### ① 過阻尼（Overdamped）
$$\[
R^2 > 4L/C
\]$$

👉 不震盪，直接衰減

---

#### ② 臨界阻尼（Critically damped）
$$\[
R^2 = 4L/C
\]$$

👉 最快回到穩定，不震盪

---

#### ③ 欠阻尼（Underdamped）⭐（會震盪）
$$\[
R^2 < 4L/C
\]$$

👉 解為：

$$\[
i(t) = e^{-\alpha t}(A\cos(\omega t) + B\sin(\omega t))
\]$$

👉 **震盪 + 指數衰減**

---

## 八、最終解結構

$$\[
i(t) = i_{transient}(t) + i_{steady}(t)
\]$$

---

### 暫態解（會消失）
$$\[
i_{transient}(t) = e^{-\alpha t}(\cdots)
\]$$

👉 控制「衰減速度」

---

### 穩態解（最後留下來）
$$\[
i_{steady}(t) = A\cos(t) + B\sin(t)
\]$$

👉 跟輸入頻率一樣（cos t）

---

## 九、工程結論（報告一定要寫）

### 1️⃣ 是否震盪？
取決於：

$$\[
R^2 - 4L/C
\]$$

---

### 2️⃣ 如何衰減？

由指數項決定：

$$\[
e^{-\frac{R}{2L}t}
\]$$

👉 阻尼越大（R 越大） → 衰減越快

---

### 3️⃣ 系統本質

這是一個典型：

- 二階系統
- 有阻尼振盪
- 頻率響應系統

---

## 十、總結（一句話版本）

RLC 電路的電流是：
👉「震盪（sin/cos） + 指數衰減（e^-t）」的組合

---
