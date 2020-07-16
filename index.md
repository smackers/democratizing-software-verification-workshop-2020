
In the past decades we have witnessed major advances in the power of automated reasoning engines like Satisfiability Modulo Theories (SMT) and Horn clause solvers. As a consequence, there has been a renaissance of software verification based on this technology. Currently, there are a number of mature verifiers available coming both from academia and industry. However, despite these advances, the bar for newcomer researchers to contribute to this field is still very high. One of the main obstacles is the very large cost of development of a new software verifier from scratch. Hence, several groups have been independently working on implementing open software verification infrastructures, which would allow for easier prototyping of research ideas in this space, e.g., new algorithms for verifying relational or timing properties, thereby democratizing software verification.

This workshop aims to bring together the developers of open software verification infrastructures and their potential clients, meaning researchers and practitioners interested in developing prototypes of software verification algorithms. We will structure the workshop to facilitate the exchange of ideas and discussions between the developers and clients. First, the workshop will start with short tutorials on several open software verification infrastructures, such as [SMACK] and [SeaHorn]. This will be followed by presentations of projects that already leverage these infrastructures, such as a side-channel attacks verifier and a firmware verifier. We also hope to attract potential new clients as well, who would present the requirements of their projects through a series of lightning talks. Through open discussions we will solicit feedback from the community on the requirements and functionality that open research infrastructures should include to make them more widely usable.

As further discussion topics, we will solicit talks and feedback on benchmarking issues, reproducibility, input languages, and potential license issues, all of which are important to have a viable software verification research ecosystem that can be leveraged by both industry and academia.

## Location

The [#workshop-democratize-sv](https://cav2020.slack.com/archives/C016WTZTBGV) channel of CAV 2020 on Slack. Zoom meeting info will be posted there.

## Program

### Hydra: A Framework For Distributed Program Verification (6:00am PDT)

Program verification is a computationally intensive task. However, most
state-of-the-art verifiers are unable to utilize readily available large
computational resources. In this work, we design an algorithm for
parallelizing SMT-based automated program verification. Our algorithm can
split large verification tasks into smaller sub-tasks by utilizing
information from the SMT solver and solve them in parallel on clusters of
machines. We implement the proposed algorithm in a tool called HYDRA which
is built on top of CORRAL, the verifier used by Microsoft's Static Driver
Verifier and evaluate its performance on hard Windows device driver
benchmarks.

presented by **Prantik Chatterjee**

### CIVL-ized Concurrent Programs (6:30am PDT)

The CIVL verifier allows the construction of safety proofs for concurrent
programs across multiple layers of refinement. Each refinement step focuses on a
small simplifying program transformations, making proofs more manageable and
reusable, and specifically eliminating the need to write complex invariants on
the low-level encoding of the program as a flat transition system. Modular
refinement reasoning is supported by a flexible combination of invariants,
reduction, and linear permissions.

In this talk, we will report on CIVL from the perspective of verification
features, programmer interaction, and the implementation atop Boogie.

presented by **Bernhard Kragl**

### A Guided Tour of a Static Analyzer for Data Science Software (7:00am PDT)

Nowadays, data science software and notably machine learning plays an increasingly important role in our daily lives. It thus becomes of paramount importance to have effective verification tools available to prove its correctness and reliability.

In this talk we will take you sightseeing through the architecture of Lyra, a static analyzer for Python components of a data science pipeline. The main attractions will be the submodules expressly designed to be stand-alone and reusable by other verification tools as well as the abstract domains designed to address new and challenging research problems that arise from targeting data science software.

presented by **Caterina Urban**

### Machine Learning based Program Analysis (7:30am PDT)

Program analysis has been widely adopted in both academia and industry to enhance the correctness, safety, and performance of programs. However, the effectiveness and scalability of existing program analyzers are often limited by suboptimal, manual design decisions. This talk will discuss two new program analysis techniques based on machine learning. First, I will introduce Lait, a learning based approximate transformer that removes redundant computation from static numerical analysis traces. Second, I will present ILF, a novel fuzzing method that learns to generate test inputs from symbolic execution traces. These techniques integrate domain knowledge in program reasoning for designing the learning algorithms, enabling fast and effective program analyses.

presented by **Jingxuan He**

### TBD (8:00am PDT)

presented by **Alex Summers**

## Registration

Please register for the workshop through the CAV registration [page](http://i-cav.org/2020/attending/).


## Organization

This workshop will be held on July 20, 2020, and coinciding with the [32nd International Conference on Computer-Aided Verification (CAV)][CAV]. The workshop is chaired by developers of [SMACK] and [SeaHorn]:

* Michael Emmi, Amazon Web Services
* Arie Gurfinkel, University of Waterloo
* Jorge Navas, SRI International

[SMACK]: http://smackers.github.io
[SeaHorn]: https://seahorn.github.io
[CAV]: http://i-cav.org/2020/
