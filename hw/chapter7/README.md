# Chapter 7: CPU Scheduling
두안주오팅  24215739
## Overview

This project explores three CPU scheduling algorithms:
- FIFO (First-In-First-Out)
- SJF (Shortest Job First)
- RR (Round-Robin)

The experiments use the OSTEP CPU scheduling simulator.

## Practice Workload

Three jobs were used with CPU burst lengths of 100, 200, and 300 time units.
For RR, the time quantum was set to 5.

## Results

| Algorithm | Average Response Time | Average Turnaround Time | Average Wait Time |
|---|---:|---:|---:|
| FIFO | 133.33 | 333.33 | 133.33 |
| SJF | 133.33 | 333.33 | 133.33 |
| RR (q=5) | 5.00 | 461.67 | 261.67 |

## Files

- `analysis.md`: Experimental results and analysis.
- `data/q1_fifo.txt`: FIFO simulator output.
- `data/q1_sjf.txt`: SJF simulator output.
- `data/q1_rr.txt`: RR simulator output.

Note: These are practice results. Confirm the official homework
questions and required parameters before using them as final answers.
