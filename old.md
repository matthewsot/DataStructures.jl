# Benchmark Report for */root/DataStructures.jl*

## Job Properties
* Time of benchmark: 24 Feb 2025 - 17:56
* Package commit: dirty
* Julia commit: d63ade
* Julia command flags: None
* Environment variables: `JULIA_NUM_THREADS => 1`

## Results
Below is a table of this job's results, obtained by running the benchmarks.
The values listed in the `ID` column have the structure `[parent_group, child_group, ..., key]`, and can be used to
index into the BaseBenchmarks suite to retrieve the corresponding benchmarks.
The percentages accompanying time and memory values in the below table are noise tolerances. The "true"
time/memory value for a given benchmark is expected to fall within this percentage of the reported value.
An empty cell means that the value was zero.

| ID                                                                    | time            | GC time | memory          | allocations |
|-----------------------------------------------------------------------|----------------:|--------:|----------------:|------------:|
| `["SparseIntSet", "create_fill"]`                                     |  89.490 μs (5%) |         | 271.59 KiB (1%) |         199 |
| `["SparseIntSet", "in while in"]`                                     |  21.330 ns (5%) |         |                 |             |
| `["SparseIntSet", "in while not in"]`                                 |  16.730 ns (5%) |         |                 |             |
| `["SparseIntSet", "iterate one"]`                                     |   2.791 μs (5%) |         |   16 bytes (1%) |           1 |
| `["SparseIntSet", "iterate two exclude one"]`                         |   6.022 μs (5%) |         |   16 bytes (1%) |           1 |
| `["SparseIntSet", "iterate two"]`                                     |   5.768 μs (5%) |         |   16 bytes (1%) |           1 |
| `["SparseIntSet", "pop push worst case"]`                             |   1.084 μs (5%) |         |   4.06 KiB (1%) |           3 |
| `["SparseIntSet", "pop push"]`                                        |  71.459 ns (5%) |         |                 |             |
| `["heap", "BinaryHeap", "make", "Float64", "10^1", "Min"]`            |   2.466 μs (5%) |         |  160 bytes (1%) |           3 |
| `["heap", "BinaryHeap", "make", "Float64", "10^1", "SlowMin"]`        |   2.444 μs (5%) |         |  160 bytes (1%) |           3 |
| `["heap", "BinaryHeap", "make", "Float64", "10^3", "Min"]`            |  13.540 μs (5%) |         |   7.89 KiB (1%) |           4 |
| `["heap", "BinaryHeap", "make", "Float64", "10^3", "SlowMin"]`        |  18.640 μs (5%) |         |   7.89 KiB (1%) |           4 |
| `["heap", "BinaryHeap", "make", "Int64", "10^1", "Min"]`              |   2.346 μs (5%) |         |  160 bytes (1%) |           3 |
| `["heap", "BinaryHeap", "make", "Int64", "10^3", "Min"]`              |  11.220 μs (5%) |         |   7.89 KiB (1%) |           4 |
| `["heap", "BinaryHeap", "pop", "Float64", "10^1", "Min"]`             |   1.300 μs (5%) |         |                 |             |
| `["heap", "BinaryHeap", "pop", "Float64", "10^1", "SlowMin"]`         |   1.294 μs (5%) |         |                 |             |
| `["heap", "BinaryHeap", "pop", "Float64", "10^3", "Min"]`             |  11.584 μs (5%) |         |                 |             |
| `["heap", "BinaryHeap", "pop", "Float64", "10^3", "SlowMin"]`         |  13.125 μs (5%) |         |                 |             |
| `["heap", "BinaryHeap", "pop", "Int64", "10^1", "Min"]`               |   1.287 μs (5%) |         |                 |             |
| `["heap", "BinaryHeap", "pop", "Int64", "10^3", "Min"]`               |   7.942 μs (5%) |         |                 |             |
| `["heap", "BinaryHeap", "push", "Float64", "10^1", "Min"]`            |   1.535 μs (5%) |         |  195 bytes (1%) |             |
| `["heap", "BinaryHeap", "push", "Float64", "10^1", "SlowMin"]`        |   1.646 μs (5%) |         |  195 bytes (1%) |             |
| `["heap", "BinaryHeap", "push", "Float64", "10^3", "Min"]`            |  26.720 μs (5%) |         |  21.78 KiB (1%) |           7 |
| `["heap", "BinaryHeap", "push", "Float64", "10^3", "SlowMin"]`        |  30.900 μs (5%) |         |  21.78 KiB (1%) |           7 |
| `["heap", "BinaryHeap", "push", "Int64", "10^1", "Min"]`              |   1.505 μs (5%) |         |  195 bytes (1%) |             |
| `["heap", "BinaryHeap", "push", "Int64", "10^3", "Min"]`              |  20.350 μs (5%) |         |  21.78 KiB (1%) |           7 |
| `["heap", "MutableBinaryHeap", "make", "Float64", "10^1", "Min"]`     |   2.494 μs (5%) |         |  400 bytes (1%) |           5 |
| `["heap", "MutableBinaryHeap", "make", "Float64", "10^1", "SlowMin"]` |   2.632 μs (5%) |         |  400 bytes (1%) |           5 |
| `["heap", "MutableBinaryHeap", "make", "Float64", "10^3", "Min"]`     |  23.300 μs (5%) |         |  23.59 KiB (1%) |           7 |
| `["heap", "MutableBinaryHeap", "make", "Float64", "10^3", "SlowMin"]` |  29.420 μs (5%) |         |  23.59 KiB (1%) |           7 |
| `["heap", "MutableBinaryHeap", "make", "Int64", "10^1", "Min"]`       |   2.471 μs (5%) |         |  400 bytes (1%) |           5 |
| `["heap", "MutableBinaryHeap", "make", "Int64", "10^3", "Min"]`       |  18.250 μs (5%) |         |  23.59 KiB (1%) |           7 |
| `["heap", "MutableBinaryHeap", "pop", "Float64", "10^1", "Min"]`      |   1.317 μs (5%) |         |                 |             |
| `["heap", "MutableBinaryHeap", "pop", "Float64", "10^1", "SlowMin"]`  |   1.338 μs (5%) |         |                 |             |
| `["heap", "MutableBinaryHeap", "pop", "Float64", "10^3", "Min"]`      |  15.468 μs (5%) |         |                 |             |
| `["heap", "MutableBinaryHeap", "pop", "Float64", "10^3", "SlowMin"]`  |  17.350 μs (5%) |         |                 |             |
| `["heap", "MutableBinaryHeap", "pop", "Int64", "10^1", "Min"]`        |   1.330 μs (5%) |         |                 |             |
| `["heap", "MutableBinaryHeap", "pop", "Int64", "10^3", "Min"]`        |  14.397 μs (5%) |         |                 |             |
| `["heap", "MutableBinaryHeap", "push", "Float64", "10^1", "Min"]`     |   2.024 μs (5%) |         |  632 bytes (1%) |             |
| `["heap", "MutableBinaryHeap", "push", "Float64", "10^1", "SlowMin"]` |   2.042 μs (5%) |         |  569 bytes (1%) |             |
| `["heap", "MutableBinaryHeap", "push", "Float64", "10^3", "Min"]`     |  63.060 μs (5%) |         |  65.00 KiB (1%) |          15 |
| `["heap", "MutableBinaryHeap", "push", "Float64", "10^3", "SlowMin"]` |  69.350 μs (5%) |         |  65.00 KiB (1%) |          15 |
| `["heap", "MutableBinaryHeap", "push", "Int64", "10^1", "Min"]`       |   1.909 μs (5%) |         |  569 bytes (1%) |             |
| `["heap", "MutableBinaryHeap", "push", "Int64", "10^3", "Min"]`       |  58.470 μs (5%) |         |  65.00 KiB (1%) |          15 |
| `["heap", "Slow nlargest", "a=rand(10^4)", "n=10^2"]`                 |  79.970 μs (5%) |         |   2.72 KiB (1%) |           6 |
| `["heap", "Slow nsmallest", "a=rand(10^4)", "n=10^2"]`                | 106.600 μs (5%) |         |   2.72 KiB (1%) |           6 |
| `["heap", "nlargest", "a=rand(10^4)", "n=10^2"]`                      |  66.940 μs (5%) |         |   2.72 KiB (1%) |           6 |
| `["heap", "nsmallest", "a=rand(10^4)", "n=10^2"]`                     |  64.230 μs (5%) |         |   2.72 KiB (1%) |           6 |
| `["trees", "avl", "biased"]`                                          | 100.787 ms (5%) |         |   6.10 MiB (1%) |      199490 |
| `["trees", "avl", "rand"]`                                            |   2.672 ms (5%) |         | 236.48 KiB (1%) |        9654 |
| `["trees", "avl", "redundant"]`                                       | 104.968 ms (5%) |         |   6.10 MiB (1%) |      199490 |
| `["trees", "rb", "biased"]`                                           |  75.321 ms (5%) |         |   7.62 MiB (1%) |      199491 |
| `["trees", "rb", "rand"]`                                             |   2.168 ms (5%) |         | 252.02 KiB (1%) |        9655 |
| `["trees", "rb", "redundant"]`                                        |  73.868 ms (5%) |         |   7.62 MiB (1%) |      199491 |
| `["trees", "splay", "biased"]`                                        |  41.822 ms (5%) |         |   6.10 MiB (1%) |      199490 |
| `["trees", "splay", "rand"]`                                          |   4.157 ms (5%) |         | 236.48 KiB (1%) |        9654 |
| `["trees", "splay", "redundant"]`                                     |   44.565 s (5%) |         |   6.10 MiB (1%) |      199490 |

