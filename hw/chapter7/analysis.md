# Chapter 7: CPU Scheduling Analysis

## 1. Experiment Setup

Three jobs were used for this example experiment.
Their CPU burst lengths were 100, 200, and 300 time units.
All jobs arrive at time 0.

Scheduling algorithms:
- FIFO
- SJF
- RR with a time quantum of 5

## 2. Experimental Results

| Algorithm | Average Response Time | Average Turnaround Time | Average Wait Time |
|---|---:|---:|---:|
| FIFO | 133.33 | 333.33 | 133.33 |
| SJF | 133.33 | 333.33 | 133.33 |
| RR (q=5) | 5.00 | 461.67 | 261.67 |

## 3. Analysis

FIFO and SJF produced the same results because the jobs were already
listed in ascending order of their CPU burst lengths. Both algorithms
ran Job 0, then Job 1, and finally Job 2.

RR with a quantum of 5 provided a much lower average response time.
The first response times were 0, 5, and 10 time units, giving an
average response time of 5.

However, RR had higher average turnaround time and average wait time
than FIFO and SJF in this experiment. This happened because jobs
shared the CPU in time slices instead of running to completion in
sequence.

These results show that scheduling algorithms involve trade-offs
between response time, turnaround time, and waiting time.

Note: These are results from a practice workload. They must not be
treated as the answers to the official homework questions unless
the official questions specify the same workload and parameters.
