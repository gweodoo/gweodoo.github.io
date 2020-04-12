---
title: Contributed Projects
layout: default
---

<h1>Multi-Processor Computing
<a href="https://mpc.hpcframework.com" target="_blank" class="btn-project">Project homepage</a>
<a href="https://mpc.hpcframework.com/download" target="_blank" class="btn-codebase">Code base</a>
</h1>

![mpc-logo](/assets/img/mpc.png){:class="img-responsive img-projects"}

The MPC (Multi-Processor Computing) framework provides a unified parallel
runtime designed to improve the scalability and performances of applications
running on clusters of (very) large multiprocessor/multicore NUMA nodes. Thanks
to its design, MPC allows mixed-mode programming models and efficient
interaction with the HPC software stack. MPC is available under the CeCILL-C
license, which is a French transposition of the LGPL and is fully
LGPL-compatible.

I have been brought to contribute on a wide variety of components including:
* Low-level network programming (TCP, OFI, Portals4)
* Privatization mechanism through low-level TLS mechanism
* Compilation workflow, ELF format (GCC & Binutils patches)
* Accelerators, main focus on CUDA-capable GPUs 
* QA Management (tests, validation suite...)
* Build system


<h1>Parallel Computing -- Validation Suite
<a href="https://pcvs.hpcframework.com" target="_blank" class="btn-project">Project homepage</a>
<a href="https://github.com/cea-hpc/pcvs" target="_blank" class="btn-codebase">Code base</a>
</h1>

**Parallel Computing -- Validation Suite** (PCVS for short) is a validation engine
designed to help users to run large test bases in a scalable manner, by taking
advantage of highly parallel environments to reduce their time to result,
improving subsequently the project efficiency thanks to a more regular
validation process. While designed to answer validation needs in
High-Performance Computing, PCVS is not limited to such projects and can run any
kind of test suites over multiple types of architectures. Through a large range
of configuration, PCVS makes no assumptions about any HPC-related concepts and
can easily translate from a validation run on an Exascale machine to a simple
workstation. 

Based on preliminary work from a validation system made for the MPC framework, I
initiated (now under [CEA](www.cea.fr) leadership) this parallel validation
system as a unified approach for validating:
* Heterogenous benchmarks
* Libraries and tools against their standards,
* in a reproducible way, restricting capabilities for tests to alter their
  environment on their own.
* With one of the highest level of customization to fit any needs.
* code bases managed by a package manager (e.g: Spack)

Depsite the fact the project is in Perl, It should be considered to be
rewritten to ease support and contributions. Most HPC developers are likely to
be more proficient in Python than Perl and it would be the best alternative to
keep PCVS growing.

<h1>JCHRONOSS
<a href="https://jchronoss.hpcframework.com" target="_blank" class="btn-project">Project homepage</a>
<a href="https://jchronoss.hpcframework.com/downloads" target="_blank" class="btn-codebase">Code base</a>
</h1>

JCHRONOSS is a tool helping to maintain a high level of quality in your project
by making the validation process easier and faster. Initially suited for High
Performance Computing test suites, JCHRONOSS is able to distribute thousands of
parallel jobs in parallel environments and over large supercomputers. Designed
with a high level of abstraction, JCHRONOSS can work with any kind of batch
managers or architectures. Some extra features embedded with JCHRONOSS like
scheduling visualization and standalone result reviewing, makes JCHRONOSS a
complete and powerful tool for most of validation suites.

This is a preliminary work I've made to bootstrap an existing validation system
with a test orchestrator able to scale with most supercomputers/batch managers.
Even if it can be used in a standalone way, it is most known today to be part of
the PCVS tool, relying on JCHRONOSS to run jobs in parallel inside a given
allocation.

<h1>Automatic Privatization System
<!--<a href="#" target="_blank" class="btn-project">Project homepage [dead]</a>
<a href="#" target="_blank" class="btn-codebase">Code base [dead]</a>-->
</h1>
The Automatic Privatization system (informally known as "AutoPriv") is a
complete toolchain allowing users to translate a given source code from a
process perspective (to be run per process) to a thread perspective (to be run
inside threads, concurrently to others). Initially part of the MPC framework, it
has been (or is going to be) released as a solution on its own. Thanks to a
support from the compiler (currently GCC, Intel & PGI) and linker effort
(currently only for GCC support), Autopriv intends to let you run a `main()`
function multiple times, from multiple concurrent threads, without having to
modify the original source code. Autopriv is designed to work with C, C++ &
Fortran codes.

From components coming from the MPC framework, I initiated this project as a
gathering of contributions. By rewriting the complete TLS support for GCC (from
low-level code injections to ELF access optimizations), it significantly reduced
the overhead induced by replacing global variables with TLS accesses.

<h1>Distributed MultiThreaded CheckPointing
<a href="https://dmtcp.sourceforge.net" target="_blank" class="btn-project">Project homepage</a>
<a href="https://github.com/dmtcp/dmtcp" target="_blank" class="btn-codebase">Code base</a>
</h1>

DMTCP transparently checkpoints a single-host or distributed computation in
upser-space -- with no modifications to user code or the O/S. It works on most
LInux applications, including Python, Matlab, R, GUI desktops, MPI, etc. It is
robust and widely used. It also supports the commonly used OFED API for
Infiniband as well as its integration with various implementations of MPI and
resource managers (e.g., SLURM).

As part of my work at Paratools SAS, I attempted to integrate a checkpoint-restart
support for the MPC framework. It leads to multiple improvements and/or fixes
during the process we then reversed to the community.

<h1>Gweodev
<a href="https://github.com/gweodoo/gweodev.git" target="_blank" class="btn-project">Project homepage</a>
<a href="https://github.com/gweodoo/gweodev.git" target="_blank" class="btn-codebase">Code base</a>
</h1>

As part of my day-to-day workflow, "Gweodev" is a environment & tool self-deployment, gathering anything I need to set up properly a new workstation.
It includes configurations for and setup rules for (but not bound to):
* Git  (including `.gitconfig`, `.gitattributes` & `.gitignore`)
* Vim RC file + plugin (through Vundle)
* Tmux
* i3
* zsh / bash (colorscheme, completions, aliases & functions)
* gdb
* Anything relevant for proper developement use (tig, diff-so-fancy...)
