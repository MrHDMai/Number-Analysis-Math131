**Numerical Methods with MATLAB - Math 131**
Computational Techniques for Mathematical Problem Solving
Numerical Methods Banner

📂 Repository Structure
This repository contains implementations of fundamental numerical methods in MATLAB, organized by topic:

Folder	Content Description
01. IntroNumericalMethodsComputation_Matlab	Introduction to numerical computing, MATLAB basics, and error analysis.
02. Bisection_FixedPoint_NewtonsMethods	Root-finding algorithms: Bisection, Fixed-Point Iteration, and Newton-Raphson.
03. Interpolation	Polynomial interpolation (Lagrange, Newton’s Divided Differences) and splines.
04. Point_CompositeTrapezoid_Simpsons	Numerical integration: Midpoint, Trapezoidal, and Simpson’s rules.
05. OrdinaryDifferential_IVPS	Solving ODEs: Euler, Runge-Kutta, and boundary value problems.
06. Elimination_Substitution_Factorization	Linear systems: Gaussian Elimination, LU Factorization, and iterative methods.
🚀 Key Algorithms Implemented
Root Finding (02.)
Bisection Method (bisection.m)

Fixed-Point Iteration (fixed_point.m)

Newton’s Method (newton_raphson.m)

Interpolation (03.)
Lagrange Interpolation (lagrange_interp.m)

Newton’s Divided Differences (newton_divided_diff.m)

Integration (04.)
Composite Trapezoidal Rule (trapezoidal.m)

Simpson’s 1/3 Rule (simpsons.m)

Differential Equations (05.)
Euler’s Method (euler_ode.m)

4th-Order Runge-Kutta (rk4.m)

Linear Algebra (06.)
Gaussian Elimination (gaussian_elim.m)

LU Factorization (lu_factorization.m)

🛠 Setup & Execution
Prerequisites
MATLAB R2020a or later

Basic knowledge of calculus and linear algebra

How to Run
Clone the repo:

bash
git clone https://github.com/MrHDMai/Numerical-Analysis-Math131.git
Open MATLAB and navigate to the desired folder (e.g., 02. Bisection_FixedPoint_NewtonsMethods).

Run scripts directly (e.g., bisection.m).

📊 Example Output
Bisection Method (bisection.m)
matlab
f = @(x) x^3 - 2*x - 5;
[root, iterations] = bisection(f, 1, 2, 1e-6);
disp(['Root: ', num2str(root), ' (Found in ', num2str(iterations), ' iterations)']);
Output:

Root: 1.52138 (Found in 24 iterations)
Runge-Kutta 4th Order (rk4.m)
matlab
dydt = @(t,y) -2*y + t;  
[t, y] = rk4(dydt, 0, 1, 0.1, 1);  
plot(t, y);  % Plots the solution curve
📝 Theory Behind the Code
Method	Mathematical Basis	Use Case
Bisection	Intermediate Value Theorem	Bracketing roots of continuous functions
Newton-Raphson	Taylor Series Expansion	Fast convergence near roots
Simpson’s Rule	Quadratic Polynomial Fit	Accurate definite integrals
LU Factorization	Matrix Decomposition	Efficient linear system solving
