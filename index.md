---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

Position & Education
============

### => Since 2019 -- *Teaching Assistant -- Université de Versailles Saint-Quentin (UVSQ) -- France*
Part of the High-Performance and Simulation (CHPS) master degree, the Advanced
Architecture of Operating Systems (AISE) course covers from the basics of use in
Unix Operating Systems (like processes, threads, synchronizations) to more complex
architectures (kernel, scheduling, virtualization). In that context, I share the
lead of this course gathering around 45 hours of teaching a year.


### => 2015 - Present -- *HPC Junior Developer & Consultant -- ParaTools SAS -- France*
As a individual part of this small company, the purpose of ParaTools is to
provide a highly specialized consulting support relatively to High performance
Computing solutions. More specifically, if this company was initially focused on
performance, thanks to the support the performance analysis tool, TAU. The French
affiliate covers a larger area, mainly focused on developing inside runtimes
(MPI, OpenMP). In that context, I contributed to multiple areas of interest and feed my knowledge among the following:

* GCC and its overall compilation chain (front-ends, GIMPLE, IR, plugins...)
* High-speed networks through their optimization inside an MPI runtime (IB,
Portals, SHMEM, OFI)
* Thread-level Storage mechanism through a complete rewrite of this support on
 top of hierarchical user-level thread model, mimicking the same capabilities as usually exposed with a regular `__thread` keyword. 
* Accelerators, mainly CUDA-capable oriented.
* Broad knowledge of HPC-specific programming models. (MPI, OpenMP.) Have been involved in the MPI Forum to release the MPI 4.0 standard.
* Low-level system engineering (ELF rewriting)


### => 2012 - 2015 -- *Apprenticeship as part of Engineering School -- ECE Paris -- France*
With the advent of new methods of learning, I got the change to almost make my
studies split half-time in school and as an internship in a company. In that
context, I joined a French leader in HPC research, known as the "Commissariat à
l'Énergie Atomique et aux Énergies Alternatives" (aka CEA) and been associated with
the development of an MPI runtime called MPC. Among the goals I contributed to:
* Deployment of a standalone non-regression base for open-source applications,
aware of HPC specifications and limitations.
* Study of several checkpoint-restart tools, to determine the best one to be
used in place of the current method of checkpoint and restore applications inside
  MPC.
* Development of a "test scheduler,” aware of HPC capacities and able to scale,
allowing any CI system to optimize their time to result.

Software Projects
=================

### Multi-Processor Computing
The MPC (Multi-Processor Computing) framework provides a unified parallel runtime designed to improve the scalability and performances of applications running on clusters of (very) large multiprocessor/multicore NUMA nodes. Thanks to its design, MPC allows mixed-mode programming models and efficient interaction with the HPC software stack. MPC is available under the CeCILL-C license, which is a French transposition of the LGPL and is fully LGPL-compatible.

### JCHRONOSS
JCHRONOSS is a tool helping to maintain a high level of quality in your project by making the validation process easier and faster. Initially suited for High Performance Computing test suites, JCHRONOSS is able to distribute thousands of parallel jobs in parallel environments and over large supercomputers. Designed with a high level of abstraction, JCHRONOSS can work with any kind of batch managers or architectures. Some extra features embedded with JCHRONOSS like scheduling visualization and standalone result reviewing, makes JCHRONOSS a complete and powerful tool for most of validation suites.

### PCVS

Skills & Certifications
=======================

* **HPC**: MPI, OpenMP, Threads, CUDA, Docker, Spack, SLURM, Portals4, OFI,
Remote Debugging
* **Languages**: C/C++, Perl (5/6), Python (2/3), Shell, LaTeX, Redis, Gnuplot, Web Tech., Java Family, Redis
* **Software Engineering**": Git, SVN, CMake, Autotools, Gitlab, Jenkins, Scrum, ITIL
* **Certified Completed Online Courses**:
	- [S190.1x: Scalable Machine Learning] (https://verify.edx.org/cert/d53680539ea545bbae9509093f3a6668) -- UC BerkeleyX -- 100%
	- [CS002x : Programming in Scratch] (https://verify.edx.org/cert/b6477262b58c44cb8662ede4766d53bf) -- HarveyMuddX -- 96%
	- [DEV203x : Introduction to Bootstrap] (https://verify.edx.org/cert/770b5514826d4be9bfd27b4ff98f12d0) -- MicrosoftX -- 78%
	- [LFS101x.2 : Introduction to Linux] (https://verify.edx.org/cert/b028f09211754025b050d9f30699d44e) -- LinxuFoundationX -- 97% 

Publications
============

* ADAM, Julien, KERMARQUER, Maxime, BESNARD, Jean-Baptiste, et al.
 " __Checkpoint/restart approaches for a thread-based MPI runtime.__" *Parallel
  Computing*, 2019, vol. 85, p. 204-219.
* ADAM, Julien, BESNARD, Jean-Baptiste, MALONY, Allen D., et al." __Transparent
high-speed network checkpoint/restart in MPI.__" In : *Proceedings of the 25th
European MPI Users' Group Meeting*. ACM, 2018. p. 12.
* BESNARD, Jean-Baptiste, ADAM, Julien, SHENDE, Sameer, et al." __Introducing
task-containers as an alternative to runtime-stacking.__" In : *Proceedings of
the 23rd European MPI Users' Group Meeting.* ACM, 2016. p. 51-63.
* ADAM, Julien et PÉRACHE, Marc." __A Parallel and Resilient Frontend for High
Performance Validation Suites.__" In : *International Conference on Vector and
Parallel Processing*. Springer, Cham, 2016. p. 248-255.

Contact
=======

Email: [julien@adamarie.pro] (mailto:julien@adamarie.pro)
Linkedin: [julienadambeulin] (https://linkedin.com/in/julienadambeulin) {:target="_blank"}
Website: [julien.adamarie.pro] (https://julien.adamarie.pro) {:target="_blank"}
