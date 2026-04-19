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

### Determine whether there is a shock

see ：

$$\[
R^2 - 4L/C
\]$$

---

### situation analysis：

#### ① Overdamped
$$\[
R^2 > 4L/C
\]$$


---

#### ② Critically damped
$$\[
R^2 = 4L/C
\]$$



---

#### ③ Underdamped will vibrate
$$\[
R^2 < 4L/C
\]$$

👉 answear ：

$$\[
i(t) = e^{-\alpha t}(A\cos(\omega t) + B\sin(\omega t))
\]$$

👉 **Oscillation + Index Decline**

---

## 八、final solution structure

$$\[
i(t) = i_{transient}(t) + i_{steady}(t)
\]$$

---

### Transient solution (will disappear)
$$\[
i_{transient}(t) = e^{-\alpha t}(\cdots)
\]$$


---

### Steady-state solution (left at the end)
$$\[
i_{steady}(t) = A\cos(t) + B\sin(t)
\]$$

-> Same as the input frequency (cos t)

---

## 九、Engineering conclusion

### 1️⃣ Is it oscillating？


$$\[
R^2 - 4L/C
\]$$

---

### 2️⃣ How to attenuate


$$\[
e^{-\frac{R}{2L}t}
\]$$

The greater the damping (the larger the R), the faster the decay.

---


