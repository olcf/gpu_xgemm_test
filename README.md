# GPU XGEMM Test

This program fills 2 matrices with random floating-point numbers, performs a matrix multiply on the CPU, performs a matrix multiply on the GPU, then verifies the answers are the same to within expected limits.

## Usage

This program can be run in single- or double-precision and the size of the matrix can be changed with runtime flags:

```bash
$ ./gpu_xgemm --help
----------------------------------------------------------------
Usage: ./gpu_xgemm [OPTIONS]

--matrix_size=<value>, -m:       Size of matrices
                                 (default is 1024)

 --precision=<value>,   -p:       <value> can be single or double
                                 to select sgemm or dgemm
                                 (default is double)

 --help,                -h:       Show help
----------------------------------------------------------------
```
