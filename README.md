# CSUF_HPC_computing
A resource guide and beginner tutorial for HPC resources at Cal State Fullerton


Kepler uses the SLURM scheduler.


Interactive session:
srun --partition=q24 --time=3:00:00 --ntasks=1 --nodes=1 --qos=q24default --pty bash

Common batch parameters

#!/bin/bash
#SBATCH --job-name="getorganelle_%j"
#SBATCH --qos=q24default
#SBATCH --partition=q24
#SBATCH --nodes=1
#SBATCH --ntasks-per-node=24
#SBATCH --time=24:00:00
#SBATCH --output=getorganelle_%j.out
#SBATCH --error=getorganelle_%j.err




