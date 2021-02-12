# Register Allocation Pseudo-Boolean Optimization Problems

## Overview
This repo contains Pseudo-Boolean Optimization problems that represent a register allocation
for a function. The problems are broken into directories based on the source code the problems
were derived from. For
more on register allocation and Pseudo-Boolean Optimization see [here](https://dash.harvard.edu/handle/1/37364763).

## solver_test Script
The solver_test script provides an easy way to solve the problems using your favorite solver.
It must be invoked with the *--solver* argument which is the invocation of the PBO solver. For example, if
your solver is located at /home/username/foo/solver and you want to provide it the option *-bar 10*, you
could run the following:

        ./solver_test --solver "/home/username/foo/solver -bar 10"

The results will be placed in a .csv file with row format:

 FILENAME,time

The time is measured in the script and is neither the clock time reported by the solver
nor a precise measurement of the solver clock time.

### Options

--max_constraints n: puts a limit on the maximum number of constraints the solver attempts to solve

--outfile PATH.csv: the path of the results csv file.