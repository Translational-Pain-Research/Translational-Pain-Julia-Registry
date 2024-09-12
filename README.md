# Translational-Pain-Research


[<img src="AntibodyMethodsDoseResponse-docs.svg" style="height: 2em;">](https://Translational-Pain-Research.github.io/AntibodyMethodsDoseResponse-documentation/)
[<img src="AdaptiveDensityApproximation-docs.svg" style="height: 2em;">](https://Translational-Pain-Research.github.io/AdaptiveDensityApproximation-documentation/)
[<img src="FittingObjectiveFunctions-docs.svg" style="height: 2em;">](https://Translational-Pain-Research.github.io/FittingObjectiveFunctions-documentation/)



## About

**Translational-Pain-Research** contains [Julia](https://julialang.org/) packages for the analysis of (antibody) dose-response curves: 

![](example.svg)

For applications, see the corresponding paper ([https://arxiv.org/abs/2407.06052](https://arxiv.org/abs/2407.06052)). In addition, the packages [`FittingObjectiveFunctions.jl`](https://github.com/Translational-Pain-Research/FittingObjectiveFunctions.jl) and [`AdaptiveDensityApproximation.jl`](https://github.com/Translational-Pain-Research/AdaptiveDensityApproximation.jl) may be of interest for general scientific projects.



## Installation


First, add the registry `Translational-Pain-Julia-Registry`:

```julia
using Pkg
Pkg.Registry.add()
Pkg.Registry.add(RegistrySpec(url = "https://github.com/Translational-Pain-Research/Translational-Pain-Julia-Registry"))
```

Then, the packages can be installed as usual. E.g. [`AntibodyMethodsDoseResponseConvenience.jl`](https://github.com/Translational-Pain-Research/AntibodyMethodsDoseResponseConvenience.jl), which installs all necessary dependencies for the analysis of dose-response curves:

```julia
using Pkg
Pkg.add("AntibodyMethodsDoseResponseConvenience")
```

### List of packages

| Package | Short Description |
| :------: | :-------- |
| [`FittingObjectiveFunctions.jl`](https://github.com/Translational-Pain-Research/FittingObjectiveFunctions.jl) | Dependency-free package to construct fitting objective functions from (measurement) data. |
| [`AdaptiveDensityApproximation.jl`](https://github.com/Translational-Pain-Research/AdaptiveDensityApproximation.jl) | Approximate density functions with discrete grids that can be refined adaptively. Contains additional calculation methods for grids (e.g. numerical integration). |
| [`AdaptiveDensityApproximationRecipes.jl`](https://github.com/Translational-Pain-Research/AdaptiveDensityApproximationRecipes.jl) | [`Plots.jl`](https://docs.juliaplots.org/stable/) recipes for the visualization of grids. |
| [`AntibodyMethodsDoseResponseConvenience.jl`](https://github.com/Translational-Pain-Research/AntibodyMethodsDoseResponseConvenience.jl) | Convenience package for the analysis of dose-response curves. Contains predefined analysis and plotting methods. Recommended for the analysis of dose-response data. |
| [`AntibodyMethodsDoseResponse.jl`](https://github.com/Translational-Pain-Research/AntibodyMethodsDoseResponse.jl) | Minimal package defining the underlying models and methods for the analysis of dose-response curves. Intended for the development of analysis methods from scratch. Requires fewer dependencies. |
| [`AntibodyMethodsDoseResponseRecipes.jl`](https://github.com/Translational-Pain-Research/AntibodyMethodsDoseResponseRecipes.jl) |  [`Plots.jl`](https://docs.juliaplots.org/stable/) recipes for `AntibodyMethodsDoseResponse` objects. |


## License

All packages are provided under MIT License (Expat). If you want to cite the packages in a scientific context, you might also want to cite the corresponding [paper](https://arxiv.org/abs/2407.06052).