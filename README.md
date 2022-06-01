# Delay-data
Delays from a real asynchronous implementation of two asynchronous algorithms (From the experiment in our ICML paper "Delay-Adaptive Step-sizes for Asynchronous Learning")

We run two asynchronous algorithms, PIAG and Async-BCD, in a machine with 10 cores.

PIAG is implemented in a master-worker framework with 8 workers, and Async-BCD uses a shared-memory setting with 8 workers.

The two algorithms are implemented in a real asynchronous way using the MPI4py framework. The file names are {algorithm}_{stepsize}_{dataset}. We consider 3 datasets (RCV1, MNIST, CIFAR100) for two algorithms. We run PIAG with 3 step-sizes (Adaptive 1, Adaptive2, sun), and Async-BCD with 4 step-sizes (Adaptive 1, Adaptive2, sun, Davis).

We log all the delays in 20 different experiment settings.

Please see section 4 of our paper for the details.
