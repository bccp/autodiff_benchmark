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
* Ensure you have a version of Python which is dynamically linked to libpython, or use one of the workarounds mentioned [here](https://pyjulia.readthedocs.io/en/latest/troubleshooting.html#your-python-interpreter-is-statically-linked-to-libpython). Personally, I just make a new Python kernel which uses the `python-jl` wrapper mentioned there, i.e.

    ```json
    {
     "argv": [
      "python-jl",
      "-m",
      "ipykernel_launcher",
      "-f",
      "{connection_file}"
     ],
     "display_name": "Python 3 (with Julia)",
     "language": "python"
    }
    ```
