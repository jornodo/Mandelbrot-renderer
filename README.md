# Mandelbrot renderer
This is a Pluto notebook in julia that renders pictures of specific coordinates of the mandelbrot set.
It includes both a sequential way of doing so on GPU, and utilizes CUDA for rendering on GPU.

# Dependencies
In order to run it, you have to have julia installed, along with its dependencies, aswell as having CUDA installed with a 
compatible nvidia GPU.

To install dependencies, launch the julia REPL and run:

```julia
begin
    using Pkg
    dependencies = ["Pluto", "CUDA", "Images", "Colors", "PlutoUI"]
    Pkg.add(dependencies)
end
```

# Running
After dealing with this all that is left is running the notebook with Pluto.

From the Julia REPL run:
```julia
using Pluto; Pluto.run()
```

This will run the notebook server, and open it as a tab in your browser.