To study an ensemble of systems, it usually requires some assumptions as a starting point, while such assumptions are commonly the preservation of some physical values. A micro-state ensemble makes the assumption that the system mass and energy are both preserved, making it an isolated system.

It might be an interesting question to put: why not the total momentum? The simple answer is that, it wouldn't be possible to study a system of particles without a container --- the inclusion of the container inevitably cause the chance of particles collision with the container, with nearly infinity amount of external momentum that can be exchanged with the system. Understanding the answer to this question may help a lot in understanding why we want to further introduce the canonical ensemble --- controlling the total energy of a system is possible, but also practically extremely hard, while controlling the temperature is much easier, and much more meaningful.

Now it is a good time for us to review some basic equations in theromdynamics, without strict proof. There are a lot, in fact. But here are two of them, both related to the concept of "entropy", are critical to us for now. In deed, they are the key to connect the macroscopic world to the microscopic world.  

1. The entropy $S$ of a system, from the macroscopic view, can be derived by the following differential equation:
$$ dS = \frac{1}{T} dE $$
2. The entropy $S$ of a system, from the microscopic view, can be derived by the Boltzmann's definition, in which $\Omega$ is the total number (or volume, if in continous space) of accessible states of the system, and $k_B$ is the Boltzmann constant:
$$ S = k_B \ln \Omega $$

Since we are using probability to describe the system, the goal thus is to find out the probability density function $\rho(\mathbf{\mu})$, where $\mathbf{\mu}$ is parameterized by some macroscopic measurement. The normalization condition is simple:

$$ \int_{\Omega} d^{6N} \mathbf{\mu} \, \rho(\mathbf{\mu}) = 1 . $$

We stated that the energy of a system here is usually given by the Hamiltonian operator on the (generalized) position parameters $\{q_i\}$ and momentum parameters $\{p_i\}$ of every single particle $i$ out of the $N$ particles in the system:

$$ H(\{q_i\}, \{p_i\}) = \text{kinetic energy} + \text{potential energy} \\ = \sum_{i=1}^{3N} \frac{p_i^2}{2m} + \sum_{i=1}^N \phi(\mathbf{x}_i) .$$

Here $\mathbf{x_i}$ represents the three positional dimensions for particle $i$. The two parts of the Hamiltonian are the kinetic energy and potential energy respectively. Since we are studying a system within a container, the potential energy term $\phi$ is usually ignored.

It however is difficult to calculate the number of accessible states $\Omega$ for any system. Fortunately, we know for a micro-state canonical system, it has simple relationship with the volume of the phase space a sphere in a high-dimension space. But it is also important to remember that, the volume of the state space is not exactly the volume of the phase space! Suppose the volume of the sphere in phase space is $\tilde{\Omega}$, then the actual volume of the $\Omega$ in an isolated system is:

$$ \Omega = \frac{\tilde{\Omega}(E + \Delta E) - \tilde{\Omega}(E)}{N! \, h^{3N}}. $$

Before move on to the discussion on $\tilde{\Omega}$, let's review this relationship between $\Omega$ and $\tilde{\Omega}$. The numerator is simple: it is the volume of the phase space between the two constant energy surfaces. But why is the two factors in the denominator neccessary? And what do they imply? In effect, both of them encourage us to believe that quantum mechanics is a more accurate description of our physical world, while the classical mechanics is just an approximation.

1. About the $N!$ term: Quantum mechanics says that the gas molecules are all identical or indistinguishable, thus won't contribute to the number of "indistinguishable" states. Maybe, I say maybe, the "one-electron universe" hypothesis is right? Maybe the only way to make things different is to make things combined in different ways, while the ingredients (basic particles) are, in fact, the same copy. PBS SpaceTime offers a very good video on this topic: https://dwz.cn/0BLXhiKx
2. About the $h^{3N}$: Superficially, the volume in the phase space is in the dimension of $(\text{momentum} \times \text{distance})^{3N}$, while the number of states that the $\ln$ operator works on should be a dimensionless value. The Planck's constant $h$ has the dimension of $\text{energy} \times \text{time} = \text{momentum} \times \text{distance}$, making $h^{3N}$ cancel out the dimension of $\Omega$. A second thought on this might convince you that the Planck's constant is truely the "basic unit" of the phase space of momentum-position. That's why the uncertainty principle tells us that $q_i \times p_i \ge h$.

Nevertheless, it both terms are just constants for a fixed $N$, thus can be replaced by a single constant variable $C$ if you like. After the $\ln$ operator, it will just become a constant value $-\ln C$ within a very long formula. So it is totally fine if you forget this denominator. 
