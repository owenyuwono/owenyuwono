<h1 align="center">Owen Yuwono</h1>

<p align="center">
Engineer working across distributed backend systems, real-time graphics and simulation, and blockchain infrastructure.
</p>

---

### [poseidon](https://github.com/owenyuwono/poseidon)

Real-time FFT ocean running entirely on the GPU. Tessendorf-style spectrum synthesis builds the wave field in frequency space, a compute-shader IFFT transforms it per frame, and displacement plus normal maps are generated on device so nothing round-trips to the CPU. Written against WebGPU through Three.js TSL, so the same node graph compiles to WGSL.

`WebGPU` `TSL` `Three.js` `compute shaders` `FFT`

### [minos](https://github.com/owenyuwono/minos)

Custom engine in Rust and Vulkan. Geometry is virtualized in the Nanite sense: meshes are split into clusters, LOD is selected per cluster rather than per object, culling runs GPU-side, and triangles that fall below a pixel go through a software rasterizer instead of the hardware path. On top of that sits tectonic-based procedural planet generation, voxel terrain streamed on demand, and an FFT ocean.

`Rust` `Vulkan` `virtualized geometry` `GPU-driven culling` `voxel terrain`

### [tiamat](https://github.com/owenyuwono/tiamat)

Fluid dynamics with smoothed-particle hydrodynamics. The fluid is carried by particles rather than a grid, with density and pressure resolved from kernel-weighted neighbors each step, which lets free surfaces and splashes fall out of the solver instead of being faked.

`SPH` `fluid simulation` `particle systems`

### [gaia](https://github.com/owenyuwono/gaia)

Procedural grass generated and rendered in the browser. Generation is fully deterministic, so a given seed reproduces the same field every run, on every machine, with no baked assets to ship.

`Three.js` `procedural generation` `deterministic`

### [dryad](https://github.com/owenyuwono/dryad)

Trees grown procedurally from planet physics and a seed. Structure follows from the simulated conditions rather than from authored models, so the same generator produces different growth under different planetary parameters.

`Three.js` `procedural generation` `simulation`

<p align="center">
<a href="https://x.com/owenyuwono">@owenyuwono</a>
</p>
