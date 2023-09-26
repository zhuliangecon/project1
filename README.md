# Project 1: Hello in Order
This repository contains the code for Project 1: Hello in Order for the course [AMS 530](https://www.stonybrook.edu/commcms/ams/graduate/_courses/ams530.php) at Stony Brook University.

## Project Description
The goal of this project is to write a program that prints the message "Hello from process i out of n" in order, where i is the rank of the process and n is the total number of processes. The program should be able to run on the cluster.

```
project1/
│
├── hello.c                 # Main program entry
├── output.txt              # Output file
├── project1.sh             # Script to execute the program on the cluster
└── README.md               # This documentation file
```

## How to run the program
The program can be executed on the cluster by running the script `project1.sh`. 
The script will compile the program and execute it. 

I used the following commands to run the program on the node `short-28core` on the `login` login node:

```
module load slurm
cd project1
sbatch project1.sh
```
The results will be stored in the file `output.txt`.
