<p align="center">
  <img src="https://avatars.githubusercontent.com/u/149065557" width="150" alt="JuliaMeshless logo"/>
</p>

<h1 align="center">JuliaMeshless</h1>

<p align="center">
  <em>A project for the development of Meshless Methods for PDEs in the Julia programming language.</em>
</p>

---

## Overview

JuliaMeshless provides a Julia ecosystem for meshless numerical methods — solving partial differential equations without traditional mesh generation. The organization develops tools for radial basis function collocation, point cloud generation, and multiphysics simulation, enabling researchers and engineers to work directly with scattered node distributions.

## Packages

| Package | Description | Status |
|---------|-------------|--------|
| [RadialBasisFunctions.jl](https://github.com/JuliaMeshless/RadialBasisFunctions.jl) | High-performance RBF interpolation and differential operators using local collocation. Supports PHS, IMQ, and Gaussian basis functions with GPU evaluation and autodiff (Enzyme, Mooncake). | [![Build Status][rbf-ci]][rbf-ci-url] |
| [WhatsThePoint.jl](https://github.com/JuliaMeshless/WhatsThePoint.jl) | Point cloud generation and manipulation for meshless PDE methods. Import surfaces from STL, volume discretization, normal computation, node repulsion, and spatial queries. | [![Build Status][wtp-ci]][wtp-ci-url] |
| [MeshlessMultiphysics.jl](https://github.com/JuliaMeshless/MeshlessMultiphysics.jl) | Meshless PDE solver framework with trait-based boundary conditions. Supports thermal, fluid, and extensible physics domains with GPU acceleration. | [![Build Status][mm-ci]][mm-ci-url] |

[rbf-ci]: https://github.com/JuliaMeshless/RadialBasisFunctions.jl/actions/workflows/CI.yml/badge.svg
[rbf-ci-url]: https://github.com/JuliaMeshless/RadialBasisFunctions.jl/actions/workflows/CI.yml
[wtp-ci]: https://github.com/JuliaMeshless/WhatsThePoint.jl/actions/workflows/CI.yml/badge.svg
[wtp-ci-url]: https://github.com/JuliaMeshless/WhatsThePoint.jl/actions/workflows/CI.yml
[mm-ci]: https://github.com/JuliaMeshless/MeshlessMultiphysics.jl/actions/workflows/CI.yml/badge.svg
[mm-ci-url]: https://github.com/JuliaMeshless/MeshlessMultiphysics.jl/actions/workflows/CI.yml

## Getting Started

RadialBasisFunctions.jl is registered in the General registry:

```julia
using Pkg
Pkg.add("RadialBasisFunctions")
```

The other packages can be added via URL:

```julia
Pkg.add(url="https://github.com/JuliaMeshless/WhatsThePoint.jl")
Pkg.add(url="https://github.com/JuliaMeshless/MeshlessMultiphysics.jl")
```

## Contributing

Contributions are welcome! Please open issues and pull requests on the individual package repositories.

## License

All packages are released under the [MIT License](https://opensource.org/licenses/MIT).
