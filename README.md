# Computer Graphics Projects
Projects for CS2240 (Advanced Computer Graphics), Spring 2024. 
> As per Brown's Academic Code, the actual source code cannot be made public, but will be available upon request. 

# Path Tracer
- Implemented a physically-based renderer based on the path tracing algorithm -- a simple, elegant Monte Carlo sampling approach to solving the rendering equation. 
- Supports visual effects, e.g. soft shadows, color bleeding, caustics, depth of field estimation, denoising through stratified sampling, diffuse and specular BRDF importance sampling.
Example Outputs:
![refraction](https://github.com/jean-yoo/graphics/assets/93178936/dc887a2e-00d6-41b1-875f-c1564cd31416)
![cornell_box_full_lighting](https://github.com/jean-yoo/graphics/assets/93178936/2479d12f-2347-4ddd-a922-e1340e85df53)
![glossy](https://github.com/jean-yoo/graphics/assets/93178936/6b9855e1-89b4-425a-b4d8-5c8c63011537)
![mirror](https://github.com/jean-yoo/graphics/assets/93178936/59f6e303-fffe-4d14-8dfc-6f345f427340)

In order: depth of field, stratified sampling, importance sampling

![dof_0 7_3](https://github.com/jean-yoo/graphics/assets/93178936/04332b98-f419-48fb-8021-f5a1d8cb5a5d)
![cornell_box_stratified](https://github.com/jean-yoo/graphics/assets/93178936/e7faa8b8-6db4-4f68-ac7f-723717528354)
![cornell_box_diffuse_importance](https://github.com/jean-yoo/graphics/assets/93178936/bdd370e3-70a5-471e-98ae-4ba44522e592)
![cornell_phong_importance](https://github.com/jean-yoo/graphics/assets/93178936/af94c593-1025-497c-8bdd-f5f3c3fc88d0)



# Mesh
-  Laplacian mesh smoothing, subdivision, quadric error simplification, isotropic remeshing.

Simplification: 

<img width="758" alt="simplify_cow" src="https://github.com/jean-yoo/graphics/assets/93178936/72a1cfb6-91a6-4483-8e7d-954380a66bbe">

Subdivision (icosahedron into sphere):

<img width="660" alt="subdivide_icosahderon" src="https://github.com/jean-yoo/graphics/assets/93178936/ec98dcb7-c306-4982-a065-267bfe4aa0c3">

Mesh smoothing:

<img width="651" alt="bunny_noise" src="https://github.com/jean-yoo/graphics/assets/93178936/194f2799-a802-4c11-97c3-5a0e82c2049f">
<img width="620" alt="bunny_denoise" src="https://github.com/jean-yoo/graphics/assets/93178936/79bcd36c-733e-4ffd-a896-c2a603937e25">

# FEM (Finite Element Method)
- Animation of deformable solid objects using the Finite Element Method (FEM). 
- Divides a continuous chunk of material into a mesh made up of a finite number of discrete elements (tetrahedra). 
- Simulation of physical-based obejcts through force computation, time integration, simple collision resolution, and user interactivity.

https://github.com/jean-yoo/graphics/assets/93178936/27bc3269-89c1-4454-94f1-f593d333057d




# ARAP (As-Rigid-As-Possible Surface Modeling)
- Implemented a system for user-interactive deformation of 3D meshes.
- Mesh vertices can be re-positioned by clicking and dragging; the rest of the mesh is updated such that it moves as-rigidly-as-possible (i.e. the deformation it exhibits is close to a rigid transformation). The end result is a deformation that looks physically-plausible, as if the mesh has an underlying rig / skeletal armature.
- Formulated the deformation process as an optimization problem, alternating between estimating the best-fit rigid transformation for each mesh vertex and solving a sparse linear system to find new mesh vertex positions.

![armadillo](https://github.com/jean-yoo/graphics/assets/93178936/8c818e36-4d98-42c3-8123-8717132fea66)
![teapot](https://github.com/jean-yoo/graphics/assets/93178936/78b915bb-bcf9-47d3-914f-81fc5ce8a8f3)


