## `OceanMesh2D: Precise distance-based two-dimensional automated mesh generation toolbox intended for coast ocean/shallow water flow models`

<p align="center">
  <img src = "nesting.png"> &nbsp &nbsp &nbsp &nbsp
</p>
OceanMesh2D is a set of open-source MATLAB functions built off approaches and ideas from many prior works that are used to generate two-dimensional (2D) unstructured meshes for coastal circulation problems. These meshes are based on a variety of feature driven geometric--topographic mesh size functions that are generated according to user-defined parameters. Mesh generation is achieved through a force-balance algorithm combined with a number of topological improvement strategies aimed at improving the worst case triangle quality. The software embeds the mesh generation process into an object-orientated framework that contains pre- and post-processing workflows that make mesh generation flexible, reproducible, and scriptable. The objective of this paper is to introduce the functionality of the software.  

## `Code framework` 
`OceanMesh2D`  consists of four standalone classes that are called in sequence. 

    OceanMesh2D::
    ├── geodata -- process geospatial data.
    ├── edgefx  -- build mesh size functions.
    ├── meshgen -- generate mesh based on mesh size functions and boundaries.
    └── msh     -- store, write, read, inspect, and visualize meshes and their axuillary components for numerical simulation.

## `Starting Out`

After downloading and unzipping the current <a href="https://github.com/NDDEV/archive/master.zip">repository</a>, read the user guide avaiable here (click download PDF): 
https://www.overleaf.com/read/hsqjhvtbkgvj#/54715995/

The data for the following examples can be downloaded here: 
 https://drive.google.com/open?id=1LeQJFKaVCM2K59pKO9jDcB02yjTmJPmL
```
Example_1_NZ.m %<- A simple mesh around South Island New Zealand that uses GSHHS shoreline. 
Example_2_NY.m %<- A mesh around the Manhattan area that uses a DEM created from LiDAR data.  
Example_3_ECGC.m %<- An example that builds a mesh for the western North Atlatnic with local nests around the mid-Atlantic.
Example_4_JBAY.m %<- An extremely high-fidelity (15-m) mesh from LiDAR data around Jamaica Bay with CFL limiting.
Example_5_GBAY.m %<- An example of the polyline/thalweg mesh size function along the Houston Ship Channel. 

```

## `References!`

If you make use of `OceanMesh2D` please include a reference to the following:
```

[1] - OceanMesh2D 1.0: MATLAB-based software for 2-D mesh generation used in coastal circulation problems. Keith J. Roberts, William J. Pringle,Joannes J. Westerink," Geoscientifc Model Development (submitted June 2018). 
```

