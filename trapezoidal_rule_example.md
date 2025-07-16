
# Numerical Integration: Trapezoidal Rule

## Trapezoidal Rule Formula

To approximate the integral

∫ₐᵇ f(x) dx

using the Trapezoidal Rule with n subdivisions:

∫ₐᵇ f(x) dx ≈ Tₙ = (h/2) [ f(x₀) + f(xₙ) + 2 Σᵢ₌₁ⁿ⁻¹ f(xᵢ) ]

where

h = (b - a) / n, xᵢ = a + i h, i = 0,1,...,n.

---

## Example: Approximate ∫₀¹ e^{4x²} dx with n=7

### Step 1: Compute step size h

h = (1 - 0)/7 = 1/7 ≈ 0.142857.

### Step 2: Compute the points xᵢ and function values f(xᵢ) = e^{4xᵢ²}

| i | xᵢ = i/7 | f(xᵢ) = e^{4xᵢ²}          |
|---|----------|----------------------------|
| 0 | 0        | 1.00000000000              |
| 1 | 0.142857 | 1.08505714419              |
| 2 | 0.285714 | 1.38615068230              |
| 3 | 0.428571 | 2.08484367736              |
| 4 | 0.571429 | 3.69183066048              |
| 5 | 0.714286 | 7.69688981037              |
| 6 | 0.857143 | 18.89269822665             |
| 7 | 1        | 54.59815003314             |

### Step 3: Apply the Trapezoidal Rule formula

T₇ = (h/2) [ f(x₀) + f(x₇) + 2 Σᵢ₌₁⁶ f(xᵢ) ]  
= (1/7)/2 [1.00000000000 + 54.59815003314 + 2(1.08505714419 + 1.38615068230 + 2.08484367736 + 3.69183066048 + 7.69688981037 + 18.89269822665)]  
= (1/14) [55.59815003314 + 2 × 34.83747020135]  
= (1/14) × 125.27309043584  
= 8.94807788827

### Final answer:

∫₀¹ e^{4x²} dx ≈ **8.9481**

---

*Feel free to ask if you want me to help create more examples or explanations in Markdown!*
