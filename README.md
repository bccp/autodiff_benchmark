# autodiff_benchmark

Repository to benchmark various autodiff framework for tasks useful in cosmology.


## Instructions

For the Julia cases you need:

* Install Julia (https://julialang.org/downloads/)
* Install the necessary Julia packages by running the following from this folder:
    ```
    julia --project=. -e 'using Pkg; pkg"instantiate"'
    ```
* Install the Julia magic for Jupyter:
    ```
    pip install julia
    ```
