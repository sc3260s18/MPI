# MPI Tutorials

You need to have Intel compilers and MPI libraries in your environment 
to run these examples:

	module load Intel IntelMPI

## Running interatively from gateway (outside SLURM)

You should only run MPI jobs from a gateway for very short tests. You can
use the ```mpirun``` command (after loading Intel and IntelMPI libraries)
like so:

	mpirun -n 2 ./mpi_executable

This will run your MPI-supported executable with 2 processes.

## Running within SLURM

SLURM has its own MPI job management command called ```srun```, which you can think of as ```mpirun```. With ```srun``` you do not need to specify the number of processes you would like to launch, SLURM just launches the program with the maximum allowed process for your job allocation (which is specified in the script that you submit to SLURM).

## Order of examples:

1. hello/
2. point_to_point/
3. trapezoid/
4. collective/
	- bcast/
	- scatter/
	- scatterv/
	- scatter_gather/
	- reduce/
5. derived_data_types/
