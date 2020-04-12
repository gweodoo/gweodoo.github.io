---
title: Publications
layout: default
---

<h3> Checkpoint/Restart approaches for a thread-based MPI runtime
<a href="https://www.sciencedirect.com/science/article/pii/S0167819118303247"
target="_blank" class="btn btn-project">Article</a>
</h3>

ADAM Julien, KERMARQUER Maxime, BESNARD Jean-Baptiste, et al. <br/>
*Parallel Computing*, 2019, vol. 85, p. 204-219.

<details open class="abstract"><summary>Abstract</summary><div class="content">
Fault-tolerance has always been an important topic when it comes to running
massively parallel programs at scale. Statistically, hardware and software
failures are expected to occur more often on systems gathering millions of
computing units. Moreover, the larger jobs are, the more computing hours would
be wasted by a crash. In this paper, we describe the work done in our MPI
runtime to enable both transparent and application-level checkpointing
mechanisms. Unlike the MPI 4.0 User-Level Failure Mitigation (ULFM) interface,
our work targets solely Checkpoint/Restart and ignores other features such as
resiliency. We show how existing checkpointing methods can be practically
applied to a thread-based MPI implementation given sufficient runtime
collaboration. The two main contributions are the preservation of high-speed
network performance during transparent C/R and the over-subscription of
checkpoint data replication thanks to a dedicated user-level scheduler support.
These techniques are measured on MPI benchmarks such as IMB, Lulesh and Heatdis,
and associated overhead and trade-offs are discussed.
</div></details>

<h3>Transparent high-speed network checkpoint/restart in MPI
<a href="https://dl.acm.org/doi/pdf/10.1145/3236367.3236383"
target="_blank" class="btn btn-project">Article</a>
</h3>

ADAM Julien, BESNARD Jean-Baptiste, MALONY Allen D., et al. <br/>
*Proceedings of the 25th European MPI Users' Group Meeting*. ACM, 2018. p. 12.

<details open class="abstract"><summary>Abstract</summary><div class="content">
Fault-tolerance has always been an important topic when it comes to running
massively parallel programs at scale. Statistically, hardware and software
failures are expected to occur more often on systems gathering millions of
computing units. Moreover, the larger jobs are, the more computing hours would
be wasted by a crash. In this paper, we describe the work done in our MPI
runtime to enable transparent checkpointing mechanism. Unlike the MPI 4.0
User-Level Failure Mitigation (ULFM) interface, our work targets solely
Checkpoint/Restart (C/R) and ignores wider features such as resiliency. We show
how existing transparent checkpointing methods can be practically applied to MPI
implementations given a sufficient collaboration from the MPI runtime. Our C/R
technique is then measured on MPI benchmarks such as IMB and Lulesh relying on
Infiniband high-speed network, demonstrating that the chosen  approach is
sufficiently general and that performance is mostly preserved. We argue that
enabling fault-tolerance without any modification inside target MPI applications
is possible, and show how it could be the first step for more integrated
resiliency combined with failure mitigation like ULFM.
</div></details>

<h3>Introducing task-containers as an alternative to runtime-stacking
<a href="https://dl.acm.org/doi/pdf/10.1145/2966884.2966910"
target="_blank" class="btn btn-project">Article</a>
</h3>

BESNARD Jean-Baptiste, ADAM Julien, SHENDE Sameer, et al. <br/>
*Proceedings of the 23rd European MPI Users' Group Meeting.* ACM, 2016. p. 51-63.

<details open class="abstract"><summary>Abstract</summary><div class="content">
The advent of many-core architectures poses new challenges to the MPI
programming model which has been designed for distributed memory message
passing. It is now clear that MPI will have to evolve in order to exploit
shared-memory parallelism, either by collaborating with other programming models
(MPI+ X) or by introducing new shared-memory approaches. This paper considers
extensions to C and C++ to make it possible for MPI Processes to run into
threads. More generally, a thread-local storage (TLS) library is developed to
simplify the collocation of arbitrary tasks and services in a shared-memory
context called a task-container. The paper discusses how such containers
simplify model and service mixing at the OS process level, eventually easing the
collocation of arbitrary tasks with MPI processes in a runtime agnostic fashion,
opening alternatives to runtime stacking.
</div></details>

<h3>A Parallel and Resilient Frontend for High Performance Validation Suites
<a href="http://vecpar.fe.up.pt/2016/docs/VECPAR_2016_paper_25.pdf"
target="_blank" class="btn btn-project">Article</a>
</h3>

ADAM Julien, PÉRACHE Marc <br/>
*International Conference on Vector and Parallel Processing*. Springer, Cham, 2016. p. 248-255.

<details open class="abstract"><summary>Abstract</summary><div class="content">
In any well-structured software project, a necessary step consists in validating
results relatively to functional expectations. However, in the high-performance
computing (HPC) context, this process can become cumbersome due to specific
constraints such as scalability and/or specific job launchers. In this paper we
present an original validation front-end taking advantage of HPC resources for
HPC workloads. By adding an abstraction level between users and the batch
manager, our tool JCHRONOSS, drastically reduces test-suite running time, while
taking advantage of distributed resources available to HPC developers. We will
first introduce validation work-flow challenges before presenting the
architecture of our tool and its contribution to HPC validation suites.
Eventually, we present results from real test-cases, demonstrating effective
speed-up up to 25x compared to sequential validation time – paving the way to
more thorough validation of HPC applications.
</div></details>
