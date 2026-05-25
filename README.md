# Topology-Optimizaiton-Steady-PNP-system

As widely used electrochemical storage devices, supercapacitors deliver higher power density than batteries, but suffer from significantly lower energy density. In this work, we propose a topology optimization model for electrode structure to maximize energy storage in supercapacitors. The existence of minimizers to the resulting optimal control problem, which is constrained by a modified steady-state Poisson--Nernst--Planck system describing ionic electrodiffusion, has been theoretically established by using the direct method. Sensitivity analysis of the topology optimization model is rigorously performed to derive variational derivatives and corresponding adjoint equations. A gradient flow formulation discretized by a stabilized semi-implicit scheme is developed to solve the resulting topology optimization problem. Numerical experiments present various porous electrode structures that own large area of electrode-electrolyte interface, demonstrating the effectiveness and robustness of the proposed topology optimization model and corresponding optimization algorithm. 

# Numerical accuracy of the PNP solver
We consider a square domain \(\Omega = (0,1)^2\) to investigate the numerical accuracy of the solution to the PNP system via the Gummel fixed-point scheme. Let $\phi = x_1$, $z_1=1$, $z_2=-1$, $p=1$, $D_1=1$, $D_0=0.5$, $\epsilon_0=1$, $\epsilon_1=0.5$, $D(\phi)=0.5+0.5\phi$, and $\epsilon(\phi)=1-0.5 \phi$.
c_1 = \sin(2\pi x_1)\sin(2\pi x_2), c_2 = \sin(3\pi x_1)\sin(3\pi x_2), \psi = \sin(\pi x_1)\sin(\pi x_2),

Example 1: Consider a design domain \(\Omega = (0, 1) \times (0, 2)\). Parameters are set as: \( \nu = 2\times 10^{-4}\), \(V_0 = 1\), \(\Lambda_2 = 10^{-2}\), $N=150$, and \(\beta = 500\).

Example 2: In this example, we consider the topology optimization of cylindrical supercapacitors. The design domain $\Omega:=\{(x_1,x_2)\vert 0.04< x_1^2+x_2^2<1 \}$ is given by an annulus centered at the origin \((0,0)\), with the inner and outer ring radii being 0.2 and 1, respectively. The electrode being placed at the outer ring.

Example 3: In this example, we consider topology optimization of maximizing the charge storage of supercapacitors in 3d. The following two cases consider the cubic and cylindrical shapes of electrode structures.
