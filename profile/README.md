# r-xla

r-xla brings just-in-time compilation and automatic differentiation to R.
Write standard R code, compile it to optimized machine code, and run it on CPU or GPU.
It consists of many packages that are developed in tandem.
The end-user facing package is [anvil](https://github.com/r-xla/anvil).

## Packages

The core packages are:

| Package | Role |
|---------|------|
| [**anvil**](https://github.com/r-xla/anvil) | User-facing API: JIT compilation + autodiff |
| [**stablehlo**](https://github.com/r-xla/stablehlo) | IR layer: create and manipulate [StableHLO](https://github.com/openxla/stablehlo) programs |
| [**pjrt**](https://github.com/r-xla/pjrt) | Runtime: compile and execute on CPU/CUDA/Metal via [PJRT](https://github.com/openxla/xla/tree/main/xla/pjrt) |
| [**tengen**](https://github.com/r-xla/tengen) | Tensor generics |
| [**xlamisc**](https://github.com/r-xla/xlamisc) | Shared utilities |

Some supporting repositories:

| Repository | Role |
|------------|------|
| [**claude-config**](https://github.com/r-xla/claude-config) | Claude configuration for contributors |
| [**docker**](https://github.com/r-xla/docker) | Daily Docker images (CPU + CUDA) with anvil pre-installed |
| [**benchmarks**](https://github.com/r-xla/benchmarks) | Performance comparisons against PyTorch and R torch |
| [**actions**](https://github.com/r-xla/actions) | Shared GitHub Actions and CI workflows |
| [**pjrt-builds**](https://github.com/r-xla/pjrt-builds) | PJRT builds for Windows |
