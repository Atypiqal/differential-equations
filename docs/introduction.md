#### The mission:

Apply the algorithm from the paper to a simple, well-undesrtood physical system:
**the quantum harmonic oscilator**
Specically, implement a quantum algorithm to solve:

$$y''+\omega²y = 0, \quad y(0)= 1, \quad y'(0)=1, \quad \omega=1$$

Once implemented, **use the resulting quantum state** to evaluate the **system's kinetic and potential energies as a function of time** in the interval  $[0,1]$.

Explore **how varying algorithmic parameters**, such as the bounds used in `inplace_prepare_state()`, **affects the accuracy of these energy values**.

Finally, analyze how resource-efficient your implementation is by comparing circuit depth and width under different optimization settings.

#### Problem cited from the paper
> The description of the problem for solving LDEs is as follows.
> A unknown vector $x(t)$ starts from a $x(0)$ and follows an evolution described by and LDE $$\frac{dx(t)}{dt} = Mx(t) + b,$$
> where where $M$ is an arbitrary $N\times N$ matrix, while $b$ and $x(t)$ are $N$-dimenional vectors

We known that the analytical solution of the equation can be written as $$x(t) = e^{Mt} x(0) + (e^{Mt} - I)M^{-1} $$