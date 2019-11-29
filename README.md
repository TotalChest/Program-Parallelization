# Program-Parallelization
Parallelizing program with OpneMP and MPI on BlueGene and Polus supercomputers  
### Sequence:
```bash
$ gcc original.c -o original
$ ./original
```
### Parallel:
```bash
$ export OMP_NUM_THREADS=$1    # $1 = 1/2/4/8/32/64/128  
$ gcc OpenMP-first.c -o first -fopenmp
$ gcc OpenMP-second.c -o second -fopenmp
$ gcc OpenMP-double.c -o double -fopenmp
$ ./first
$ ./second
$ ./double
```
