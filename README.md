Patus
=====
Reference repository:
https://github.com/matthias-christen/patus
=====
In many numerical codes, ranging from simple PDE solvers to complex AMR and multigrid solvers, the class of stencil computations is a constituent class of kernels. Oftentimes, stencil computations comprise a dominant part of the compute time. Therefore, in order to minimize the time to solution, it is crucial that the stencil kernels make use of the available computing resources as efficiently as possible.

The Patus framework is a code generation and autotuning tool for the class of stencil computations. The idea behind the Patus framework is twofold: on the one hand, it provides a software infrastructure for generating architecture-specific (CPUs, GPUs) stencil code from a specification of the stencil incorporating domain-specific knowledge that enables optimizing the code beyond the abilities of current compilers. On the other hand, it aims at being an experimentation toolbox for parallelization and optimization strategies. Using a small domain specific language, the user can define the stencil kernel as shown in the example. Predefined strategies describe how the kernel is optimized and parallelized. Or custom strategies can be designed to experiment with other algorithms or to find a better mapping to the hardware.
