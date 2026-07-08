# Topology-Optimizaiton-Steady-PNP-system

Abstract: As widely used electrochemical storage devices, supercapacitors deliver higher power density than batteries, but suffer from significantly lower energy density. In this work, we propose a topology optimization model for electrode structure to maximize energy storage in supercapacitors. The existence of minimizers to the resulting optimal control problem, which is constrained by a modified steady-state Poisson--Nernst--Planck system describing ionic electrodiffusion, has been theoretically established by using the direct method. Sensitivity analysis of the topology optimization model is rigorously performed to derive variational derivatives and corresponding adjoint equations. A gradient flow formulation discretized by a stabilized semi-implicit scheme is developed to solve the resulting topology optimization problem. Numerical experiments present various porous electrode structures that own large area of electrode-electrolyte interface, demonstrating the effectiveness and robustness of the proposed topology optimization model and corresponding optimization algorithm. 

# Sec 5.1 Numerical accuracy of the PNP solver
We consider a square domain $\Omega = (0,1)^2$ to investigate the numerical accuracy of the solution to the PNP system via the Gummel fixed-point scheme. Let $\phi = x_1$, $z_1=1$, $z_2=-1$, $p=1$, $D_1=1$, $D_0=0.5$, $\epsilon_0=1$, $\epsilon_1=0.5$, $D(\phi)=0.5+0.5\phi$, and $\epsilon(\phi)=1-0.5 \phi$.
$c_1 = \sin(2\pi x_1)\sin(2\pi x_2), c_2 = \sin(3\pi x_1)\sin(3\pi x_2), \psi = \sin(\pi x_1)\sin(\pi x_2)$,

# Sec 5.2 Effect of penalized alpha0 in PNP system
To investigate the numerical influence of the parameter $\alpha_0$ in the modified PNP system \eqref{PNPdis}, which is introduced to suppress the penetration of ions into the electrode region, we carry out numerical tests with different values of $\alpha_0$. We consider a square domain $\Omega=(0,1)^2$ discretized by a quasi-uniform triangular mesh with a mesh size $h=1/128$. The parameters for the PNP system are set as $\epsilon_1 = 0.01$, $\epsilon_0 = 5$, $D_1 = 0.5$, $D_0 = 0.01$, $g = -0.5$, and $c_1^{\infty} = c_2^{\infty} = 0.5$. The phase field function $\phi$ is defined as
\begin{equation}
\left\{
\begin{aligned}
&\phi(x_1,x_2) =1, \quad&& x_1\leq 0.5+0.1\sin(4\pi x_2)-h,\\
&0<\phi(x_1,x_2) <1, &&|x_1- 0.5-0.1\sin(4\pi x_2)|<h,\\
&\phi(x_1,x_2) =0, \quad&& x_1\geq 0.5+0.1\sin(4\pi x_2)+h,
\end{aligned}\right.
\end{equation}
where the interface is parameterized by \( \{(x_1,x_2): x_1 = 0.5 + 0.1\sin(4\pi x_2), x_2 \in [0,1]\}\).

# Sec 5.3 Topology optimization
Example 1: Consider a design domain $\Omega = (0, 1) \times (0, 2)$. Parameters are set as: $ \nu = 2\times 10^{-4}$, $V_0 = 1$, $\Lambda_2 = 10^{-2}$, $N=150$, and $\beta = 500$.

Example 2: In this example, we consider the topology optimization of cylindrical supercapacitors. The design domain $\Omega:=\{(x_1,x_2)\vert 0.04< x_1^2+x_2^2<1 \}$ is given by an annulus centered at the origin $(0,0)$, with the inner and outer ring radii being 0.2 and 1, respectively. The electrode being placed at the outer ring.

Example 3: In this example, we consider topology optimization of maximizing the charge storage of supercapacitors in 3d. The following two cases consider the cubic and cylindrical shapes of electrode structures.
