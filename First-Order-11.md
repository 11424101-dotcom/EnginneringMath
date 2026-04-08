Bernoulli Differential Equation
Constant transform function And Differentiation
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

$$y = \frac{1}{\sqrt{-\frac{2}{5} e^x + Ce^{-4x}}}$$