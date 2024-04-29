# Computer Graphics Projects
Projects for CS2240 (Advanced Computer Graphics)
> As per Brown's Academic Code, the actual source code cannot be made public, but is available upon request. 

# Path Tracer
- Implemented a physically-based renderer based on the path tracing algorithm -- a simple, elegant Monte Carlo sampling approach to solving the rendering equation. 
- Supports visual effects, e.g. soft shadows, color bleeding, caustics, depth of field estimation, denoising through stratified sampling, diffuse and specular BRDF importance sampling. 

# Mesh
-  Laplacian mesh smoothing, subdivision, quadric error simplification, isotropic remeshing.

# FEM (Finite Element Method)
- Animation of deformable solid objects using the Finite Element Method (FEM). 
- Divides a continuous chunk of material into a mesh made up of a finite number of discrete elements (tetrahedra). 
- Simulation of physical-based obejcts through force computation, time integration, simple collision resolution, and user interactivity. 

# ARAP (As-Rigid-As-Possible Surface Modeling)
- Implemented a system for user-interactive deformation of 3D meshes.
- Mesh vertices can be re-positioned by clicking and dragging; the rest of the mesh is updated such that it moves as-rigidly-as-possible (i.e. the deformation it exhibits is close to a rigid transformation). The end result is a deformation that looks physically-plausible, as if the mesh has an underlying rig / skeletal armature.
- Formulated the deformation process as an optimization problem, alternating between estimating the best-fit rigid transformation for each mesh vertex and solving a sparse linear system to find new mesh vertex positions.