## Benchmark Group List
Here's a list of all the benchmark groups executed by this job:

- `["SparseIntSet"]`
- `["heap", "BinaryHeap", "make", "Float64", "10^1"]`
- `["heap", "BinaryHeap", "make", "Float64", "10^3"]`
- `["heap", "BinaryHeap", "make", "Int64", "10^1"]`
- `["heap", "BinaryHeap", "make", "Int64", "10^3"]`
- `["heap", "BinaryHeap", "pop", "Float64", "10^1"]`
- `["heap", "BinaryHeap", "pop", "Float64", "10^3"]`
- `["heap", "BinaryHeap", "pop", "Int64", "10^1"]`
- `["heap", "BinaryHeap", "pop", "Int64", "10^3"]`
- `["heap", "BinaryHeap", "push", "Float64", "10^1"]`
- `["heap", "BinaryHeap", "push", "Float64", "10^3"]`
- `["heap", "BinaryHeap", "push", "Int64", "10^1"]`
- `["heap", "BinaryHeap", "push", "Int64", "10^3"]`
- `["heap", "MutableBinaryHeap", "make", "Float64", "10^1"]`
- `["heap", "MutableBinaryHeap", "make", "Float64", "10^3"]`
- `["heap", "MutableBinaryHeap", "make", "Int64", "10^1"]`
- `["heap", "MutableBinaryHeap", "make", "Int64", "10^3"]`
- `["heap", "MutableBinaryHeap", "pop", "Float64", "10^1"]`
- `["heap", "MutableBinaryHeap", "pop", "Float64", "10^3"]`
- `["heap", "MutableBinaryHeap", "pop", "Int64", "10^1"]`
- `["heap", "MutableBinaryHeap", "pop", "Int64", "10^3"]`
- `["heap", "MutableBinaryHeap", "push", "Float64", "10^1"]`
- `["heap", "MutableBinaryHeap", "push", "Float64", "10^3"]`
- `["heap", "MutableBinaryHeap", "push", "Int64", "10^1"]`
- `["heap", "MutableBinaryHeap", "push", "Int64", "10^3"]`
- `["heap", "Slow nlargest", "a=rand(10^4)"]`
- `["heap", "Slow nsmallest", "a=rand(10^4)"]`
- `["heap", "nlargest", "a=rand(10^4)"]`
- `["heap", "nsmallest", "a=rand(10^4)"]`
- `["trees", "avl"]`
- `["trees", "rb"]`
- `["trees", "splay"]`

## Julia versioninfo
```
Julia Version 1.11.3
Commit d63adeda50d (2025-01-21 19:42 UTC)
Build Info:
  Official https://julialang.org/ release
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  uname: Linux 6.1.0-31-cloud-amd64 #1 SMP PREEMPT_DYNAMIC Debian 6.1.128-1 (2025-02-07) x86_64 unknown
  CPU: QEMU Virtual CPU version 2.5+: 
                 speed         user         nice          sys         idle          irq
       #1-32     0 MHz      40413 s          0 s       3114 s   75246440 s          0 s
  Memory: 47.05205154418945 GB (46604.13671875 MB free)
  Uptime: 235316.23 sec
  Load Avg:  1.0  0.71  0.33
  WORD_SIZE: 64
  LLVM: libLLVM-16.0.6 (ORCJIT, k8-sse3)
Threads: 1 default, 0 interactive, 1 GC (on 32 virtual cores)
```